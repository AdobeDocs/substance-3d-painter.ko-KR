---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/fill-projections/spherical-projection.html"
breadcrumb-title: ''
description: Substance 3D Painter의 구형 투영을 사용하여 구의 텍스처를 투영하여 오브젝트를 중심으로 텍스처를 감쌀 수 있습니다.
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > Spherical projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 구형 투영
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 2%

---


# 구형 투영

![](../../assets/spherical-proj.jpg)

칠 구형 투영을 사용하면 개체 주위에 이미지와 패턴을 투영할 수 있습니다. 둥근 오브젝트에 투영하거나 텍스처를 원형 패턴으로 왜곡하는 것이 유용할 수 있습니다.

## 속성

| 설정 | 설명 |
| --- | --- |
| **필터링** | 텍스처 또는 재질을 필터링하는 방법을 제어합니다. 이 설정은 텍스처가 여러 번 반복될 때 나타나는 모양에 영향을 줄 수 있습니다. 기본값과 다른 필터링을 사용하여 높은 비율 값을 지정하면 더 나은 결과를 얻을 수 있습니다. 현재 사용 가능한 설정:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>쌍선형 | HQ</strong>(기본값): 타일링 값이 높을 때 텍스처의 품질을 개선하려는 고급 쌍선형 필터링.</li><li data-preserve-html="true"><strong>쌍선형 | 날카로운</strong>: 텍스처를 약간 매끄럽게 하지만 세부 사항을 유지하려는 간단한 쌍선형 필터링.</li><li data-preserve-html="true"><strong>가장 가까운</strong>: 필터링이 없습니다. 쌍선형 필터링으로 인해 결과가 흐릿해지고 세부 사항이 세분화된 경우 유용합니다. 텍스처에 앨리어싱을 적용할 수 있습니다.</li></ul> |
| **UV 랩** | 투영 내에서 텍스처가 반복되는 방식을 제어합니다. 가능한 값은 다음과 같습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>없음</strong>: 텍스처가 반복되지 않습니다. 텍스처 외부의 모든 요소는 검정색/투명입니다.</li><li data-preserve-html="true"><strong>가로로 반복</strong>: 텍스처가 가로로만 반복됩니다.</li><li data-preserve-html="true"><strong>세로로 반복</strong>: 텍스처가 세로로만 반복됩니다.</li><li data-preserve-html="true"><strong>반복</strong>(기본값): 텍스처가 두 축 모두에서 반복됩니다.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/spherical-repeat.jpg" width="500px"/></div> |
| **모양 자르기** | 투영된 텍스처가 투영 영역의 외부에 표시되어야 하는지 여부를 정의합니다. 가능한 값은 다음과 같습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>프로젝트가 모양으로 잘림</strong>: 프로젝트가 투영 영역 내에 제한되어 있습니다.</li><li data-preserve-html="true"><strong>투영이 모양 밖으로 확장됨</strong>(기본값): 투영이 투영 영역을 넘어 계속됩니다.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/spherical-shape-crop.jpg" width="500px"/></div> |

### UV 변형

UV 변형 설정은 투영 내의 텍스처를 제어합니다.

| *설정* | *설명* |
| --- | --- |
| **크기 조절** | 투영 내에서 텍스처가 반복될 횟수를 정의합니다. |
| **회전** | 투영에 적용된 텍스처의 각도를 제어합니다. |
| **오프셋** | 투영되는 텍스처의 원점을 제어합니다. 기본값은 텍스처가 투영 중간에 있음을 의미합니다. |

### 3D 투영 설정

3D 투영 설정은 3D 공간에서 투영 변환을 제어합니다.

| 설정 | 설명 |
| --- | --- |
| **오프셋** | 3D 공간에서 투영 원점의 위치입니다. 단위는 전체 장면의 테두리 상자를 기반으로 합니다. 0이 이 상자의 중심입니다. |
| **회전** | 각 축의 전체 투영을 회전하는 각도(도)입니다. |
| **크기 조절** | 각 축에 있는 전체 투영의 크기입니다. |

## 상황별 도구 모음

뷰포트 맨 위에 있는 [상황별 도구 모음](../../interface/toolbars.md)에서 조작기와 프로젝션을 제어할 수 있는 몇 가지 설정과 도구를 사용할 수 있습니다.

