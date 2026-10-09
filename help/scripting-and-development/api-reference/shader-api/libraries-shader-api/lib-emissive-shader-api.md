---
breadcrumb-title: ""
description: Substance 3D Painter용 Lib 방출 셰이더 API 참조에 액세스하여 방출 재질 및 광선 효과를 만듭니다.
title: Lib 방출 - 셰이더 API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 0%
---

# Lib 방출 - 셰이더 API

## lib-방출.glsl

**공용 함수:** *pbrComputeEmissive*

라이브러리에서 가져오기

```
import lib-sparse.glsl
```


방출 채널 텍스처.

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


보는 사람의 눈까지 방출 광도 계산

```
vec3 pbrComputeEmissive(SamplerSparse emissive, SparseCoord coord) 

{ 

  return emissive_intensity * textureSparse(emissive, coord).rgb; 

} 

 
```
