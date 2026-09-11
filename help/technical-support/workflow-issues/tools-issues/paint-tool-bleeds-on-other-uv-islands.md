---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/workflow-issues/tools-issues/paint-tool-bleeds-on-other-uv-islands.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 UV 섬 간 페인트 도구 번짐을 해결하여 텍스처 경계를 깔끔하게 유지하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Paint Tool bleeds on other UV islands
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 페인트 도구가 다른 UV 섬에서 재단 물림
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '126'
ht-degree: 0%

---


# 페인트 도구가 다른 UV 섬에서 재단 물림

[페인트 도구](../../../features/effects/paint.md)의 일부 기본 동작은 일부 특정 상황에서 반직관적으로 보일 수 있습니다. Substance 3D Painter은 주로 3D 공간에서 작동하는 애플리케이션입니다. 이것은 페인팅에도 적용됩니다. 페인트 브러시의 기본 설정은 페인팅 시 UV 전체에 걸쳐 매끄럽도록 시도하는 것입니다. 2D 보기와 상호 작용할 때 예상하지 못한 결과가 나올 수 있는 이유다.

2D 보기에서 페인팅할 때 다른 UV 섬이 번지지 않도록 하려면 도구 매개 변수에서 **정렬** 설정을 변경하기만 하면 됩니다.

| *정렬 모드* | *미리 보기* |
| --- | --- |
| **접선 줄 바꿈** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-tangent-optim.gif"/></div> |
| **UV** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../../assets/paint-mode-uv.gif" width="450px"/></div> |
