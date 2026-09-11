---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/workflow-issues/viewport-issues/viewports-and-textures-are-blurry-or-lack-sharpness.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 흐린 뷰포트 및 텍스처를 수정하여 선명하고 선명한 시각적 품질을 보장하는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Viewport Issues > Viewports and textures are blurry or lack sharpness
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 뷰포트와 텍스처가 흐리거나 선명도가 떨어집니다
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 1%

---


# 뷰포트와 텍스처가 흐리거나 선명도가 떨어집니다

서로 다른 이유로 뷰포트가 흐리게 표시될 수 있습니다.

## 높은 DPI 화면(Retina) 설정

기본적으로 Substance 3D Painter은 높은 DPI/Retina 화면에서 뷰 포트 해상도를 다운스케일하여 성능을 개선합니다.

이 동작은 **뷰포트 비율** 매개 변수를 변경하여 [기본 설정](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/general-71008262.html)에서 변경할 수 있습니다.

## 텍스처 필터링

뷰포트는 믹맵 및 텍스처 필터링을 사용하여 [스파스 가상 텍스처](../../../features/sparse-virtual-textures.md)에서 스트리밍 및 스트리밍하여 성능을 향상시킵니다. 경우에 따라 텍스처가 흐릿해질 수 있습니다.

텍스처 필터링은 [뷰포트 설정](../../../interface/display-settings/viewport-settings.md) 매개 변수 아래의 디스플레이 설정 창을 통해 조정할 수 있습니다.
