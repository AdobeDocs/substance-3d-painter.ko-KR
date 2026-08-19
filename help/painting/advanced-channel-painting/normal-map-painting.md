---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/painting/advanced-channel-painting/normal-map-painting.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 직접 표준 맵을 페인트하여 텍스처에 표면 세부 사항과 깊이를 추가하는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Normal Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 표준 맵 페인팅
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---


# 표준 맵 페인팅

페인팅 세부 사항은 메시에 직접 표준 맵 데이터를 페인팅하여 수행할 수 있습니다. 이 페이지에서는 다른 방식으로 재그룹화하여 일반 맵 페인팅을 관리합니다.

## 표준 맵 세부 정보 페인팅

표준 맵 세부 정보를 페인트하려면 다음을 수행합니다.

1. 현재 텍스처 세트에 표준 채널을 추가합니다(아직 없는 경우)
1. 현재 페인팅 도구에서 표준 채널 활성화
1. 현재 페인팅 도구의 [재질] 섹션에 있는 [표준] 슬롯에 표준 리소스를 로드합니다.

거기서부터, 표준 지도로 페인팅하는 것은 구운 표준의 정확도가 더해져 [Height 맵 페인팅](height-map-painting.md)과 매우 비슷합니다.

![](../../assets/normal-painting.gif)

## 표준 혼합 모드

표준 맵은 레이어 스택에 고유한 혼합 모드가 있습니다.

* **표준 맵 세부 정보**(기본값)
* **표준 맵 역산 세부 정보**
* **표준 맵 결합**

자세한 내용은 [혼합 모드](../../interface/layer-stack/blending-modes.md) 페이지를 참조하세요.

## 표준 색상 공간

표준 맵을 재질의 슬롯에 로드할 때(도구 속성 또는 칠 레이어) 기본 색상 공간을 변경할 수 있습니다.

기본적으로 DirectX(Y-) 표준 맵이 필요한데(프로젝트 설정의 영향을 받지 않음) 이 설정을 사용하여 표준 맵 포맷을 지정할 수 있습니다. 따라서 OpenGL(Y+) 표준 맵을 사용할 때는 작은 화살표를 클릭하여 색상 공간 메뉴를 연 다음 비트맵의 색상 공간을 변경해야 합니다.

![](../../assets/normal-color-space.png)

## 구운 표준 맵 위에 페인팅

경우에 따라 디테일을 숨기거나 베이킹 문제를 해결하기 위해 구운 표준 맵 위에 페인트하는 것이 유용할 수 있습니다.\
Substance 3D Painter에서 프로젝트의 기본 설정에서는 보통 채널과 구운 보통 채널을 개별적으로 계산하기 때문에 이 설정이 허용되지 않습니다. 이 동작은 [텍스처 설정](../../interface/texture-set/texture-set-settings.md) 을 통해 변경할 수 있습니다.

### 1 - 텍스처 세트 혼합 모드 변경

기본적으로 텍스처 세트는 **일반 믹싱** 설정이 **결합**(으)로 설정된 상태로 만들어집니다.

일반 맵을 재정의/페인트하려면 대신 이 설정을 **바꾸기**(으)로 설정해야 합니다. 표준 지도는 뷰포트에서 사라지지만, 그것은 예상된 것이다. 이 모드를 **바꾸기**(으)로 변경하면 최종 표준 맵을 생성할 때 일반 채널과 Height 채널만 고려하도록 Substance 3D Painter에 지시됩니다.

![](../../assets/normal-mixing.png)

### 2 - 적용된 표준 맵으로 채우기 레이어 설정

새 칠 레이어를 만들고 속성 패널을 통해 &quot;표준&quot; 슬롯 내에 구운 표준 레이어를 놓습니다. 칠 레이어가 1로 설정되어 있지 않은 경우 기본 틸링을 변경해야 합니다.

![](../../assets/fill-layer_1.gif)

### 3 - 칠 레이어 혼합 모드 변경

기본적으로 새 레이어에 있는 일반 채널의 혼합 모드는 &quot;표준 맵 세부 정보&quot;로 설정됩니다. 기본 레이어는 채우기 레이어를 사용하는 것이 좋으므로 비트맵에 알파가 없으므로 &quot;표준&quot; 혼합 모드를 선택한 다음 아래 모든 것을 대체합니다(셰이더의 기본 색상 포함).

![](../../assets/blending-mode.gif)

### 4 - 구워진 표준 맵 위에 페인트할 레이어 만들기

새 레이어(일반 또는 칠)를 만들고 일반 채널에 대한 혼합 모드를 &quot;표준&quot;으로 변경합니다. 이 설정이 완료되면 표준 채널에서 페인팅한 모든 항목이 아래 레이어에 있는 구운 표준 맵을 대체합니다.

![](../../assets/normal-painting-over.gif)
