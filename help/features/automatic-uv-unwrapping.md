---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/automatic-uv-unwrapping.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 자동 UV 언래핑을 사용하여 3D 모델에 사용할 UV 레이아웃을 자동으로 생성하는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Features > Automatic UV Unwrapping
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 자동 UV 풀기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# 자동 UV 풀기

![](../assets/auto-unwrap-update-810.jpg)\
자동 UV 언래핑을 사용하면 3D 모델을 가져올 때 자동으로 UV 섬을 생성할 수 있습니다. 기존 UV가 없는 3D 모델을 페인트으로 표시하는 데 사용할 수 있습니다.

## 자동 UV 감싸기 해제 사용

![](../assets/uv-new-project.png)

새 프로젝트를 만들거나 기존 프로젝트로 메시를 다시 가져오는 경우 &quot;자동 줄 바꿈&quot; 설정이 선택되어 있는지 확인합니다. 비활성화된 경우 프로세스를 건너뛰고 메시 UV가 그대로 유지됩니다.

## UV 감싸기 해제 설정

![](../assets/unwrap-settings.png)

메쉬를 가져오고 감싸기 해제 프로세스를 사용할 때는 다음과 같은 설정을 사용할 수 있습니다. 일부 설정은 인터페이스의 옵션 버튼을 통해 사용할 수 있습니다.

| 섹션 | ***설정*** | ***설명*** |
| --- | --- | --- |
| **시퀀스 줄 바꿈 해제** | **이음새** | 솔기(UV 섬 테두리)가 없거나 항상 재생성되는 메시에 대해서만 솔기를 생성할지 여부를 제어합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> 누락된 데이터 </strong>을(를) 생성합니다(기본값). 누락된 메시에 대해 솔기가 생성됩니다.</li><li data-preserve-html="true"><strong> 모든 </strong>을(를) 다시 계산 : 모든 메시에 대해 솔기가 생성됩니다.</li></ul> |
| **UV 섬** | UV가 없는 메시나 메시에 대해 UV 감싸기 해제를 생성할지 여부를 제어합니다. 가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> 누락된 데이터 </strong>을(를) 생성합니다(기본값). 누락된 UV에 대해 UV 감싸기가 생성됩니다.</li><li data-preserve-html="true"><strong> 모든 </strong>을(를) 다시 계산 : 모든 메시에 대해 UV 감싸기가 생성됩니다.</li></ul> |  |
| **패킹** | 메시 UV 섬의 패킹/레이아웃을 제어합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> 누락된 데이터 </strong>을(를) 생성합니다(기본값). UV가 없는 메시에 대해 UV 섬을 압축합니다.</li><li data-preserve-html="true"><strong> 모든 </strong> 다시 계산 : 모든 UV 섬 압축.</li></ul> |  |
|  |  |  |
| **레이아웃 사용자 지정** | **여백 크기** | UV 섬 사이의 간격을 정의합니다. 이 설정은 해상도와는 독립적인 일반 백분율을 적용합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong> 여백 없음 </strong> : 0%</li><li data-preserve-html="true"><strong> 작은 </strong>(기본값): 0.2%</li><li data-preserve-html="true"><strong> 중간 </strong> : 0.5%</li><li data-preserve-html="true"><strong> 큰 </strong>: 1%</li></ul> |
|  | **UV 섬 방향** | 패킹 프로세스 중에 UV 섬 방향을 제어합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>제한 없음</strong>(기본값): 방향을 계산하는 데 제한이 적용되지 않습니다.</li><li data-preserve-html="true"><strong>3D 메시에 맞춤</strong>: UV 섬이 메시 방향을 향하도록 제한합니다</li></ul> |
|  |  |  |
| **UV 타일** | **최대 UV 타일 수** | UV 타일 워크플로우를 사용하는 경우 이 설정은 UV 섬에서 배포할 최대 타일 수를 결정합니다. |
|  |  |  |
| **최적화** | **길어진 UV 섬 방지** | 이 프로세스가 활성화된 경우 너무 긴 것으로 간주되는 UV 섬을 분할하여 텍스처 공간 사용을 개선할 수 있습니다.앞(위쪽)과 뒤(아래쪽)의 예: <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r10-column-c2_dynamic_grid_items_grid-cell_position-par_image" src="../assets/uv-before-after.jpg" width="400px"/></div> |

## 알려진 제한 사항

다음은 래핑 해제 프로세스와 관련된 제한 사항 목록입니다.

* 높은 폴리 메쉬를 처리하는 데는 오랜 시간이 걸릴 수 있습니다.
* 정확히 동일한 좌표의 정점이 병합됩니다
* 드물게 일부 메시 부분에서 UV 생성이 실패할 수 있습니다
* 경우에 따라 단일 UV 섬에서 균일하지 않거나 매우 왜곡된 텍셀 비율
* 텍스처 세트 간의 균일한 텍셀 비율
* 생성된 UV 섬은 매우 길어질 수 있고, 경우에 따라 UV 공간에 맞지 않을 수 있다
* 가장자리가 작거나 겹치는 퇴화된 면 또는 비삼각형 메시 면은 UV를 언랩할 수 없습니다
