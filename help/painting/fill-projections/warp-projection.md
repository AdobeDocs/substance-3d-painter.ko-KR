---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/painting/fill-projections/warp-projection.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 뒤틀기 투영을 사용하여 창의적인 텍스처 페인팅을 위해 왜곡 효과와 함께 텍스처를 투영합니다.
helpx_creative_field: ""
helpx_description: Painter > Painting > Fill projections > Warp projection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 뒤틀기 투영
user-guide-description: ''
user-guide-title: ''
source-git-commit: 5ab9709e1630071fddf0db0f03a292e92b84b31f
workflow-type: tm+mt
source-wordcount: '1859'
ht-degree: 2%

---


# 뒤틀기 투영

![](../../assets/proj-warp.jpg)

채우기의 뒤틀기 투영은 3D 투영으로, 그리드의 점을 편집하여 텍스처를 변형할 수 있습니다. 비평면 표면에 패턴 및 로고를 맞추는 데 사용할 수 있습니다.

## 빠른 설정

[에셋 창](../../interface/assets/assets.md)에서 메시로 리소스를 끌어서 놓아 뒤틀기 투영이 있는 레이어를 빠르게 설정할 수 있습니다. 마우스를 놓으면 리소스를 할당할 채널을 선택할 수 있는 메뉴가 열립니다.

호환되는 리소스 유형은 다음과 같습니다.

* **Alpha**
* **절차**
* **텍스처**
* **재질**(Alt 키를 눌러야 함)

![](../../assets/drop-viewport-warp.gif)

## 속성

| 설정 | 설명 |
| --- | --- |
| **필터링** | 텍스처 또는 재질을 필터링하는 방법을 제어합니다. 이 설정은 텍스처가 여러 번 반복될 때 나타나는 모양에 영향을 줄 수 있습니다. 기본값과 다른 필터링을 사용하여 높은 비율 값을 지정하면 더 나은 결과를 얻을 수 있습니다. 현재 사용 가능한 설정:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>쌍선형 `\|` HQ</strong>(기본값): 타일링 값이 높을 때 텍스처의 품질을 개선하려는 고급 쌍선형 필터링입니다.</li><li data-preserve-html="true"><strong>쌍선형 `\|` 선명</strong>: 텍스처를 약간 매끄럽게 하지만 세부 사항을 유지하려는 간단한 쌍선형 필터링입니다.</li><li data-preserve-html="true"><strong>가장 가까운</strong>: 필터링이 없습니다. 쌍선형 필터링으로 인해 결과가 흐릿해지고 세부 사항이 세분화된 경우 유용합니다. 텍스처에 앨리어싱을 적용할 수 있습니다.</li></ul> |
| **UV 랩** | 투영 내에서 텍스처가 반복되는 방식을 제어합니다. 가능한 값은 다음과 같습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>없음</strong>: 텍스처가 반복되지 않습니다. 텍스처 외부의 모든 요소는 검정색/투명입니다.</li><li data-preserve-html="true"><strong>가로로 반복</strong>: 텍스처가 가로로만 반복됩니다.</li><li data-preserve-html="true"><strong>세로로 반복</strong>: 텍스처가 세로로만 반복됩니다.</li><li data-preserve-html="true"><strong>반복</strong>(기본값): 텍스처가 두 축 모두에서 반복됩니다.</li></ul> |
| **모양 자르기** | 투영된 텍스처가 투영 영역의 외부에 표시되어야 하는지 여부를 정의합니다. 가능한 값은 다음과 같습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>프로젝트가 모양으로 잘림</strong>: 프로젝트가 투영 영역 내에 제한되어 있습니다.</li><li data-preserve-html="true"><strong>투영이 모양 밖으로 확장됨</strong>(기본값): 투영이 투영 영역을 넘어 계속됩니다.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/warp-extend.jpg" width="500px"/></div> |
| **투영 깊이** | 투영이 Z축을 따라 얼마나 멀리 이동할지 제어합니다. 이 설정은 격자점이나 투영 평면이 너무 멀리 떨어져 있을 때 메시 표면에 도달하는 데 도움을 줍니다.녹색 화살표는 격자의 각 점에 대한 투영의 방향과 거리를 나타냅니다. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/warp-depth.gif"/></div> **경고:** 값이 높으면 성능에 심각한 영향을 줄 수 있습니다. 이 매개 변수는 가능한 한 낮게 유지하는 것이 좋습니다. |
| **깊이 컬링** | 거리에 따라 투영을 페이드 합니다. 다음과 같은 매개 변수를 사용할 수 있습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>경도</strong>: 페이드 전환이 얼마나 단단하거나 부드러운지 제어합니다.</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/warp-hardness.gif"/></div> |