| 아이콘 | 이름 | 설명 |
| --- | --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_image" src="../../assets/icon-hide-manipulator.png" width="50px"/></div> | 조작기 표시/숨기기 | 이 옵션을 활성화하면 매니퓰레이터가 뷰포트에 표시되고 제어할 수 있습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_image" src="../../assets/icon-manipulator-settings.png" width="50px"/></div> | 매니퓰레이터 설정 | 이 메뉴에는 세 가지 설정이 있습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>조작기 크기</strong>: 뷰포트에서 조작기의 크기를 제어합니다.</li><li data-preserve-html="true"><strong>눈금 단계</strong>: 제약 조건을 사용하여 변환할 때 단계의 크기를 정의합니다.</li><li data-preserve-html="true"><strong>각도 단계</strong>: 제약 조건으로 회전할 때 단계의 각도를 정의합니다.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-translate.png" width="50px"/></div> | 병진 조작기 | 장면에서 주 축(X, Y, Z)을 따라 투영을 이동할 수 있습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-rotate.png" width="50px"/></div> | 회전 조작기 | 장면에서 주 축(X, Y, Z)을 따라 투영을 회전시킬 수 있습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-scale.png" width="50px"/></div> | 비율 조작기 | 장면에서 주 축(X, Y, Z)을 따라 투영의 비율을 조정할 수 있습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-surface.png" width="50px"/></div> | 서피스 매니퓰레이터 | 3D 모델 표면에 투영을 스냅하여 이동할 수 있습니다.  **참고:** 이 조작기는 평면 및 뒤틀기 투영 유형에서만 사용할 수 있습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-space.png" width="50px"/></div> | 매니퓰레이터 공간 | 변환을 수행할 공간을 정의합니다. 가능한 값은 다음과 같습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>로컬 공간</strong>: 축이 현재 변환에 맞춰 정렬됩니다.</li><li data-preserve-html="true"><strong>월드 공간</strong>: 축이 장면에 정렬됩니다.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-x.png" width="50px"/></div> | X에 미러링 | X축의 변형 뒤집기 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r9-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-y.png" width="50px"/></div> | Y에 미러링 | Y축의 변형을 뒤집습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r10-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-z.png" width="50px"/></div> | Z에 미러링 | Z축에서 변형을 뒤집습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r11-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-reset.png" width="50px"/></div> | 변환 재설정 | 투영 변환을 다시 기본 상태로 복원합니다. |

## 조작자

이 투영 조작기는 [3D 뷰포트](../../interface/viewport/3d-view.md)에서만 사용할 수 있습니다.

| 액션 | 단축키 | 설명 |
| --- | --- | --- |
| **번역** | 마우스 클릭 | 변환 매니퓰레이터에서 축을 클릭하면 투영이 이동합니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>한 축</strong>: 투영의 한 방향으로만 이동합니다.</li><li data-preserve-html="true"><strong>두 축</strong>: 축을 기준으로 정렬된 평면에서 투영을 이동합니다.</li><li data-preserve-html="true"><strong>세 축</strong>: 카메라 공간에서 투영을 이동합니다(마주보는 평면).</li></ul>   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-translate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/3d-translate-2axes.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r1-column-c2_dynamic_grid_items_grid-cell2_position-par_image" src="../../assets/3d-translate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **번역 제한됨** | SHIFT+마우스 클릭 | 변환 매니퓰레이터를 사용하여 선택한 축을 따라 특정 간격(스테핑)으로만 투영을 이동합니다. 간격 크기는 조작기 설정을 통해 정의됩니다. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r2-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-translate-step.gif" width="200px"/></div> |
| **회전** | 마우스 클릭 | 회전 매니퓰레이터로 한 축을 클릭하면 투영이 회전합니다. 축 사이를 클릭하여 모든 축을 동시에 회전할 수 있습니다.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-rotate.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r3-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/3d-rotate-3axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **회전 제한됨** | SHIFT+마우스 클릭 | 회전 조작기를 사용하면 한 축을 클릭하여 투영을 회전하면 특정 간격에만 투영이 발생합니다. 단계는 조작기 설정을 통해 각도로 정의됩니다. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r4-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/3d-rotate-step.gif" width="200px"/></div> |
| **크기 조절** | 마우스 클릭 | 배율 매니퓰레이터를 사용하여 한 축 핸들을 클릭하면 주어진 축을 따라 투영 크기가 조정됩니다.   <table> <tr style="border: 0;"> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-one-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell1_position-par_image" src="../../assets/scale-two-axis.gif" width="200px"/></div>  </td> <td style="border: 0;" valign="top">  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r5-column-c2_dynamic_grid_items_grid-cell2_position-par_image" src="../../assets/scale-3-axes.gif" width="200px"/></div>  </td> </tr> </table> |
| **크기 조절** | SHIFT+마우스 클릭 | 배율 매니퓰레이터로 단축키를 유지하면서 한 축 핸들을 클릭하면 투영의 크기를 단계적으로 조정할 수 있습니다. 단계 크기는 변환 조작기와 동일합니다. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r6-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-1-axis-constrained.gif" width="200px"/></div> |
| **표면** | 마우스 클릭 | 서피스 매니퓰레이터를 사용하여 3D 모델 위로 클릭하고 드래그하면 서피스에서 스냅됩니다. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table2_row-r7-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/surface.gif" width="200px"/></div> **참고:** 이 조작기는 **평면** 및 **뒤틀기** 투영 유형에서만 사용할 수 있습니다. |
