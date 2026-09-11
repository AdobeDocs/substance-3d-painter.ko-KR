---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/shelf-issues/thumbnails-in-the-shelf-look-incorrect.html"
breadcrumb-title: ''
description: 리소스 미리 보기를 정확하게 하기 위해 Substance 3D Painter 선반에 표시되는 썸네일이 잘못 표시되는 문제를 해결하는 방법에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Shelf Issues > Thumbnails in the shelf look incorrect
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 선반의 축소판이 잘못 표시됨
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---


# 선반의 축소판이 잘못 표시됨

셸프의 축소판이 상습적인 것과 다른 것으로 나타나는 이유는 미리 보기를 렌더링하는 데 사용되는 셰이더 때문일 수 있습니다.

| 깨진 축소판 | 표준 축소판 |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/shelf-broken-preview.png"/></div> | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/shelf-normal-preview.png" width="300px"/></div> |

## 1 - 기본 설정 창 열기

**편집**&#x200B;으로 이동하고 **설정** :

![](../../../assets/pref-menu.png)

## 2 - 셸프 미리 보기 셰이더 제거

**일반** 보기에서 &quot;미리 보기 옵션&quot; 섹션이 표시될 때까지 아래로 스크롤합니다.\
&quot; **재질 미리 보기 셰이더**&quot; 앞에 있는 **십자** 단추를 클릭하여 지정한 현재 셰이더를 제거합니다.

![](../../../assets/remove-preview-shader.png){width="450px"}

## 3 - Substance 3D Painter 다시 시작

축소판이 올바르게 표시되도록 다시 생성하려면 Substance 3D Painter을 다시 시작해야 합니다.
