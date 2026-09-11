---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack.html"
breadcrumb-title: ''
description: Substance 3D Painter의 레이어 스택을 사용하여 여러 텍스처 페인팅 레이어를 구성하고 관리하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 레이어 스택
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 3%

---


# 레이어 스택

![](../../assets/layer-stack.png)

**레이어 스택**&#x200B;를 사용하면 텍스처 집합의 레이어를 조작할 수 있습니다. 레이어에는 장면의 3D 개체에 텍스처를 만들기 위한 페인팅과 효과가 포함되어 있습니다. 레이어를 숨기거나 숨기고, 폴더에 삽입하고, 불투명도와 혼합 모드를 변경할 수 있습니다.

자세한 내용은 다음 페이지를 참조하십시오.

* [레이어 만들기](creating-layers.md)
* [레이어 관리](managing-layers.md)
* [마스크 및 효과](masking-and-effects.md)
* [혼합 모드](blending-modes.md)
* [레이어 인스턴싱](layer-instancing.md)
* [모양 마스크](geometry-mask.md)

## 개요

레이어 스택에 특정 계층 구조의 레이어가 표시됩니다. 하단의 레이어가 먼저 메쉬에 그려지고 상단의 레이어가 그 뒤를 따릅니다. 따라서 스택 맨 위에 있는 레이어가 마지막 항목이고 맨 아래에 있는 레이어가 첫 번째 항목입니다. 같은 원칙이 폴더에 적용되지만 폴더의 내용은 우선 순위를 갖습니다. 즉, 폴더의 내용이 같은 레벨의 레이어보다 먼저 처리됩니다.

**일반적인 특성 :**

* 각 레이어는 **다중 채널**&#x200B;입니다.
* 재질 설정에 따라 페인트 도구에서 **모든 해당 채널에서** 페인트를 지정합니다(현재 레이어 스택에서 보고 있는 채널은 영향을 주지 않음).
* 각 레이어에는 채널당 **혼합 모드**&#x200B;와 **불투명도**&#x200B;가 있습니다(왼쪽 상단 드롭다운 메뉴를 통해 채널 간에 전환할 수 있음).

**레이어 유형 :**

* **레이어 페인팅** : 이 유형의 레이어는 브러시와 파티클로 페인트할 수 있습니다.
* **레이어 채우기** : 이 레이어는 페인팅할 수 없으며, 대신 채널을 채우기 위해 이 레이어에 재질을 로드할 수 있습니다. 변형 작업을 조작하여 재질을 반복할 수도 있습니다.
* **폴더** : 이 유형의 레이어는 다른 레이어를 포함할 목적으로만 사용되며, 주로 레이어 스택 구성에 사용됩니다

각 레이어에서 **마스크를 추가**&#x200B;할 수 있습니다. 이 마스크를 사용하면 현재 텍스처 집합의 채널 중 특정 부분에만 콘텐츠를 적용할 수 있습니다.\
마스크를 수동으로 페인트(브러시가 있는 회색 음영)하거나 필터와 재질을 사용하여 다이내믹/프로시저 결과를 얻을 수 있습니다.

## 보기 모드

![](../../assets/switch-viewmode-optim.gif)

레이어 스택의 왼쪽 상단 드롭다운은 레이어 스택의 보기 모드를 제어합니다. 레이어는 여러 채널을 다룰 수 있으므로 이러한 속성을 한 번에 모두 표시할 수는 없습니다. 따라서 뷰 모드는 현재 디스플레이 컨텍스트를 정의하는 데 사용할 수 있습니다. 이 드롭다운을 사용할 때 레이어 축소판에 표시할 채널을 지정할 수 있고 이 채널의 혼합 모드와 불투명도만 제어할 수 있습니다.

이 드롭다운의 목록은 [텍스처 집합 설정](../texture-set/texture-set-settings.md)에서 사용할 수 있는 채널 목록을 기반으로 합니다.

## 액션

![](../../assets/image2020-9-30-12-2-13.png)

아이콘의 오른쪽 위 목록은 레이어 스택에서 수행할 수 있는 일반적인 작업 입니다.

| 액션 | 설명 |
| --- | --- |
| 효과 추가 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-effect.png"/></div> | 새 효과를 만들고 현재 선택한 레이어에 추가합니다. 효과에 대한 자세한 내용은[전용 페이지](../../features/effects/effects.md)를 참조하세요. |
| 마스크 만들기 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-mask.png"/></div> | 다음 항목이 포함된 마스크 작업 메뉴를 엽니다 .<ul data-preserve-html="true"><li data-preserve-html="true">흰색 마스크 추가</li><li data-preserve-html="true">검정 마스크 추가</li><li data-preserve-html="true">비트맵 마스크 추가</li><li data-preserve-html="true">색상 선택 항목과 함께 마스크 추가</li><li data-preserve-html="true">높이 조합이 있는 마스크 추가</li></ul> |
| 새 레이어 페인팅 만들기 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-11-52-41.png"/></div> | 현재 선택된 레이어 페인팅 위에 새 그룹을 만듭니다. |
| 새 칠 레이어 만들기 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-12-0-49.png"/></div> | 현재 선택한 레이어 위에 새 [칠 레이어](../../painting/fill-projections/fill-projections.md)를 만듭니다. |
| 새 스마트 재질 추가 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-smartmat.png"/></div> | 현재 선택된 레이어 위에 새 스마트 재질을 삽입합니다.이 단추를 클릭하면 미니 선반이 열려 현재 [에셋](../../interface/assets/assets.md)에서 사용할 수 있는 스마트 재질 목록을 검색할 수 있습니다. |
| 새 폴더 추가 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/image2020-9-30-12-1-13.png"/></div> | 현재 선택된 레이어 위에 새 빈 폴더를 만듭니다. |
| 레이어 삭제 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-trash.png"/></div> | 현재 선택한 항목(레이어, 폴더 또는 효과)을 삭제합니다. |
