---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/painting/tool-list/polygon-fill.html"
breadcrumb-title: ''
description: Substance 3D Painter의 다각형 채우기 도구를 사용하여 선택한 다각형을 페인트로 채우면 텍스처 페인팅이 효율적으로 수행됩니다.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Polygon fill
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 다각형 채우기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 1%

---


# 다각형 채우기

**다각형 채우기** 도구(![](../../assets/image2018-6-12-18-15-12.png))를 사용하면 선택한 다각형을 픽셀 마스크로 변환하여 마스크를 빠르게 그릴 수 있습니다. 다른 3DCC 응용 프로그램의 3D 선택 도구처럼 보일 수 있지만 실제로는 픽셀 데이터가 생성되는 페인팅 채우기 도구입니다. 즉, 작품을 선택하고 선택 취소한 다음 이를 사용하여 흰색이나 검은색으로 페인팅합니다.

다각형 채우기 도구는 [페인트 레이어](../../interface/layer-stack/layer-stack.md)에서 작동하지만 기본색으로만 제한되며 이러한 용도로 사용되지 않습니다. [마스크에만 사용](../../interface/layer-stack/masking-and-effects.md).

여기에는 4가지 선택 모드가 있습니다.

* ![](../../assets/image2020-9-30-11-31-53.png) **삼각형 채우기** - 개별 메시 트리를 채웁니다.
* ![](../../assets/image2020-9-30-11-32-12.png) **다각형 채우기** - 전체 다각형을 채웁니다. 메쉬가 내보낼 때 이미 삼각측정되어 있는 경우 삼각형 채우기와 다른 작업을 수행하지 않습니다.
* **![](../../assets/image2020-9-30-11-32-42.png)메시 채우기** - 연결된 전체 하위 메시를 채웁니다. 3D 애플리케이션의 &quot;하위 개체&quot; 모드와 마찬가지로, 클릭한 하나에 연결된 모든 다각형을 채웁니다.
* **![](../../assets/image2020-9-30-11-32-54.png)UV 청크 채우기** - 전체 UV 청크 또는 &quot;섬&quot;을 채웁니다. 메시 채우기와 비슷하게 작동하지만 UV 공간에서 연결된 다각형을 보면 작동합니다. UV 테두리에서 채우기가 중지됩니다.

![](../../assets/polygon-fill.gif)

이러한 4가지 모드를 결합 및 전환할 수 있습니다. 즉, 일부 스마트 사용을 통해 메시 및 UV 청크 모드를 사용하여 마스크에서 섹션을 빠르게 표시하고 표시 해제할 수 있습니다.

[다각형 채우기] 도구와 연결된 (기본) 핫키는 다음과 같습니다.

* *숫자 키 4* - 다각형 채우기 도구를 선택합니다.
* *X* - 마스크를 칠할 때 현재 색상을 반전합니다. 검은색과 흰색이 빠르게 바뀝니다. 재질 페인팅 모드에서 이 핫키는 영향을 주지 않습니다.
