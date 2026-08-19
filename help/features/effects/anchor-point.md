---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/features/effects/anchor-point.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 기준점 효과를 사용하여 다른 레이어의 텍스처를 참조하여 고급 합성을 만드는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Anchor Point
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 고정점
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---


# 고정점

기준점은 레이어 스택의 리소스 또는 요소를 노출하고 레이어 스택의 다른 영역에 참조하여 용도에 따라 그리고 조정한 내용에 따라 진행하는 방법입니다. 레이어 또는 마스크를 효과적으로 연결하고 단일 기준점이 프로젝트의 여러 측면에 영향을 미치도록 하는 등 완전히 새로운 가능성을 열어주어 Substance 3D Painter을 진정한 비선형 환경으로 변화시킬 수 있습니다.

>[!NOTE]
>
> 기준점은 동일한 텍스처가 만들어진 내에서만 참조할 수 있습니다. 텍스처 세트 간에는 앵커와 해당 참조 간에 링크를 만들 수 없습니다.

## 고정점 추가

효과 메뉴에서 기준점 사용 가능 레이어와 마스크 모두에 추가할 수 있습니다.

![](../../assets/add-anchor-point.png)

## 기준점을 참조로 사용

기준점은 다른 레이어에서 참조할 수 있습니다. 이렇게 하면 기준점을 참조하는 레이어로 기준점의 콘텐츠가 인스턴스화됩니다.

기준점은 다음 리소스에서 참조로 사용할 수 있습니다.

* 채우기 레이어
* 채우기 효과
* Substance 필터 입력(효과, 절차, 생성기)

![](../../assets/anchor-point-resource.png)

참조하는 레이어에서 **아래**&#x200B;인 기준점만 참조로 사용할 수 있습니다.\
기준점을 참조하는 레이어 위로 기준점을 이동하면 해당 기준점이 해제됩니다. 이 작업을 취소하려면 실행 취소할 수 있습니다.

![](../../assets/layer-broken.png)![](../../assets/reference-broken.png)

## 고정점에 대한 참조 찾기

기준점을 클릭하면 속성 패널에서 이 기준점이 참조로 사용되는 레이어 목록을 볼 수 있습니다.

![](../../assets/references.png)

## 고정점 찾기

기준점을 참조로 사용하는 칠 레이어/효과인 경우 기준점으로 이동할 수 있습니다.

![](../../assets/jump-to-anchor-point.png)