### UV 변형

UV 변형 설정은 투영 내의 텍스처/재질을 제어합니다.

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 40.0%;"/> <col style="width: 20.0%;"/> <col style="width: 40.0%;"/> </colgroup><tbody><tr><th>크기 조절 모드</th><th>설정</th><th>설명</th></tr><tr><td><p><strong>타일링</strong>(기본값)<strong> <br/></strong></p><p>현재 텍스처의 반복 양을 수동으로 설정할 수 있습니다.</p></td><td><strong>타일링</strong></td><td>텍스처가 반복되는 횟수를 제어합니다.</td></tr><tr><td rowspan="2"><br/><br/></td><td colspan="1"><strong>회전</strong></td><td colspan="1">텍스처가 메시에 투영되는 각도를 제어합니다.</td></tr><tr><td colspan="1"><strong>오프셋</strong></td><td colspan="1">텍스처가 투영될 위치를 제어합니다. 기본값은 텍스처 중심이 메시 UV의 중심에 있음을 의미합니다.</td></tr><tr><th colspan="1"><br/></th><th colspan="1"><br/></th><th colspan="1"><br/></th></tr><tr><td rowspan="4"><p><strong>실제 크기</strong></p><p>메시 크기와 임베드된 물리적 크기에 따라 텍스처를 자동으로 조정합니다. 올바른 물리적 크기를 계산하기 위해 너비 및 길이(X 및 Y 측정)를 사용합니다. Z 측정은 고려되지 않습니다.</p><p>(자세한 내용은 전용 [설명서 페이지](https://experienceleague.adobe.com/ko/docs/substance-3d-painter/using/features/physical-size)를 참조하십시오.)</p></td><td><strong>사용자 정의 크기</strong></td><td><p>활성화되면 물리적 크기를 수동으로 입력하고 에셋에서 제공한 템플릿을 재정의할 수 있습니다.</p><p>감지된 물리적 크기가 없거나, 동일한 레이어/효과 내에 서로 다른 물리적 크기를 가진 여러 에셋이 사용된 경우 자동으로 선택됩니다.</p></td></tr><tr><td colspan="1"><strong>크기(cm)</strong></td><td colspan="1">포함된 물리적 크기는 센티미터로 표시됩니다. 다른 측정 단위를 사용하여 만든 메시 파일로 작업할 수 있습니다. 그러면 올바른 비율이 유지됩니다. 그러나 에셋 크기는 현재 센티미터로만 표시됩니다.</td></tr><tr><td colspan="1"><strong>회전</strong></td><td colspan="1">텍스처가 메시에 투영되는 각도를 제어합니다.</td></tr><tr><td colspan="1"><strong>오프셋</strong></td><td colspan="1"><p>텍스처가 투영될 위치를 제어합니다. 기본값은 텍스처 중심이 메시 UV의 중심에 있음을 의미합니다.</p></td></tr></tbody></table>

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
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-hide-manipulator.png" width="50px"/></div> | 조작기 표시/숨기기 | 이 옵션을 활성화하면 뷰포트에 조작자가 표시되고 제어되어 투영 변환 또는 격자 점을 편집할 수 있습니다. 비활성화하면 조작기와 격자가 모두 숨겨집니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-manipulator-settings.png" width="50px"/></div> | 매니퓰레이터 설정 | 이 메뉴에는 세 가지 설정이 있습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>조작기 크기</strong>: 뷰포트에서 조작기의 크기를 제어합니다.</li><li data-preserve-html="true"><strong>눈금 단계</strong>: 제약 조건을 사용하여 변환할 때 단계의 크기를 정의합니다.</li><li data-preserve-html="true"><strong>각도 단계</strong>: 제약 조건으로 회전할 때 단계의 각도를 정의합니다.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-warp-tools.png" width="50px"/></div> | 뒤틀기 버전 메뉴 | 이 메뉴에는 다섯 가지 작업이 있습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>뒤틀기 변형</strong>: 뒤틀기 변형을 편집합니다. 전체 격자 위치, 회전 및 크기를 조작할 수 있습니다.</li><li data-preserve-html="true"><strong>정점 편집</strong>: 뒤틀기 격자 점을 개별적으로(또는 그룹에서) 편집합니다.</li><li data-preserve-html="true"><strong>뒤틀기를 십자형으로 분할</strong>: 뒤틀기 분할 도구를 시작하여 가로와 세로 모두에 새 격자 분할을 삽입합니다.</li><li data-preserve-html="true"><strong>뒤틀기를 수평으로 분할</strong>: 뒤틀기 분할 도구를 시작하여 새 격자 분할을 수평으로 삽입합니다.</li><li data-preserve-html="true"><strong>뒤틀기를 수직으로 분할</strong>: 뒤틀기 분할 도구를 시작하여 새 격자 분할을 수직으로 삽입합니다.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-warp-setting.png" width="50px"/></div> | 뒤틀기 투영 설정 | 이 메뉴는 현재 뒤틀기 투영에만 영향을 주는 설정을 다시 그룹화합니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>행 및 열</strong>: 뒤틀기 격자의 분할 수를 지정합니다. 격자의 점을 수정하지 않은 경우에만 이 설정을 편집할 수 있습니다.</li><li data-preserve-html="true"><strong>핸들 크기</strong>: <strong>정점 편집</strong> 모드에서 격자 점의 크기를 정의합니다.</li><li data-preserve-html="true"><strong>격자 색상</strong>: 뒤틀기 격자 선의 색상을 정의합니다.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-lock-tangent.png" width="50px"/></div> | 자동 접선 | 활성화되면 접점을 이동할 때 접점을 인접 포인트로 자동으로 정렬합니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-translate.png" width="50px"/></div> | 병진 조작기 | 주 축(X, Y, Z)을 따라 투영 또는 격자점을 이동할 수 있습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-rotate.png" width="50px"/></div> | 회전 조작기 | 주 축(X, Y, Z)을 따라 투영이나 격자점을 회전할 수 있습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-scale.png" width="50px"/></div> | 비율 조작기 | 장면에서 주 축(X, Y, Z)을 따라 투영의 비율을 조정할 수 있습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r9-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-surface.png" width="50px"/></div> | 서피스 매니퓰레이터 | 3D 모델 표면에 투영 또는 격자점을 스냅하여 이동할 수 있습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r10-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-space.png" width="50px"/></div> | 매니퓰레이터 공간 | 변형이 수행되는 공간을 정의합니다. 가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>로컬 공간</strong>: 축이 현재 변환에 맞춰 정렬됩니다.</li><li data-preserve-html="true"><strong>월드 공간</strong>: 축이 장면에 정렬됩니다.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r11-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-x.png" width="50px"/></div> | X에 미러링 | X축의 변형 뒤집기 |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r12-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-y.png" width="50px"/></div> | Y에 미러링 | Y축의 변형을 뒤집습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r13-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-flip-z.png" width="50px"/></div> | Z에 미러링 | Z축에서 변형을 뒤집습니다. |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r14-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-warp-reset.png" width="50px"/></div> | 변환 재설정 | 이 메뉴에는 세 가지 작업이 있습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>전역 변형 복원</strong>: 프로젝션의 위치, 회전 및 비율을 다시 초기 값으로 다시 설정합니다. 이 작업은 격자 점 자체에는 영향을 주지 않습니다.</li><li data-preserve-html="true"><strong>모든 꼭짓점 재설정</strong>: 뒤틀기 격자의 격자 점의 모든 위치와 접선을 재설정합니다.</li><li data-preserve-html="true"><strong>선택한 정점을 다시 설정</strong>: 뒤틀기 격자의 선택한 점의 위치와 접선만 다시 설정합니다.</li></ul> |

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

