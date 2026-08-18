---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/display-settings/environment-settings.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 재질 미리 보기의 조명과 배경을 제어하도록 환경 설정을 구성하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Interface > Display settings > Environment settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 환경 설정
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---


# 환경 설정

**디스플레이 설정**&#x200B;의 이 섹션은 뷰포트의 조명을 제어합니다.

## 환경

![](../../assets/env-settings.png)

| *설정* | *설명* |
| --- | --- |
| **환경 맵** | 장면을 밝히는 데 사용할 환경 맵 텍스처입니다. &quot;환경&quot; 사전 설정을 사용하여 [에셋](../assets/assets.md) 창에서 찾을 수 있습니다.버튼을 클릭하여 미니 선반을 열고 다른 환경 맵을 선택합니다. |
| **환경 맵 색상 공간 재정의** | 현재 프로젝트에서 [색상 관리](../../features/color-management/color-management.md)를 사용하는 경우 이 설정을 활성화하여 환경 맵의 색상 공간을 재정의할 수 있습니다. |
| **환경 불투명도** | 뷰포트 배경에 있는 환경 텍스처의 가시성/불투명도를 제어합니다. 이 설정은 장면의 조명에 영향을 주지 않습니다. |
| **환경 노출** | 노출 값(EV)은 고정된 장면 광도를 나타내는 수치이다. 이 설정을 사용하면 기본 광도 값을 오프셋할 수 있습니다.응용 프로그램과 함께 제공되는 환경 맵을 사용하여 작업할 때는 이 설정을 0으로 유지해야 합니다. 잘못된 노출 값으로 에셋을 텍스처링하면 다른 애플리케이션에서 색상 보정 문제가 발생할 수 있습니다. |
| **환경 회전** | 환경 텍스처의 가로 회전을 제어합니다. 장면의 조명을 회전하고 개체의 반응 방식을 변경하는 데 유용합니다. [바로 가기](../settings/shortcuts.md)로 제어할 수 있습니다. |
| **환경 흐림 효과** | 뷰포트 배경에서 환경 텍스처가 얼마나 선명하거나 흐리게 표시되는지 제어합니다. 이 설정은 조명에 영향을 주지 않습니다. |
| **환경 맞춤** | 뷰포트 내에서 3D 모드를 기준으로 환경 텍스처가 회전하는 방식을 제어합니다. 이 설정은 로컬로 설정된 경우 3D 모델 아래의 영역을 밝게 하는 데 사용할 수 있습니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>세계</strong>(기본값): 환경이 장면에 정렬되고 3D 모델의 위쪽 축을 기준으로 회전합니다.</li><li data-preserve-html="true"><strong>로컬</strong>: 환경이 카메라에 정렬되고 카메라의 위쪽 축을 기준으로 회전합니다.</li></ul> |

## 그림자

![](../../assets/shadow-2.png)

| *설정* | *설명* |
| --- | --- |
| **어두운 영역** | 뷰포트에서 그림자 렌더링을 활성화/비활성화합니다. |
| **계산 모드** | 그림자가 계산되는 속도를 제어합니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong> 집약적 </strong>: 빠르게 계산하지만 뷰포트의 렌더링이 중단될 수 있습니다.</li><li data-preserve-html="true"><strong> 평균 </strong>: 강도 및 경량 모드의 평균입니다.</li><li data-preserve-html="true"><strong> 경량 </strong> : (기본값) 몇 초에 걸쳐 어두운 영역을 느리게 계산하지만 뷰포트 성능이 느려지지 않습니다.</li></ul> |
| **그림자 불투명도** | 장면에 그림자가 표시되는 정도를 제어합니다. |
