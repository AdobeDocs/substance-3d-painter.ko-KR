---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/layering-declare-stacks-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter에 대한 레이어 지정 스택 셰이더 API 참조에 액세스하여 사용자 정의 재질 레이어 스택을 만듭니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > Layering Declare Stacks - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 레이어 형식 선언 스택 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 0%

---


# 레이어 형식 선언 스택 - 셰이더 API

## 재질 레이어: 편집 가능한 스택 선언

편집 가능한 스택은 고유한 식별자와 문서 채널 목록으로 정의됩니다. 가능한 채널 ID는 다음과 같습니다. *ambientocclusion* *anisotropyangle* *anisotropylevel* *basecolor* *blendingmask* *disperse* *변위* *방출* *광택도* *Height* *ior* *metallic* *normal* *opacity* *reflection* *거칠음* **&#x200B; Specular &#x200B;** specularlevel **&#x200B;투과&#x200B;** user0 **&#x200B; user1 &#x200B;** user2 **&#x200B; user3 &#x200B;** user4 **&#x200B; user5 &#x200B;** user6 **&#x200B; user7 &#x200B;**

예:

```
//:  stacks [ 

//:    { 

//:      "id": "Mask1", 

//:      "channels": [ 

//:        {"id": "opacity"} 

//:      ] 

//:    }, { 

//:      "id": "Mask2", 

//:      "channels": [ 

//:        {"id": "opacity"}, 

//:        {"id": "user0"} 

//:      ] 

//:    } 

//:  ]
```


스택의 식별자를 sampler 매개 변수에 바인딩하려면 채널 태그에 스택 태그를 접두어로 추가합니다.

```
//: param auto Mask1.channel_opacity 

uniform sampler2D mask_tex1; 

//: param auto Mask2.channel_opacity 

uniform sampler2D mask_tex2; 

 
```
