---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/project-issues/preserve-brush-strokes-setting-stays-disabled.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 브러시 획을 올바르게 유지하기 위해 비활성화 상태로 유지되는 브러시 획 보존 설정을 수정하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Preserve brush strokes setting stays disabled
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 브러시 획 유지 설정이 비활성화된 상태 유지
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# 브러시 획 유지 설정이 비활성화된 상태 유지

Substance 3D Painter 1.5에서 발생한 불행한 버그(1.7에서 부분적으로 수정됨) 때문에 일부 프로젝트에서는 메쉬와 관련된 메타데이터가 손실됩니다. 따라서 이 버그는 [프로젝트 구성](../../../interface/project-configuration.md) 창에서 &quot;메시 상의 선 위치 유지&quot; 설정을 사용하지 않도록 설정합니다.

이 문제를 해결하려면 몇 가지 특정 단계를 따라야 합니다 :

* Substance 3D Painter 1.7 이상에서 문제가 있는 프로젝트를 엽니다
* 편집 > 프로젝트 구성으로 이동합니다.
* 업데이트된 버전이 아닌 현재 프로젝트에서 사용한 원래 메시를 선택하고 다시 가져옵니다
* Substance 3D Painter에서 레이어를 확인하고 계산하도록 합니다. 동일한 메쉬이면 아무것도 변경되지 않습니다
* 편집 > 프로젝트 구성으로 다시 이동
* 이제 새 메시를 가져올 수 있도록 &quot;메시에서 선 위치 유지&quot;가 다시 활성화되어야 합니다
