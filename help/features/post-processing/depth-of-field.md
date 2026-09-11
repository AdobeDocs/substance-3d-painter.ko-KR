---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/depth-of-field.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 필드 후처리 깊이를 사용하여 사실적인 카메라 초점 흐림 효과를 만드는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Depth of Field
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 필드 깊이
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '132'
ht-degree: 0%

---


# 필드 깊이

![](../../assets/dof-example.jpg)![](../../assets/dof.png)

**DOF(필드 깊이**)에 직접 매개 변수가 없습니다. 활성화되면 **Ray**&#x200B;의 DOF가 **재정의**&#x200B;됩니다.

뷰포트에서 DOF의 모양을 제어하기 위해 카메라를 통해 두 가지 설정을 사용할 수 있습니다.

| *설정* | *설명* |
| --- | --- |
| **초점 거리** | 포커스점이 있는 거리를 정의합니다.  이 점은 [필드] 효과의 깊이에 사용됩니다. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/focus-distance-optim.gif"/></div> **참고:** 포커스 거리는 단축키 **CTRL + 마우스 가운데 단추**&#x200B;로 메시 지점을 클릭하여 자동으로 설정할 수 있습니다. |
| **조리개** | 필드 깊이 범위를 정의합니다. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/dof-aperture-optim.gif"/></div> **참고:** Iray가 이 매개 변수를 제어하는 경우 매개 변수를 변경하면 계산을 다시 트리거합니다. |
