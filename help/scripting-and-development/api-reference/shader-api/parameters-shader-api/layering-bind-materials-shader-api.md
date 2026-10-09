---
breadcrumb-title: ""
description: Substance 3D Painter의 레이어 바인딩 재질 셰이더 API 참조에 액세스하여 레이어 워크플로우에서 재질을 바인딩합니다.
title: 바인딩 재질 레이어 구성 - 셰이더 API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%
---

# 바인딩 재질 레이어 구성 - 셰이더 API

## 재질 레이어 구성: 재질을 셰이더 매개 변수로 바인딩합니다.

재질은 고유한 식별자 &#39;id&#39;로 정의됩니다. 추가 매개 변수:

* &#39;default&#39;: 사용할 기본 재료 자원 이름입니다.
* &#39;size&#39;: 질감 맵의 텍스처 크기입니다.
* &#39;group&#39;: 재질 선택 위젯의 UI 그룹입니다.

예:

```
//:  materials [ 

//:    { 

//:       "id": "Material1", 

//:       "default": "Concrete 044", 

//:       "size": 512, 

//:       "group": "Material 1" 

//:    }, { 

//:       "id": "Material2", 

//:       "default": "Leaves elm", 

//:       "size": 1024, 

//:       "group": "Material 2" 

//:    } 

//:  ]
```


재질의 채널을 샘플러에 바인딩하려면 재질의 ID와 채널 태그를 차례로 사용하여 자동 매개 변수를 정의합니다([all-engine-params.glsl](all-engine-params-shader-api.md)의 사용 가능한 채널 참조).

```
//: param auto Material1.channel_basecolor 

uniform sampler2D basecolor_tex1; 

//: param auto Material1.channel_metallic 

uniform sampler2D metallic_tex1; 

//: param auto Material1.channel_roughness 

uniform sampler2D roughness_tex1; 

 

//: param auto Material2.channel_basecolor 

uniform sampler2D basecolor_tex2; 

//: param auto Material2.channel_metallic 

uniform sampler2D metallic_tex2; 

//: param auto Material2.channel_roughness 

uniform sampler2D roughness_tex2; 

 
```
