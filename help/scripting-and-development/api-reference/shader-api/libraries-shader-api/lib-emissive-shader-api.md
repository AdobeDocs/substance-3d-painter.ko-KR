---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-emissive-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter용 Lib Emissive 셰이더 API 참조에 액세스하여 발광 재질 및 광선 효과를 생성합니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Emissive - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib Emissive - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%

---


# Lib Emissive - 셰이더 API

## lib-emissive.glsl

**공용 함수:** *pbrComputeEmissive*

라이브러리에서 가져오기

```
import lib-sparse.glsl
```


발광 채널 텍스처입니다.

```
//: param auto channel_emissive 

uniform SamplerSparse emissive_tex;
```


방출 강도를 조정하는 데 사용되는 값입니다.

```
//: param custom { 

//:   "default": 1.0, 

//:   "label": "Emissive Intensity", 

//:   "min": 0.0, 

//:   "max": 100.0, 

//:   "group": "Common Parameters" 

//: } 

uniform float emissive_intensity;
```


보는 사람의 눈까지 방출 광도를 계산합니다.

```
vec3 pbrComputeEmissive(SamplerSparse emissive, SparseCoord coord) 

{ 

  return emissive_intensity * textureSparse(emissive, coord).rgb; 

} 

 
```
