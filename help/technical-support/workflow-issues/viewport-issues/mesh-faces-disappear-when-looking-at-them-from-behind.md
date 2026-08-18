---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/workflow-issues/viewport-issues/mesh-faces-disappear-when-looking-at-them-from-behind.html"
breadcrumb-title: ''
description: Substance 3D Painter 뷰포트에서 뒤에서 볼 때 망 모양이 사라지도록 수정하여 적절한 망 가시성을 유지하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Mesh faces disappear when looking at them from behind
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 뒤에서 볼 때 메시 얼굴이 사라집니다
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '86'
ht-degree: 0%

---


# 뒤에서 볼 때 메시 얼굴이 사라집니다

기본적으로 뷰포트의 메시는 메시 다각형의 뒤(뒷면)를 표시하지 않을 수 있습니다. 이는 현재 셰이더에 의해 컬링되기 때문입니다.

면 뒷면을 표시하려면 [셰이더 설정](../../../interface/shader-settings/shader-settings.md)에서 현재 셰이더를 **pbr-metal-rough-alpha-test**(으)로 변경하면 됩니다.
