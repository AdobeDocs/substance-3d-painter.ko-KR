---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/painting/dynamic-strokes/enabling-dynamic-stroke-feature.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 동적 획 기능을 사용하여 다양한 효과로 반응형 브러시 획을 만드는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Enabling Dynamic Stroke Feature
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 동적 선 기능 활성화
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 2%

---


# 동적 선 기능 활성화

역동적인 획 기능을 활성화하려면 먼저 특정 리소스가 필요합니다.

## 역동적인 획 호환 리소스 찾기

[에셋](../../interface/assets/assets.md) 창을 탐색할 때 축소판 오른쪽 하단에 있는 전용 아이콘이 리소스의 호환성 유형을 나타냅니다. 아이콘이 표시되지 않으면 리소스가 기능을 활용할 수 없음을 의미합니다.

| *아이콘* | *설명* |
| --- | --- |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-dyn.png"/></div> | 이 리소스는 다음 비헤이비어 중 하나 이상을 사용할 수 있습니다.<ul data-preserve-html="true"><li data-preserve-html="true">스탬프 인덱스</li><li data-preserve-html="true">시간</li><li data-preserve-html="true">임의 시드</li></ul> |
| <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/icon-random.png"/></div> | 이 리소스는 Random Seed 매개 변수만 표시합니다. |

다음 키워드와 함께 Shelf 의 검색 필드를 사용하여 리소스를 검색할 수도 있습니다.

* 동적 뇌졸중
* 임의화 시드

## 역동적인 획 매개 변수

![](../../assets/dynamic-strokes-settings.png)

동적 획 리소스가 로드되면 새 매개 변수 목록이 Substance 매개 변수 그룹 바로 앞에 추가됩니다.

| *매개 변수* | *설명* |
| --- | --- |
| **동적 컨트롤** | 현재 사용되는 Substance 파일에서 사용할 수 있는 매개 변수를 나열합니다. |
| **스탬프 시작** | 리소스에 동적 컨트롤 &quot;스탬프 인덱스&quot;가 있는 경우에만 사용할 수 있습니다. 브러시 획 안에 있는 스탬프의 색인이 시작되는 값을 나타냅니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>시작(0)</strong>: 기본값입니다. 색인은 각각의 새 획에서 0부터 시작합니다.</li> <li data-preserve-html="true"><strong>임의 인덱스에서</strong>: 인덱스가 스탬프 주기 카운트에 의해 정의된 최대값인 임의 값에서 시작합니다. 다음 값은 여전히 순서대로 있으며 완전히 무작위하지는 않습니다.</li> </ul> |
| **스탬프 주기 수** | 리소스에 동적 컨트롤 &quot;스탬프 인덱스&quot;가 있는 경우에만 사용할 수 있습니다. 이 매개 변수는 Substance 3D Painter에서 새 Substance 변형 생성을 중단하고 기존 변형 재생을 시작해야 하는 시기를 제어합니다. 이 매개 변수는 성능에 큰 영향을 미치며, [동적 선 성능](dynamic-stroke-performances.md)에 대해 자세히 알아볼 수 있습니다. |
| **임의화 형식** | 리소스에 동적 컨트롤 &quot;임의 시드&quot;가 있는 경우에만 사용할 수 있습니다. 임의화의 변경 방식을 제어합니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>단일</strong>: 기본값입니다. Substance 매개 변수를 통해 수동으로 설정할 수 있는 단일 임의화 값을 사용합니다.</li> <li data-preserve-html="true"><strong>획당 임의</strong>: 각 새 브러쉬 획에 대해 새 임의 시드 값을 생성합니다.</li> <li data-preserve-html="true"><strong>스탬프당 무작위</strong>: 브러시 획 내의 각 스탬프에 대해 새 무작위 시드 값을 생성합니다. <em><strong>매개 변수는 비용이 많이 들 수 있으므로 주의하세요</strong>.</em></li> </ul> |
| **시간** | 시간 동적 컨트롤에 매개 변수가 없습니다. 브러쉬 획의 페인팅 시간에 따라 시간이 달라집니다. |

## 호환되는 도구 목록

동적 획 설정은 다음 도구 및 컨텍스트에서만 사용할 수 있습니다.

| *도구 유형* | *호환 리소스 슬롯* |
| --- | --- |
| **페인트** | <ul data-preserve-html="true"><li data-preserve-html="true">알파</li><li data-preserve-html="true">재질</li></ul> |
| **지우개** | <ul data-preserve-html="true"><li data-preserve-html="true">알파</li><li data-preserve-html="true">재질</li></ul> |
| **투영** | <ul data-preserve-html="true"><li data-preserve-html="true">알파</li></ul> |
| **손가락** | <ul data-preserve-html="true"><li data-preserve-html="true">알파</li></ul> |
| **복제** | <ul data-preserve-html="true"><li data-preserve-html="true">알파</li></ul> |

>[!NOTE]
>
> 역동적인 획은 **파티클** 과(와) 호환되지 않으므로 물리적 모드에서 도구를 사용할 때 이 기능이 비활성화됩니다.
