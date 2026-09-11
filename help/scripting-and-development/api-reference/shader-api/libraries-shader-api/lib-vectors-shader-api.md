---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-vectors-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 사용자 정의 셰이더에서 벡터 작업을 수행하려면 Lib 벡터 셰이더 API 참조에 액세스하십시오.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Vectors - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib 벡터 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 0%

---


# Lib 벡터 - 셰이더 API

## lib-vectors.glsl

**공용 함수:** *computeLocalFrame* *getEyeVec* *tangentSpaceToWorldSpace* *worldSpaceToTangentSpace*

라이브러리에서 가져오기

```
import lib-normal.glsl
```


음영 처리된 뷰는 무엇입니까?

```
//: param auto is_2d_view 

uniform bool is2DView;
```


어떤 종류의 투사가 사용됩니까?

```
//: param auto is_perspective_projection 

uniform bool is_perspective;
```


세계 공간의 눈 위치.

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


월드 공간에서 카메라 방향.

```
//: param auto world_camera_direction 

uniform vec3 camera_dir; 

 

//: param auto facing 

uniform int facing; 

 

bool isBackFace() { 

  return facing == -1 || (facing == 0 && !gl_FrontFacing); 

}
```


세계 공간 아이 벡터 계산

```
vec3 getEyeVec(vec3 position) { 

  return is_perspective ? 

    normalize(camera_pos - position) : 

    -camera_dir; 

}
```


벡터를 탄젠트 공간에서 월드 공간으로 변환

```
vec3 tangentSpaceToWorldSpace(vec3 vecTS, V2F inputs) { 

  return normalize( 

    vecTS.x * inputs.tangent + 

    vecTS.y * inputs.bitangent + 

    vecTS.z * inputs.normal); 

}
```


벡터를 월드 공간에서 탄젠트 공간으로 변환

```
vec3 worldSpaceToTangentSpace(vec3 vecWS, V2F inputs) { 

  // Assume the transformation is orthogonal 

  return normalize(vecWS * mat3(inputs.tangent, inputs.bitangent, inputs.normal)); 

}
```


월드 공간에서 정점의 로컬 프레임

```
struct LocalVectors { 

  vec3 vertexNormal; 

  vec3 tangent, bitangent, normal, eye; 

};
```


사용자 정의 세계 공간 표준 및 비등방성 각도에서 로컬 프레임 계산

```
LocalVectors computeLocalFrame(V2F inputs, vec3 normal, float anisoAngle) { 

  LocalVectors vectors; 

  vectors.vertexNormal = inputs.normal; 

  vectors.normal = normal; 

 

  // Flip the normals for back facing polygons 

  if (isBackFace()) { 

    vectors.vertexNormal = -vectors.vertexNormal; 

    vectors.normal = -vectors.normal; 

  } 

 

  vectors.eye = is2DView ? 

    vectors.normal : // In 2D view, put view vector along the normal 

    getEyeVec(inputs.position); 

 

  // Trick to remove black artifacts 

  // Backface ? place the eye at the opposite - removes black zones 

  if (dot(vectors.eye, vectors.normal) < 0.0) { 

    vectors.eye = reflect(vectors.eye, vectors.normal); 

  } 

 

  // Create a local frame for BRDF work 

  vec3 tangent = normalize( 

    inputs.tangent 

    * vectors.normal * dot(inputs.tangent, vectors.normal) 

  ); 

  vec3 bitangent = normalize( 

    inputs.bitangent 

    * vectors.normal * dot(inputs.bitangent, vectors.normal) 

    * tangent * dot(inputs.bitangent, tangent) 

  ); 

 

  float cosAngle = cos(anisoAngle); 

  float sinAngle = sin(anisoAngle); 

  vectors.tangent = cosAngle * tangent - sinAngle * bitangent; 

  vectors.bitangent = cosAngle * bitangent + sinAngle * tangent; 

 

  return vectors; 

}
```


메시 및 문서 Height 및 표준에서 로컬 프레임 계산

```
LocalVectors computeLocalFrame(V2F inputs) { 

  // Get world space normal 

  vec3 normal = computeWSNormal(inputs.sparse_coord, inputs.tangent, inputs.bitangent, inputs.normal); 

  return computeLocalFrame(inputs, normal, 0.0); 

} 

 
```
