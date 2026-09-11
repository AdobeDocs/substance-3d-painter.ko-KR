---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/gpu-issues/multi-bi-gpu.html"
breadcrumb-title: ''
description: 렌더링 성능을 최적화하기 위해 다중 GPU 및 Bi-GPU 시스템용 Substance 3D Painter을 구성하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > MultiBi-GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: MultiBi-GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%

---


# Multi/Bi-GPU

일부 GPU 구성 및/또는 GPU 모델은 Substance 3D Painter과 호환되지 않으며 불안정하고 충돌이 발생할 수 있습니다. 다음은 호환되지 않는 구성 목록입니다.

| ***구성*** | ***해결 방법*** |
| --- | --- |
| **Nvidia SLI / AMD Crossfire**(그래픽 카드 브리지) | GPU 드라이버 설정에서 SLI 또는 Crossfire를 비활성화합니다. |
| **Bi-GPU**(하나의 그래픽 카드에 GPU 칩셋 2개) | 드라이버 설정에서 두 GPU 칩셋을 하나만 사용하지 않도록 설정합니다. |
