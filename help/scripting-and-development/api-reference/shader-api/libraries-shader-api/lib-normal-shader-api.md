---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-normal-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter에 대한 [Lib 표준] 셰이더 API 참조에 액세스하여 사용자 정의 셰이더에서 표준 맵 및 표면 표준을 사용하여 작업할 수 있습니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Normal - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib 표준 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---


# Lib 표준 - 셰이더 API

## lib-normal.glsl

**공용 함수:** *normalBlend* *normalBlendOriented* *normalFade* *normalUnpack* *normalFromBaseNormal* *normalFromNormal* *normalFromHeight* *getTSNormal* *computeWSBaseNormal* *computeWSNormal*

라이브러리에서 가져오기

```
import lib-defines.glsl 

import lib-sparse.glsl
```


모든 엔진 매개변수는 일반 중심 작업에 유용합니다.

```
//: param auto channel_height 

uniform SamplerSparse height_texture; 

//: param auto channel_normal 

uniform SamplerSparse normal_texture; 

//: param auto texture_normal 

uniform SamplerSparse base_normal_texture; 

//: param auto normal_blending_mode 

uniform int normal_blending_mode;
```


표준 맵의 Y축을 반전하는 데 사용됩니다.

```
//: param auto normal_y_coeff 

uniform float base_normal_y_coeff;
```


우리 아티스트들이 경험적으로 결정한...

```
const float HEIGHT_FACTOR = 400.0;
```


2개의 표준 맵 간 혼합 수행

이는 Whiteout blending http://blog.selfshadow.com/publications/blending-in-detail/ 을 기반으로 합니다.

```
vec3 normalBlend(vec3 baseNormal, vec3 overNormal) 

{ 

  return normalize(vec3( 

    baseNormal.xy + overNormal.xy, 

    baseNormal.z  * overNormal.z)); 

}
```


2개의 표준 맵 간에 세부 방향 혼합 수행

이는 디테일 지향 블렌딩을 기반으로 합니다 http://blog.selfshadow.com/publications/blending-in-detail/

```
vec3 normalBlendOriented(vec3 baseNormal, vec3 overNormal) 

{ 

  baseNormal.z += 1.0; 

  overNormal.xy = -overNormal.xy; 

  return normalize(baseNormal * dot(baseNormal,overNormal) - 

    overNormal*baseNormal.z); 

}
```


감쇠 계수에 의해 병합된 일반 값을 반환합니다.

```
vec3 normalFade(vec3 normal,float attenuation) 

{ 

  if (attenuation<1.0 && normal.z<1.0) 

  { 

    float phi = attenuation * acos(normal.z); 

    normal.xy *= 1.0/sqrt(1.0-normal.z*normal.z) * sin(phi); 

    normal.z = cos(phi); 

  } 

 

  return normal; 

}
```


알파 채널이 있는 일반 압축 풀기

```
vec3 normalUnpack(vec4 normal_alpha, float y_coeff) 

{ 

  if (normal_alpha.a == 0.0 || normal_alpha.xyz == vec3(0.0)) { 

    return vec3(0.0, 0.0, 1.0); 

  } 

 

  // Attenuation in function of alpha 

  vec3 normal = normal_alpha.xyz/normal_alpha.a * 2.0 - vec3(1.0); 

  normal.y *= y_coeff; 

  normal.z = max(1e-3, normal.z); 

  normal = normalize(normal); 

  normal = normalFade(normal, normal_alpha.a); 

 

  return normal; 

}
```


알파 채널이 있는 일반 압축 풀기, Y 반전 없음

```
vec3 normalUnpack(vec4 normal_alpha) 

{ 

  return normalUnpack(normal_alpha, 1.0); 

}
```


문서의 Height 채널에서 탄젠트 공간 수직 계산

