---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-alpha-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 알파 채널 및 사용자 정의 셰이더의 투명도를 사용하여 작업하려면 Lib Alpha 셰이더 API 참조에 액세스하십시오.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Alpha - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Alpha - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '72'
ht-degree: 0%

---


# Lib Alpha - 셰이더 API

## lib-alpha.glsl

**공용 함수:** *alphaKill*

```
import lib-sampler.glsl 

import lib-random.glsl
```


불투명도 맵, 엔진에서 제공.

```
//: param auto channel_opacity 

uniform SamplerSparse opacity_tex;
```


Alpha 테스트 임계값입니다.

```
//: param custom { 

//:   "default": 0.33, 

//:   "label": "Alpha threshold", 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float alpha_threshold;
```


Alpha 테스트 디더링.

```
//: param custom { 

//:   "default": false, 

//:   "label": "Alpha dithering", 

//:   "group": "Common Parameters" 

//: } 

uniform bool alpha_dither;
```


알파 테스트 에뮬레이션 : 불투명도가 사용자 정의 임계값 미만인 경우 현재 조각을 버립니다. AFTER 텍스처 샘플링 호출로 불러야 합니다.

```
void alphaKill(float alpha) 

{ 

  float threshold = alpha_dither ? getBlueNoiseThresholdTemporal() : alpha_threshold; 

  if (alpha < threshold) discard; 

} 

 

void alphaKill(SparseCoord coord) 

{ 

  alphaKill(getOpacity(opacity_tex, coord)); 

} 

 
```
