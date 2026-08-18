---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/workflow-issues/tools-issues/normal-map-looks-incorrect-when-loaded-in-layer-or-tool-properties.html"
breadcrumb-title: ''
description: 정확한 표면 세부 사항을 위해 Substance 3D Painter 레이어 및 도구 속성에서 일반적인 맵 표시 문제를 해결하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Tools Issues > Normal map looks incorrect when loaded in layer or tool properties
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 레이어 또는 도구 속성에 불러올 때 표준 맵이 잘못 표시
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '105'
ht-degree: 0%

---


# 레이어 또는 도구 속성에 불러올 때 표준 맵이 잘못 표시

칠하기 레이어의 현재 도구에 표준을 로드할 때 이 표준이 OpenGL 표준 맵인 경우 잘못 표시될 수 있습니다.\
이유는 매우 간단합니다. Substance 3D Painter 엔진은 로드된 표준 맵이 기본적으로 DirectX으로 간주합니다.

이 비헤이비어는 Substance 재질 또는 전용 채널 옆에 있는 작은 화살표를 클릭하여 쉽게 편집할 수 있습니다.

![](../../../assets/channel-format-override.png)