## 격자선 포인트 편집

뒤틀기 투영은 평면과 점 격자로 표현됩니다. 3D 모델에 더 잘 맞도록 투영을 수정할 수 있지만 텍스처가 왜곡되도록 각 점을 수정할 수도 있습니다.

그리드 포인트를 편집하려면 컨텍스트 도구 모음에서 편집 모드를 **정점 편집**(으)로 전환합니다.

![](../../assets/edit-vertices.png)

>[!NOTE]
>
> 키보드 단축키를 사용하면 **변형 뒤틀기**&#x200B;와 **정점 편집** 사이를 빠르게 전환할 수 있습니다. [바로 가기](../../interface/settings/shortcuts.md) 페이지에서 **뒤틀기 편집 모드 전환**&#x200B;을 참조하세요.

### 점 선택

| 액션 | 설명 |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/grid-point-selection-single-click.gif" width="250px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">점을 한 번 클릭하면 선택됩니다.</li><li data-preserve-html="true">점 또는 조작기에서 다른 곳을 클릭하면 점이 선택 해제됩니다.</li><li data-preserve-html="true"><strong>SHIFT</strong>를 누른 상태에서 점을 클릭하면 여러 점을 선택할 수 있습니다.</li><li data-preserve-html="true"><strong>CTRL</strong>을 누른 상태에서 점을 클릭하면 이 점만 선택 해제되고 다른 점은 선택 해제되지 않습니다.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table3_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/grid-point-selection-rectangle.gif" width="250px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">클릭하고 드래그하면 사각형 선택이 가능합니다. 마우스를 놓으면 사각형 안의 모든 점이 선택됩니다.</li><li data-preserve-html="true"><strong>SHIFT</strong>를 누른 상태에서 클릭하고 드래그하면 현재 선택 영역에 점을 더 추가할 수 있습니다.</li><li data-preserve-html="true"><strong>CTRL</strong>을 누른 상태에서 클릭하고 드래그하면 현재 선택 영역에서 점을 제거할 수 있습니다.</li></ul> |

