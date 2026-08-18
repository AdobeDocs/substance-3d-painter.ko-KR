---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/toon-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter의 툰 셰이더 API 참조에 액세스하여 사용자 정의 툰 스타일 렌더링 효과를 만듭니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Toon - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 툰 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# 툰 - 셰이더 API

## 기본 툰 셰이더

라이브러리에서 가져옵니다.

```
import lib-sampler.glsl
```


우리는 전체 빛의 위치를 정의한다

```
const vec3 light_pos = vec3(10.0, 10.0, 10.0);
```


자동 매개 변수 세계 눈 위치를 **camera\_pos**&#x200B;에 **바인딩**&#x200B;합니다.

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


**문서의 채널**&#x200B;기본 색상&#x200B;**을(를) 균일한**&#x200B;기본 색상\_tex **에 바인딩**&#x200B;합니다.

```
//: param auto channel_basecolor 

uniform SamplerSparse basecolor_tex;
```


**메쉬 곡률**&#x200B;을 균일한 **곡률\_tex**&#x200B;에 **바인딩**&#x200B;합니다. 곡률을 사용할 수 없는 경우 투명 텍스처가 제공됩니다.

```
//: param auto texture_curvature 

uniform SamplerSparse curvature_tex;
```


이 셰이더에 대한 새 사용자 정의 트윅을 기본값과 함께 정의합니다. 이 옵션은 그림자가 표시되면 윤곽선의 Thickness을 조정하는 데 사용됩니다.

```
//: param custom { 

//:  "default": 0.4, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Unlit outline thickness" 

//: } 

uniform float unlit_outline_thickness;
```


이 셰이더에 대한 새 사용자 정의 트윅을 기본값과 함께 정의합니다. 이 클립은 불이 켜져 있을 때 외곽선의 Thickness을 조정하는 데 사용됩니다.

```
//: param custom { 

//:   "default": 0.1, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Lit outline thickness" 

//: } 

uniform float lit_outline_thickness;
```


우리가 곡률을 사용하는 것을 선호하는지 아닌지.

```
//: param custom { 

//:   "default": false, 

//:   "label": "Use curvature" 

//: } 

uniform bool use_curvature;
```


셰이더의 진입점입니다.

```
void shade(V2F inputs) 

{
```


우리는 몇 가지 유용한 값을 계산한다.

```
  vec3 V = normalize(camera_pos - inputs.position); 

  vec3 N = normalize(inputs.normal); 

  vec3 L = normalize(light_pos - inputs.position); 

  float NdV = dot(N, V); 

  float NdL = max(0.0, dot(N, L));
```


**우선 순위**&#x200B;는 **윤곽선 검색**&#x200B;을 수행하는 것입니다. 사용자가 윤곽선 감지를 위해 곡률 맵을 사용할지 여부를 선택할 수 있도록 허용합니다.

```
  if (use_curvature) { 

    float curv = textureSparse(curvature_tex, inputs.sparse_coord).r; 

    NdV = 1.0 - curv; 

  }
```


윤곽선 조건에 도달하면 검은색으로 종료합니다.

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  }
```


여기서, 우리는 색상의 4단계 이산화를 수행한다.

```
  vec3 color = getBaseColor(basecolor_tex, inputs.sparse_coord); 

  if (NdL > 0.75) { 

    color = color; 

  } else if (NdL > 0.5) { 

    color = color * 0.5; 

  } else if (NdL > 0.1) { 

    color = color * 0.1; 

  } 

  else
```


대체(fallback)가 검정입니다.

```
    color = vec3(0.0); 

 

  diffuseShadingOutput(color); 

} 

 
```