```
vec3 normalFromHeight(SparseCoord coord, float height_force) 

{ 

  // Normal computation using height map 

 

  // Determine gradient offset in function of derivatives 

  vec2 dfd = max(coord.dfdx,coord.dfdy); 

  dfd = max(dfd,height_texture.size.zw); 

 

  vec2 dfdx,dfdy; 

  textureSparseQueryGrad(dfdx, dfdy, height_texture, coord); 

  float h_r  = textureGrad(height_texture.tex, coord.tex_coord+vec2( dfd.x,  0    ), dfdx, dfdy).r; 

  float h_l  = textureGrad(height_texture.tex, coord.tex_coord+vec2(-dfd.x,  0    ), dfdx, dfdy).r; 

  float h_t  = textureGrad(height_texture.tex, coord.tex_coord+vec2(     0,  dfd.y), dfdx, dfdy).r; 

  float h_b  = textureGrad(height_texture.tex, coord.tex_coord+vec2(     0, -dfd.y), dfdx, dfdy).r; 

  float h_rt = textureGrad(height_texture.tex, coord.tex_coord+vec2( dfd.x,  dfd.y), dfdx, dfdy).r; 

  float h_lt = textureGrad(height_texture.tex, coord.tex_coord+vec2(-dfd.x,  dfd.y), dfdx, dfdy).r; 

  float h_rb = textureGrad(height_texture.tex, coord.tex_coord+vec2( dfd.x, -dfd.y), dfdx, dfdy).r; 

  float h_lb = textureGrad(height_texture.tex, coord.tex_coord+vec2(-dfd.x, -dfd.y), dfdx, dfdy).r; 

 

  vec2 dh_dudv = (0.5 * height_force) / dfd * vec2( 

    2.0*(h_l-h_r)+h_lt-h_rt+h_lb-h_rb, 

    2.0*(h_b-h_t)+h_rb-h_rt+h_lb-h_lt); 

 

  return normalize(vec3(dh_dudv, HEIGHT_FACTOR)); 

}
```


기본 수직과 Height 값으로부터 탄젠트 공간 수직을 계산하고 선택적 세부 수직을 계산하는 도우미

```
vec3 getTSNormal(SparseCoord coord, vec3 normalFromHeight) 

{ 

  vec3 normal = normalBlendOriented( 

    normalUnpack(textureSparse(base_normal_texture, coord), base_normal_y_coeff), 

    normalFromHeight); 

 

  if (normal_texture.is_set) { 

    vec3 channelNormal = normalUnpack(textureSparse(normal_texture, coord)); 

    if (normal_blending_mode == BlendingMode_Replace) { 

      normal = normalBlendOriented(normalFromHeight, channelNormal); 

    } else if (normal_blending_mode == BlendingMode_NM_Combine) { 

      normal = normalBlendOriented(normal, channelNormal); 

    } 

  } 

 

  return normal; 

}
```


기본 수직과 Height에서 탄젠트 공간 수직을 계산하고 선택적 세부 수직을 계산하는 도우미

```
vec3 getTSNormal(SparseCoord coord) 

{ 

  float height_force = 1.0; 

  vec3 normalH = normalFromHeight(coord, height_force); 

  return getTSNormal(coord, normalH); 

}
```


탄젠트 공간 베이스 수직에서 월드 공간 수직을 계산하는 도우미.

```
vec3 computeWSBaseNormal(SparseCoord coord, vec3 tangent, vec3 bitangent, vec3 normal) 

{ 

  vec3 normal_vec = normalUnpack(textureSparse(normal_texture, coord), base_normal_y_coeff); 

  return normalize( 

    normal_vec.x * tangent + 

    normal_vec.y * bitangent + 

    normal_vec.z * normal 

  ); 

}
```


getTSNormal 도우미 및 메시의 로컬 프레임에서 제공된 탄젠트 공간 법선에서 월드 공간 법선을 계산하는 도우미.

```
vec3 computeWSNormal(SparseCoord coord, vec3 tangent, vec3 bitangent, vec3 normal) 

{ 

  vec3 normal_vec = getTSNormal(coord); 

  return normalize( 

    normal_vec.x * tangent + 

    normal_vec.y * bitangent + 

    normal_vec.z * normal 

  ); 

} 

 
```
