---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/surface-shader-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter의 Surface 셰이더 API 참조에 액세스하여 사용자 정의 표면 셰이더 효과 및 재질을 만듭니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Surface Shader - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 서피스 셰이더 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---


# 서피스 셰이더 - 셰이더 API

## surface-shader.glsl

Substance Painter에 사용할 수 있는 셰이더 리소스를 만들려면 다음 프로필로 *음영*&#x200B;이라는 단일 함수를 포함하는 glsl 파일을 만듭니다.

```
void shade(V2F inputs);
```


## V2F 입력 형식 정의:

```
struct V2F { 

  vec3 normal;               // interpolated normal 

  vec3 tangent;              // interpolated tangent 

  vec3 bitangent;            // interpolated bitangent 

  vec3 position;             // interpolated position 

  vec4 color[1];             // interpolated vertex colors (color0) 

  vec2 tex_coord;            // interpolated texture coordinates (uv0) 

  SparseCoord sparse_coord;  // interpolated sparse texture coordinates used by textureSparse() sampling function 

  vec2 multi_tex_coord[8];   // interpolated texture coordinates (uv0-uv7) 

};
```


참고: uv1-uv7에 대한 SparseCoord를 얻으려면 [lib-sparse.glsl](../libraries-shader-api/lib-sparse-shader-api.md)에 정의된 *getSparseCoord(vec2)*&#x200B;을(를) 명시적으로 호출해야 합니다.

## 서피스 셰이더 출력:

조각 속성을 설명하기 위해 *shade* 함수 내에서 다음 함수를 호출할 수 있습니다.

```
// fragment opacity. default value: 1.0 

void alphaOutput(float); 

// diffuse lighting contribution. default value: vec3(0.0) 

void diffuseShadingOutput(vec3); 

// specular lighting contribution. default value: vec3(0.0) 

void specularShadingOutput(vec3); 

// color emitted by the fragment. default value: vec3(0.0) 

void emissiveColorOutput(vec3); 

// fragment color. default value: vec3(1.0) 

void albedoOutput(vec3); 

// subsurface scattering properties, see lib-sss.glsl for details. default value: vec4(0.0) 

void sssCoefficientsOutput(vec4);
```


예를 들어, 조각 색상을 계산하는 가장 기본적인 렌더링 방정식은 *emissiveColor + 알베도 \* diffuseShading + specularShading*입니다.
