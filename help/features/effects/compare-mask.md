---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/effects/compare-mask.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 [마스크 비교] 효과를 사용하여 텍스처 비교 작업을 기반으로 마스크를 만드는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Features > Effects > Compare Mask
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 마스크 비교
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---


# 마스크 비교

![](../../assets/compare-mask.png)

이 효과를 사용하면 두 채널을 빠르고 쉽게 비교하고 그 결과로 마스크를 만들 수 있습니다. 이 효과는 [레이어]의 마스크에만 사용할 수 있습니다.

아래는 이 효과에 대해 사용 가능한 설정입니다 .

| 설정 | 설명 |
| --- | --- |
| **채널** | 마스크를 만들 원본과 대상을 비교할 채널입니다. 이 목록은 [텍스처 집합 설정](../../interface/texture-set/texture-set-settings.md)에서 사용할 수 있는 채널을 기반으로 합니다. |
| **비교** | 여기서 세 가지 매개 변수를 사용하여 마스크 계산 방법을 선택할 수 있습니다. 중간에 있는 드롭다운은 비교 작업(보다 작음, 공차 내, 보다 큼)을 정의합니다. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/compare-mode.png"/></div> 소스 및 대상 모드:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>다음 레이어</strong> : 현재 레이어 아래에 있는 모든 레이어의 병합된 버전을 고려합니다.</li><li data-preserve-html="true"><strong>이 레이어</strong> : 이 레이어만 고려하십시오.</li><li data-preserve-html="true"><strong>이 마스크</strong> : 마스크의 기존 내용을 고려합니다(예: 채우기 효과 또는 생성기 효과가 이미 있는 경우).</li><li data-preserve-html="true"><strong>상수</strong> : 균일 값.</li></ul>작업은 다음과 같습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>보다 작음</strong> : 소스(왼쪽 드롭다운)의 값이 대상(오른쪽 드롭다운)보다 작으면 마스크에 흰색 값이 출력됩니다.</li><li data-preserve-html="true"><strong>허용치 내</strong> : 소스(왼쪽 드롭다운)의 값이 대상(오른쪽 드롭다운)과 비슷하면 마스크에 흰색 값이 출력됩니다.</li><li data-preserve-html="true"><strong>보다 큼</strong> : 소스(왼쪽 드롭다운)의 값이 대상(오른쪽 드롭다운)의 값보다 큰 경우 마스크에 흰색 값이 출력됩니다.</li></ul> |
| **상수** | 비교 설정이 &quot;상수&quot;로 설정된 경우 비교할 값입니다. |
| **경도** | 결과 마스크 비교의 Smoothness/경도를 제어합니다. |
| **소스 채널 막대 그래프** | 소스와 대상의 막대 그래프 보기를 제공합니다. 마스크가 약간 겹치는지 전혀 겹치지 않는지 확인하는 데 유용합니다(마스크와 겹치지 않으면 비어 있음).막대 그래프의 작동 방식에 대한 자세한 내용은 [수준](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/atomic-nodes/levels)을 참조하십시오. |

>[!NOTE]
>
> 레이어를 마우스 오른쪽 버튼으로 클릭하고 바로 가기 &quot;**Height 조합이 있는 마스크 추가**&quot;을(를) 선택하여 레이어에 이 새 효과를 빠르게 추가할 수 있습니다. 또한 이 바로 가기는 기본 &quot;**선형 닷지(추가)**&quot; 대신 Height 채널 **혼합 모드**&#x200B;를 &quot;**표준**&quot;(으)로 전환합니다.\
> ![](../../assets/compare-shortcut.png)
