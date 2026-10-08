---
breadcrumb-title: ""
description: Substance 3D Painter 레이어의 노멀 맵 표시 문제와 정확한 표면 세부 사항을 위한 도구 속성을 해결하는 방법을 알아봅니다.
title: 레이어 또는 도구 속성에 로드하면 노멀 맵이 잘못 표시됩니다
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '105'
ht-degree: 0%
---

# 레이어 또는 도구 속성에 로드하면 노멀 맵이 잘못 표시됩니다

표준 레이어를 현재 칠 레이어 노멀 맵으로 불러올 때 이 도구가 OpenGL 도구이면 잘못 표시될 수 있습니다.\
이유는 매우 간단합니다. Substance 3D Painter 엔진은 로드된 노멀 맵이 기본적으로 DirectX으로 간주합니다.

이 비헤이비어는 Substance 재질 또는 전용 채널 옆에 있는 작은 화살표를 클릭하여 쉽게 편집할 수 있습니다.

![](../../../assets/channel-format-override.png)
