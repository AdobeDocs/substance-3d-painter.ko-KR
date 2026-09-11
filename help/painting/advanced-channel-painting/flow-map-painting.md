---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/advanced-channel-painting/flow-map-painting.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 플로우 맵을 페인트 하여 재질 흐름 방향과 이방성 효과를 제어하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Flow Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 플로우 맵 페인팅
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# 플로우 맵 페인팅

전용 채널이 계획되어 있지만 그 동안 표준 채널과 일부 브러시 매개 변수를 사용하여 Substance 3D Painter에서 플로우 맵을 페인트할 수 있습니다.

## 1단계 : 노멀 맵 만들기

16 x 16픽셀의 노멀 맵 텍스처를 만듭니다. 색상은 128, 255, 128이어야 합니다. ![](../../assets/up-dx.png)\
(이 색상은 DirectX에서 위를 올려다보는 벡터의 해당)

## 2단계 : 일반 채널 추가

Substance 3D Painter 프로젝트에서 이 채널이 없는 경우 **텍스처 설정**&#x200B;을 통해 **표준** 채널을 추가하세요.

## 3단계 : 브러시 설정

브러쉬 매개 변수에서 경로 따르기 기능을 활성화합니다. 노멀 맵 텍스처(1단계)를 일반 채널 슬롯에 로드합니다. 다른 채널을 비활성화합니다.

![](../../assets/brush-settings-1.png){width="300px"}

## 4단계 : 페인트 !

노멀 맵 따라가기 설정을 활성화한 상태로 메시를 페인트하면 브러쉬 선이 패스에 방향을 그립니다.

![](../../assets/painting-1.png){width="700px"}
