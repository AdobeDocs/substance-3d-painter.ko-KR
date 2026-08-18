---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/interface/viewport/2d-view.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 2D 보기를 사용하여 UV 공간에서 텍스처를 보고 편집하여 정밀한 텍스처 페인팅을 수행하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Interface > Viewport > 2D view
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 2D 보기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# 2D 보기

![](../../assets/2d-view.jpg){width="450px"}

2D 보기는 현재 선택한 [텍스처 집합](../texture-set/texture-set.md)에서 메시 UV 섬을 표시합니다. 이 도구를 사용하면 레이어 스택의 텍스처를 볼 수 있을 뿐만 아니라 메시 UV 섬에 페인팅할 수 있습니다.

## 표시 모드

![](../../assets/display-mode-1.png)

뷰포트의 오른쪽 상단에 디스플레이 모드 드롭다운이 있습니다. 이 컨트롤을 사용하면 뷰포트에 표시할 정보를 변경할 수 있습니다. 단일 채널, 메시 맵 또는 최종 재질 결과를 조명과 함께 표시할 수 있습니다.

## 축 정보

![](../../assets/2d-axis.png)

뷰포트의 오른쪽 하단에는 2차원 축의 방향을 나타내는 **축 정보**&#x200B;가 있습니다. 이 경우 2D 보기의 축은 U와 V입니다.

## UV 타일 정보

![](../../assets/2d-view-button.png)

**표시 모드** 옆에는 UV 타일과 관련된 정보를 표시하거나 숨길 수 있는 **UV 타일 정보** 단추가 있습니다. 이 단추는 일반 프로젝트에 표시되지 않습니다.

## 프로젝트 워크플로우

프로젝트를 만들 때 정의된 워크플로우에 따라 2D 보기의 모양과 동작이 달라질 수 있습니다.

| *프로젝트 워크플로* | *동작* |
| --- | --- |
| **일반 프로젝트** | 일반 프로젝트에서는 UV 범위 [0-1]의 UV만 페인트할 수 있습니다. 이 범위를 벗어나는 모든 항목은 표시되지만 대화형으로 표시되지 않습니다.이 예제에서는 왼쪽의 UV 섬만 밝은 회색 배경 뒤에 페인트할 수 있습니다. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-regular.jpg" width="500px"/></div> |
| **UV 타일 프로젝트** | UV 타일 프로젝트를 사용하면 각 UV 범위가 페인트 칠할 수 있는 새로운 텍스처 세트입니다. 2D 보기는 각 타일이 구성되는 방식을 더 잘 볼 수 있도록 격자를 표시합니다. 각 타일에는 UDIM 번호가 할당됩니다. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/2d-view-range-uvtiles.jpg" width="500px"/></div> |
