---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/interface/layer-stack/geometry-mask.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 지오메트리 마스크를 사용하여 메시 지오메트리 및 표면 속성을 기반으로 레이어를 마스킹하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Geometry mask
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 모양 마스크
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 1%

---


# 모양 마스크

![](../../assets/geometry-mask.png)\
지오메트리 마스크는 연관된 텍스처 세트의 3D 모델 지오메트리를 기반으로 레이어를 마스킹할 수 있는 레이어의 보조 마스크입니다. 메시 이름이나 UV 타일 기준으로 마스킹할 수 있습니다.

## 개요

지오메트리 마스크는 레이어가 포함/제외 목록을 통해 3D 모델의 어느 부분에 적용되어야 하는지 지정하는 방식으로 작동합니다.

[모양] 마스크는 3D 모델 모양의 큰 부분을 빠르게 버릴 수 있는 유용한 도구입니다. 페인트 마스크에는 다음과 같은 여러 가지 이점이 있습니다.

* 일반적으로 뷰포트 선택 모드를 사용하여 설정하고 사용하는 것이 더 빠릅니다.
* 텍스처 생성 시 기하학을 완전히 버릴 수 있어 더 나은 성능을 제공합니다.
* 비파괴적이며 다시 가져온 후 3D 모델이 변경되면 업데이트됩니다.
* 마스크된 형상 아래에 있는 형상을 페인트 하여 숨겨진 부품을 페인트 할 수 있습니다.
* 페인트 마스크와 마찬가지로 지오메트리 마스크를 그룹에 적용하여 한 번에 여러 레이어에 적용할 수 있습니다.

### 아이콘 상태

모양 마스크 아이콘은 상태를 다음과 같이 나타낼 수 있습니다.

| 아이콘 | 설명 |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-default.png"/></div> | 형상이 제외되지 않았으며 레이어는 연관된 텍스처 세트의 전체 메쉬에 적용됩니다. 이는 새 레이어 또는 폴더의 기본 상태입니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-selection.png"/></div> | 하나 이상의 메시 이름이 제외되었습니다. 번호는 아직 레이어의 영향을 받는 나머지 요소의 양을 나타냅니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-uvtiles.png"/></div> | 하나 이상의 UV 타일이 제외되었습니다. 번호는 아직 레이어의 영향을 받는 나머지 요소의 양을 나타냅니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-mask-icon-empty.png"/></div> | 포함된 메시 이름은 없으며 레이어는 실제 효과를 나타내지 않습니다. |

## 도형 마스크 편집

지정된 레이어의 지오메트리 마스크를 수정하려면 전용 아이콘을 클릭하면 됩니다. 편집 모드를 종료하려면 레이어의 다른 부분(내용 또는 페인트 마스크)을 클릭하면 됩니다.

![](../../assets/geo-mask-editing.gif)

### 마스크 유형

모양 마스크는 다음 두 가지 유형의 마스크를 지원합니다.

| 유형 | 설명 |
| --- | --- |
| **UV 타일** | 마스크는 포함할 UV 타일(UDIM) 번호를 지정하여 수행합니다. 이 방법은 계산에서 텍스처를 완전히 삭제하는 데 사용할 수 있는 가장 강력한 방법입니다. |
| **메시 이름** | 마스크는 3D 모델에 포함해야 하는 하위 메시를 지정하여 수행됩니다. 형상은 메시 이름별로 그룹화됩니다. |

### 레이어 스택 액션

![](../../assets/geo-mask-actions.png)

아이콘을 마우스 오른쪽 버튼으로 클릭하면 레이어 스택에서 직접 모양 마스크 상태를 빠르게 수정할 수 있습니다.

다음과 같은 동작을 제공합니다.

| 액션 | 설명 |
| --- | --- |
| **모양 마스크 복사** | 지정된 레이어의 지오메트리 마스크 유형 및 선택 항목을 복사합니다. |
| **모양 마스크에 붙여넣습니다.** | 이전에 복사한 지오메트리 마스크 속성을 붙여넣습니다. |
| **모두 포함** | 지정된 마스크의 모든 요소를 선택된 것으로 표시합니다. |
| **모두 제외** | 지정된 마스크의 모든 요소를 선택 해제된 것으로 표시합니다. |

## 마스킹된 기하학을 통해 페인팅

형상의 일부가 제외된 경우 뷰포트에서 숨길 수 있습니다. 이렇게 하면 이전에 아래에 있었으며 액세스할 수 없었던 도형을 페인트 할 수 있습니다.

제외된 형상을 숨기려면 상황별 도구 모음의 뷰포트 상단에 있는 버튼을 사용합니다.

![](../../assets/hide-excluded-geo-button.png)

아래 예에서는 3D 모델이 두 개의 개체(위 및 아래 부분)로 분할되었습니다. 기본적으로 브러시 획은 모든 오브젝트와 충돌합니다. 윗부분을 제외함으로써 이제 아랫부분에만 배타적으로 페인팅할 수 있다.

>[!NOTE]
>
> 형상 마스크 포함/제외 목록은 동적이며, 그 상태를 변경하면 레이어에서 브러시 획을 새로 계산합니다. 이렇게 하면 새 UV 타일이 있는 메시를 다시 가져오거나 메시 이름이 변경된 경우 브러시 획을 잃지 않고 마스크를 조정할 수 있습니다. 그러나 브러시 획이 적용되지 않았으므로 모양 마스크를 변경하면 이후에 잘못된 브러시 투영이 발생할 수 있습니다.

| 시각적 | 설명 |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/no-geo-excluded.jpg" width="420px"/></div> | 지오메트리 마스크에서 제외된 지오메트리가 없습니다. 흰색 브러시 획이 수행된 레이어 페인팅이 모든 지오메트리를 충돌합니다.**제외된 도형 숨기기** 단추를 사용할 수 없습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-excluded-hidden.jpg" width="420px"/></div> | 형상 마스크에서 위쪽 부분이 제외되고 흰색 브러시 획이 형상의 아래쪽 부분에만 충돌합니다.**제외된 도형 숨기기** 단추를 사용할 수 있습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/geo-excluded-visible.jpg" width="420px"/></div> | 형상 마스크에서 위쪽 부분이 제외되고 흰색 브러시 획이 형상의 아래쪽 부분에만 충돌합니다.**제외된 도형 숨기기** 단추를 사용할 수 없습니다. |
