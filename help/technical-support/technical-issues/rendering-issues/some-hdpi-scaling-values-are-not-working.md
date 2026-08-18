---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/some-hdpi-scaling-values-are-not-working.html"
breadcrumb-title: ''
description: 적절한 고해상도 디스플레이 지원을 위해 Substance 3D Painter에서 HDPI 비율 값 문제를 해결하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Some HDPI scaling values are not working
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 일부 HDPI 비율 값이 작동하지 않음
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%

---


# 일부 HDPI 비율 값이 작동하지 않음

Windows에서는 일부 HDPI 비율 값(높은 해상도의 모니터에서 인터페이스 비율을 조정하는 데 사용됨)이 제대로 작동하지 않을 수 있습니다.\
이는 당사의 윈도우 프레임워크(Qt)가 이를 지원하지 않기 때문입니다. 프레임워크 자체의 제공자가 실제로 관리할 때까지 이 문제를 해결할 수 없습니다.

따라서 설정에 따라 발생할 수 있는 동작은 다음과 같습니다.

* 120DPI(**125%** 비율) - 96DPI로 렌더링됨(**100%** 비율)
* 144DPI(**150%** 비율) - 192DPI(**200%** 비율)로 렌더링됨
* 168DPI(**175%** 비율) - 192DPI(**200%** 비율)로 렌더링됨

자세한 내용은 <https://bugreports.qt.io/browse/QTBUG-55654>을(를) 참조하십시오.
