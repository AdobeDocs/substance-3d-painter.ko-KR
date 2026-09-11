---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/generic-filter.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 일반 필터 효과를 만들어 사용자 정의 이미지 처리 및 텍스처 필터를 적용하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Generic filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 일반 필터
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---


# 일반 필터

불투명도를 포함한 일반 효과가 모든 문서 채널에 적용됩니다. 일반 필터는 다음과 같을 수 있습니다.

* **회색 음영**, 각 채널의 각 구성 요소(R, G, B 및 A)(기본 색상, 금속, 거칠기 등)에 적용됩니다.
* **색상**&#x200B;으로, 색상이 적용된 채널에 그대로 적용되거나 내부적으로 회색 음영으로 변환되어 회색 음영 채널에 영향을 줍니다

효과의 입력 노드에는 **입력**&#x200B;에 정의된 **식별자** 또는 **사용량**&#x200B;이 있어야 하고 해당 출력 노드에는 **출력**&#x200B;이 있어야 합니다. 레이어의 마스크에는 **색상** 기반 필터를 사용할 수 없습니다. **회색 음영** 필터만 호환됩니다.

>[!NOTE]
>
> 입력 노드에서 **사용량** 또는 **식별자**&#x200B;을(를) 사용할 수 있습니다(사용량에 우선 순위가 있음).

예 :

![](../../assets/generic-filter.png)![](../../assets/generic-rgba.png){width="575px"}
