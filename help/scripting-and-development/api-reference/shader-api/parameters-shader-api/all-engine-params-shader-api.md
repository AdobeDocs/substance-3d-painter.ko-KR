---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-engine-params-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter에 대한 모든 엔진 매개변수 셰이더 API 참조에 액세스하여 엔진 레벨 셰이더 매개변수를 제어합니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Engine Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 모든 엔진 매개변수 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# 모든 엔진 매개변수 - 셰이더 API

## 엔진 매개변수 예

## 텍스처 매개 변수

Substance Painter은 SVT(Sparse Virtual Texture) 시스템을 사용하여 뷰포트에 텍스처를 표시합니다.

이 시스템에 대한 자세한 내용은 [온라인 설명서](../../../../features/sparse-virtual-textures.md)를 참조하십시오.

이 시스템은 셰이더 코드를 작성하는 방법에 영향을 미칩니다. *SamplerSparse* 구조 및 텍스처 조회 함수를 사용하여 사용을 단순화하는 데 도움을 주고 있습니다([lib-sparse.glsl](../libraries-shader-api/lib-sparse-shader-api.md) 참조).

기본 사용법:

```
// Defines the SamplerSparse structure 

import lib-sparse.glsl 

 

//: param auto TEXTURE_TAG 

uniform SamplerSparse uniform_tex;   // Texture sampler and its information
```


텍스처 매개 변수를 사용하면 &#39;or&#39; 연산자를 사용하여 대체(fallback)를 정의할 수 있습니다.

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform SamplerSparse uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2
```


여기서 *TEXTURE\_TAG*&#x200B;는 아래 설명된 태그 중 하나입니다.

### 문서의 채널 태그

이러한 모든 텍스처는 이음새 문제를 방지하기 위해 **미리 곱하기** 및 **확장**&#x200B;됩니다.

**텍스처 집합 채널**

*채널\_ambientocclusion* *채널\_anisotropyangle* *채널\_anisotropylevel* *채널\_basecolor* *채널\_blendingmask* *채널\_disperse* *채널\_변위* *채널\_emissive* *채널\_glossness* *채널\_emissive* *채널\_ior* *채널\_metallic* *채널\_normal* *채널\_opacity* *채널\_반사* *채널\_거칠기* *채널\_산란* *채널\_Specular* *채널\_specularlevel* *채널\_투과성*

**사용자 채널**

*채널\_사용자0* *채널\_사용자1* *채널\_사용자2* *채널\_사용자3* *채널\_사용자4* *채널\_사용자5* *채널\_사용자6* *채널\_사용자7*

### 메시 맵

*텍스처\_ambientocclusion* : 주변 오클루전 맵\
*텍스처\_곡률* : 곡률 맵\
*텍스처\_id* : ID 맵\
*텍스처\_표준* : 접선 공간 표준 맵\
*텍스처\_표준\_ws* : 월드 공간 표준 맵\
*텍스처\_위치* : 세계 공간 위치 맵\
*텍스처\_Thickness* : Thickness 맵

## 추가 텍스처 매개 변수

기본 사용법:

```
//: param auto TEXTURE_TAG 

uniform sampler2D uniform_tex;   // The texture itself 

 

//: param auto TEXTURE_TAG_size 

uniform vec4 uniform_tex_size;   // The size of the texture (width, height, 1/width, 1/height)
```


텍스처 매개 변수를 사용하면 &#39;or&#39; 연산자를 사용하여 대체(fallback)를 정의할 수 있습니다.

```
//: param auto TEXTURE_TAG_1 or TEXTURE_TAG_2 

uniform sampler2D uniform_tex; // if TEXTURE_TAG_1 exists then TEXTURE_TAG_1 else TEXTURE_TAG_2 

 

//: param auto TEX_TAG_1_size or TEX_TAG_2_size 

