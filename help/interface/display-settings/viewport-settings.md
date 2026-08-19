---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/interface/display-settings/viewport-settings.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 뷰포트 설정을 구성하여 디스플레이 옵션 및 렌더링 품질을 사용자 정의하는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Viewport settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 뷰포트 설정
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 2%

---


# 뷰포트 설정

**표시 설정**&#x200B;의 이 섹션은 텍스처 필터링 및 메시 와이어프레임과 같이 뷰포트의 표시와 관련된 다양한 설정을 제어합니다.

## 텍스처 필터링

![](../../assets/texture-filtering.png)

Anisotropic Filtering 및 MipMap Bias를 사용하면 뷰포트에서 텍스처의 표시를 제어할 수 있습니다. 이러한 설정은 텍스처에 직접 영향을 주지 않으며 내보내기 시에 적용되지 않으며 뷰포트에서 렌더링 프로세스를 다듬기만 합니다. [MipMap 바이어스] 설정을 사용하면 멀리 있거나 비스듬한 각도의 픽셀에 매우 날카로운 텍스처를 강제로 사용할 수 있지만, 경우에 따라 모아레 패턴 또는 지터링을 만들 수 있습니다.

기본 설정은 품질과 성능의 절충안이며 필요한 경우에만 변경해야 합니다.

| *설정* | *설명* |
| --- | --- |
| **비등방성 필터링** | 비등방성 필터링은 비스듬한 각도에서 볼 때 텍스처 품질을 향상시킵니다. 고품질 값은 더 나은 필터링을 제공하지만 성능을 저하시킬 수 있습니다. 이 설정은 필터링에 사용되는 픽셀당 샘플(spp) 양을 제어합니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>사용 안 함</strong>: 필터링 없음</li><li data-preserve-html="true"><strong>낮음</strong>(2spp)</li><li data-preserve-html="true"><strong>중간</strong>(4spp) : 기본값</li><li data-preserve-html="true"><strong>높음</strong>(8spp)</li><li data-preserve-html="true"><strong>매우 높음</strong>(16spp)</li></ul> <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/quality-anisotropic-filtering.jpg"/></div> |
| **MipMap 편향** | 디테일의 밉맵 레벨을 오프셋하여 텍스처 품질을 개선합니다. 값을 선명하게 하면 성능이 떨어지고 들쭉날쭉한 텍스처가 생길 수 있습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>0 - 소프트</strong>(경량 성능) : 기본값</li><li data-preserve-html="true"><strong>1 - 중간 소프트</strong></li><li data-preserve-html="true"><strong>2 - 선명</strong></li><li data-preserve-html="true"><strong>3 - 매우 날카로움</strong>(집약적 성능)</li></ul>(0~3) |

## 카메라 프레임

![](../../assets/camera-frame.png)

카메라 관리에 대한 자세한 내용은 [카메라 관리](../viewport/camera-management.md)를 참조하세요.

## 도구 표시

![](../../assets/viewport-tool.png)

| *설정* | *설명* |
| --- | --- |
| **페인팅 시 스텐실 숨기기** | 스텐실을 사용할 때(페인트 도구 속성 참조) 이 설정을 사용하면 메시에 페인팅할 때 일시적으로 숨길 수 있습니다. |
| **스텐실 표시 불투명도** | 페인팅하지 않을 때 뷰포트 렌더링에 대한 스텐실의 가시성을 제어합니다. |
| **프로젝션 미리 보기 채널** | 투영 도구를 사용할 때 표시할 재질의 채널을 제어합니다. |

## 메시 와이어프레임

![](../../assets/viewport-mesh.png)

| *설정* | *설명* |
| --- | --- |
| **메시 와이어프레임 표시** | 뷰포트에 망 와이어프레임 표시를 활성화하거나 비활성화합니다. |
| **와이어프레임 색상** | 망 와이어프레임 그리기에 사용되는 색상을 제어합니다. |
| **와이어프레임 불투명도** | 메시 위에 그릴 때 와이어프레임이 표시되는 정도를 제어합니다. |

## 채널 표시

![](../../assets/viewport-channel.png)

>[!NOTE]
>
> 채널 표시 설정은 **단일 채널** 보기 모드를 사용하는 경우에만 사용할 수 있습니다.

| *설정* | *설명* |
| --- | --- |
| **조명 없이 단독 보기 표시(비발광)** | 단일 채널 모드에서 보는 경우 이 설정을 사용하면 조명이 제거되고 채널이 단색으로 표시됩니다. 비활성화하면 메쉬의 테두리에 그림자가 적용됩니다. |
| **HDR 값 크기 조정** | 단일 채널 모드에서 **HDR** 텍스처(예: Height)를 볼 때 이 설정은 총 값의 비율을 조정합니다. 1보다 크거나 -1보다 작은 값을 볼 때 유용합니다. 결과는 **채널 비율**&#x200B;과 같습니다.아래 예에서 Height 채널은 최대 3의 값을 가집니다. 그러나 기본적으로 배율 값을 변경하지 않으면 이 값을 볼 수 없습니다 . <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/scale-hdr.jpg"/></div> |
| **HDR 값에 +/- 색상 사용** | 이 설정을 사용하면 양수 값을 제1 색상으로, 음수 값을 제2 색상으로 대체하여 보다 쉽게 HDR 텍스처를 볼 수 있습니다. 중간 값(0)은 검정색입니다.예 : <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/colored-hdr.jpg"/></div> |
| **색상 채널** | 뷰포트 보기 모드를 수정하여 현재 채널의 R, G, B 또는 Alpha 구성 요소만 개별적으로 표시합니다. 재질 디스플레이 모드에서는 이 설정을 사용할 수 없습니다. 이 옵션을 활성화하면 선택한 색상 채널의 이름이 뷰포트에 표시됩니다.  <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table1_row-r4-column-c1_image" src="../../assets/color-channel.png"/></div>  가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>RGBA</strong>(기본값): 색상 채널에서 투명도로 모든 구성 요소를 표시합니다.</li><li data-preserve-html="true"><strong>회색 음영+Alpha</strong>(기본값): 회색 음영 채널에서 투명도로 회색 음영 값을 표시합니다.</li><li data-preserve-html="true"><strong>R</strong>: 색상 채널에서 빨간색 구성 요소만 표시합니다.</li><li data-preserve-html="true"><strong>G</strong>: 색상 채널에서 녹색 구성 요소만 표시합니다.</li><li data-preserve-html="true"><strong>B</strong>: 색상 채널에서 파랑 구성 요소만 표시합니다.</li><li data-preserve-html="true"><strong>Alpha</strong>: 모든 채널에서 텍스처의 투명도만 표시합니다.</li></ul> |

## 격자

![](../../assets/display-settings-grid.png)

격자 설정을 사용하면 3D 뷰포트 내부에 3D 격자의 드로잉을 표시하고 제어할 수 있습니다.

격자 구분은 현재 카메라 수준의 확대/축소 및 각도에 따라 자동으로 이루어집니다. 현재 격자 단위는 뷰포트의 왼쪽 하단에 표시됩니다.

| 설정 | 설명 |
| --- | --- |
| **격자 표시** | 이 옵션을 활성화하면 3D 뷰포트에 격자가 표시됩니다. |
| **축** | 뷰포트에 격자가 표시되는 축을 따라 정의합니다. 응용 프로그램의 위쪽 축이므로 기본값은 Y입니다. |
| **격자 색상** | 뷰포트에 그릴 때 표시되는 그리드의 색입니다. |
| **격자 불투명도** | 뷰포트에 있는 격자의 불투명도입니다. |