### 포인트 이동

| 액션 | 설명 |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table4_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/point-move.gif" width="250px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">점을 이동하려면 평행 이동 매니퓰레이터(Translation manipulator)를 사용합니다.</li><li data-preserve-html="true">서피스 매니퓰레이터를 사용하여 3D 모델 서피스에서 점을 이동합니다.</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table4_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/point-move-clickdrag.gif" width="250px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">점을 클릭하고 드래그하여 먼저 선택할 필요 없이 빠르게 이동합니다.</li><li data-preserve-html="true">점을 클릭하고 드래그하면 서피스 조작기처럼 이동합니다.</li><li data-preserve-html="true"><strong>CTRL</strong>을 누른 상태에서 점을 클릭하고 드래그하면 변환 조작기처럼 이동합니다(세 축의 카메라 공간에서).</li></ul> |

### 접선 조정

뒤틀기 투영 격자는 [베지어 패치](https://en.wikipedia.org/wiki/B%C3%A9zier_surface)이며, 각 점에 접점을 연결하는 선의 곡선을 제어하는 자체 접선 집합이 있음을 의미합니다. 접선을 조정하면 텍스처의 변형 방식을 보다 효과적으로 제어할 수 있습니다.

| 액션 | 설명 |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table5_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/tangent-rotate-scale.gif" width="250px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">빨간색으로 표시되는 점의 접선을 수정하려면 지정된 점을 선택한 다음 회전 또는 배율 매니퓰레이터를 사용하면 됩니다.</li></ul> |

>[!NOTE]
>
> 컨텍스트 도구 모음에서 **자동 접선** 설정을 활성화하면 점을 이동할 때 접선이 자동으로 재설정되고 조정됩니다.
> 
> ![](../../assets/warp-tangent-adjustment.gif)

### 포인트 수 증가 또는 감소

뒤틀기 그리드는 점의 수를 늘리고 텍스처를 변형하는 방법에 대한 더 많은 컨트롤을 제공하기 위해 세분화될 수 있다.

| 액션 | 설명 |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table6_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/warp-split.gif" width="300px"/></div> | <ul data-preserve-html="true"><li data-preserve-html="true">뒤틀기 설정 메뉴에서 격자를 행과 열로 나눕니다. (포인트가 이동되지 않은 경우에만 가능합니다.)</li><li data-preserve-html="true">세 개의 분할 도구 중 하나를 사용하여 격자를 세분화합니다.</li><li data-preserve-html="true"><strong>Esc</strong>를 눌러 분할 도구를 취소할 수 있습니다.</li></ul> |