uniform vec4 uniform_tex_size; // if TEX_TAG_1 exists then TEX_TAG_1_size else TEX_TAG_2_size
```


여기서 *TEXTURE\_TAG*&#x200B;는 아래 설명된 태그 중 하나입니다.

*텍스처\_파랑\_노이즈* : 파랑 노이즈 텍스처\
*텍스처\_환경* : 환경 맵, **mip-mapped**, [lib-env.glsl](../libraries-shader-api/lib-env-shader-api.md)을 사용하여 이 맵 사용

## 기타 매개 변수

*종횡비* : 뷰포트 *너비/Height* 비율을 포함하는 *부동*

```
//: param auto aspect_ratio 

uniform float uniform_aspect_ratio;
```


*camera\_view\_matrix* : 월드 공간에서 카메라 공간으로 변환을 나타내는 *mat4*

```
//: param auto camera_view_matrix 

uniform mat4 uniform_camera_view_matrix;
```


*camera\_view\_matrix\_it* : *camera\_view\_matrix*&#x200B;의 역 전치 버전

```
//: param auto camera_view_matrix_it 

uniform mat4 uniform_camera_view_matrix_it;
```


*camera\_vp\_matrix\_inverse* : *투영 \* 카메라\_뷰\_행렬* 행렬의 반전

```
//: param auto camera_vp_matrix_inverse 

uniform mat4 uniform_camera_vp_matrix_inverse;
```


*환경\_노출* : 엔브맵의 노출을 나타내는 *부동 소수점*

```
//: param auto environment_exposure 

uniform float uniform_environment_exposure;
```


*환경\_max\_lod* : mip-map 피라미드의 envmap 깊이를 나타내는 *float*

```
//: param auto environment_max_lod 

uniform float uniform_max_lod;
```


*환경\_회전* : 위쪽 축을 중심으로 한 엔브맵의 회전을 나타내는 *부동*\
값의 범위는 [0,1]이며 [0, 2\*pi] 범위로 매핑되어야 합니다.

```
//: param auto environment_rotation 

uniform float uniform_environment_rotation;
```


*페이싱* : 렌더링된 얼굴(-1: 뒷면, 0: 정의되지 않음, 1: 앞면)을 나타내는 *정수*\
값이 0이면 glsl 내장 변수 *gl\_FrontFacing*&#x200B;에 안전하게 의존할 수 있습니다.

```
//: param auto facing 

uniform int uniform_facing;
```


*fovy* : Y축을 따라 카메라 시야를 나타내는 *부동 소수점*

```
//: param auto fovy 

uniform float uniform_fovy;
```


*is\_2d\_view* : 2D 보기에 대해 렌더링을 수행할지 여부를 나타내는 *bool*

```
//: param auto is_2d_view 

uniform bool uniform_2d_view;
```


*is\_perspective\_projection* : 투사가 원근법인지 직교 투영인지를 나타내는 *bool*

```
//: param auto is_perspective_projection 

uniform bool uniform_perspective_projection;
```


*주\_조명* : 환경에서 주 조명의 위치를 나타내는 *vec4*

```
//: param auto main_light 

uniform vec4 uniform_main_light;
```


*mvp\_matrix* : 모델 뷰 투영 행렬을 나타내는 *mat4*

```
//: param auto mvp_matrix 

uniform mat4 uniform_mvp_matrix;
```


*장면\_원본\_반경* : 정규화 전에 장면의 테두리 구의 반경을 나타내는 *부동 소수점*

```
//: param auto scene_original_radius 

uniform float uniform_scene_original_radius;
```


*화면\_크기* : 화면 크기 데이터 *(너비, Height, 1/너비, 1/Height)을 포함하는* vec4 **

```
//: param auto screen_size 

uniform vec4 uniform_screen_size;
```


*world\_camera\_direction* : 세계 카메라 방향을 나타내는 *vec3*

```
//: param auto world_camera_direction 

uniform vec3 uniform_world_camera_direction;
```


*세계 눈\_위치* : 세계 눈 위치를 나타내는 *vec3*

```
//: param auto world_eye_position 

uniform vec3 uniform_world_eye_position; 

 
```
