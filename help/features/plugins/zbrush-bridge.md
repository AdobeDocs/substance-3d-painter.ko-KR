---
breadcrumb-title: ''
description: Substance 3D Painter 버전 전체의 모든 변경 내용 및 업데이트를 검토하여 시간의 흐름에 따른 기능 변화 및 개선 사항을 추적하세요.
title: ZBrush와 Painter Bridge
user-guide-description: ''
user-guide-title: ''
source-git-commit: c50b48e520277293b9ddef466baf8e27db4891ab
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---


# ZBrush와 Painter Bridge

ZBrush 2026.2.0(Maxon One 2026년 4월 업데이트) 및 Substance 3D Painter 12.0.2(Steam 및 CC 버전)부터 최신 버전의 ZBrush와 함께 자동으로 설치된 플러그인을 통해 ZBrush에서 Painter으로 직접 모델을 보낼 수 있습니다.

![Zbrush와 Painter에서 동일한 에셋으로 겹쳐서 렌더링된 에셋을 보여 주는 프로모션 이미지입니다.](../../assets/zbrush_promotional.png)

Substance Bridge 플러그인을 사용하면 별도의 low-poly 및 high-poly 파일을 내보내고 Painter으로 가져오고 베이크를 구성 및 실행하는 긴 프로세스를 거칠 필요가 없습니다.

Zbrush를 사용하여 Painter bridge로 시작하려면:

1. ZBrush 2026.2.0 이상 버전이 설치되어 있는지 확인하십시오.
1. **Python > zbrush_painter_plugin**&#x200B;이 선택되어 있는지 확인하여 Painter 내에서 플러그인을 활성화합니다.
1. ZBrush의 **Painter으로 보내기**&#x200B;는 **텍스처 > Substance 브리지**&#x200B;에서 사용할 수 있습니다.

![ZBrush의 Substance Bridge 플러그인 사진](../../assets/zbrush_painterSendTo.png)

## 구성

Painter에서 자동 프로젝트 생성을 위해 다음 설정을 구성할 수 있습니다.

| 설정 | 설명 |
| --- | --- |
| Painter으로 보내기 | 현재 설정이 적용된 모델을 Substance 3D Painter으로 보냅니다. 클릭할 때마다 처음부터 새 Substance 프로젝트가 만들어집니다. |
| **하위 도구** | |
| 전체 | 가시성과 관계없이 모든 SubTool을 보냅니다. 안구가 켜져 있든 꺼져 있든, 모든 것이 보내집니다. |
| 보임 | SubTool 목록에서 눈 아이콘이 켜져 있는 SubTools만 보냅니다. |
| 활성 | 현재 선택한 하위 도구만 보냅니다. |
| PolyPaint 보내기 | [폴리 페인트]를 텍스처 맵으로 변환하고 Substance에서 칠 레이어로 적용하여 페인트 위에 놓고 혼합할 수 있습니다. |
| 스무드 노멀스 | 내보낼 때 탄젠트 법선을 매끄럽게 하여 Substance에서 면처리된 메시가 매끄럽게 나타나도록 하여 게임 엔진이 이를 렌더링하는 방식과 일치합니다. 도형의 실제 면을 보려면 끕니다. |
| 지도 자동 굽기 | 모델이 도달한 후 Substance의 베이킹 알고리즘을 자동으로 실행하여 높음/낮음 메시 비교에서 노멀 맵, 앰비언트 오클루전, 곡률 및 기타 세부 맵을 생성합니다. |
| UV 자동 언랩 강제 적용 | 도착하는 모든 하위 도구에 대해 Substance의 UV 감싸기 해제 알고리즘을 트리거합니다. UV가 이미 좋은 경우 덮어쓰므로 끄십시오. |
| 서브디비전 수준 | 전송할 서브디비전 수준을 제어합니다. [현재]는 표시된 레벨만 보냅니다. [낮음 및 높음]을 선택하면 굽기에 가장 낮은 레벨과 가장 높은 레벨이 모두 전송되며 대부분의 워크플로우에 권장되는 옵션입니다. |
| 텍스처 세트 | Substance에서 UV 공간을 분할하는 방법을 제어합니다. [하위 도구당] (SubTool당 하나의 텍스처 세트) 또는 [폴리 그룹당] (각 SubTool 내에서 [폴리 그룹당 하나의 텍스처 세트]) 중에서 선택할 수 있습니다. |

Painter이 모델을 받으면 자동 굽기가 활성화되면 굽기가 실행됩니다. 모델의 가장 낮은 세분화는 low-poly mesh로 가져온 mesh이며 가장 높은 세분화는 high-poly로 사용하여 디테일을 굽는다. ZBrush는 Painter보다 훨씬 많은 수의 다각형을 처리할 수 있으므로 낮은 폴리 메쉬가 최적의 작업 크기를 갖는지 확인하십시오(기계에 따라 다르지만 100만 미만이 가장 좋습니다).

Painter의 [텍스처 세트]는 재질 할당을 나타냅니다. 하나의 텍스처 세트는 하나의 UV 공간과 같습니다.

* [하위 도구]별로 각 하위 도구에 대해 하나의 [텍스처 세트]를 만듭니다(모든 하위 도구 부분이 동일한 UV 공간을 공유함). 이 옵션이 더 간단합니다.
* Per PolyGroup은 각 SubTool 내에서 PolyGroup당 하나의 텍스처 세트를 생성하여 재료 할당을 보다 세밀하게 제어할 수 있습니다.

>[!NOTE]
>
>Painter의 Steam 버전에서는 Painter이 열려 있어야 ZBrush 모델을 사용할 수 있습니다.


## 추가 리소스

[이 비디오를 시청](https://www.youtube.com/watch?v=fLkkwV4BzrU)하여 Bridge의 작동 상태를 보거나 [ZBrush 설명서](https://help.maxon.net/zbr/en-us/Default.htm#html/reference-guide/texture/substance-bridge/substance-bridge.html?Highlight=painter)에 액세스하여 자세한 내용을 확인하십시오.
