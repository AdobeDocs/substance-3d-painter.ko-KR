---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.html"
breadcrumb-title: ''
description: 안정적인 렌더링과 성능을 보장하기 위한 Substance 3D Painter의 GPU 드라이버 호환성 요구 사항에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > GPU drivers compatibility
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPU 드라이버 호환성
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 2%

---


# GPU 드라이버 호환성

이 페이지에서는 Substance 3D Painter 문제를 일으킬 수 있는 GPU 드라이버에 대한 정보를 다시 그룹화합니다.

## Nvidia

아래 표에는 Nvidia GPU(GeForce 또는 Quadro 모델) 문제를 생성하는 데 알고 있는 모든 드라이버 버전이 나열되어 있습니다.

| *드라이버 버전* | *문제 설명* |
| --- | --- |
| <b> 425.xx </b> | GPU 광선 추적 가공물. |
| <b> 429.xx 이상 </b> | 검은색 텍스처가 가공물을 차단합니다. |
| <b> 435.xx 이상 </b> | 텍스처를 계산할 때 sRGB 색상 문제가 발생합니다. |
| <b> 439.xx </b> | 텍스처 손상. |
| <b> 441.08 </b> | 충돌 또는 안정성 문제. |
| <b> 442.19 </b> | 충돌 또는 안정성 문제. |
| <b>528.09</b> | 운영 체제 중단. |
| <b>572.16~572.42</b> | 텍스처를 굽는 동안 아티팩트 또는 충돌이 발생합니다. |

### AMD

| *드라이버 버전* | *문제 설명* |
| --- | --- |
| **20.7.x** - **20.11.2** | 텍스처 결함 또는 손상. |
| **20.11.3** - **21.2.1** | 텍스처 문제 또는 손상과 충돌 또는 안정성 문제가 함께 발생합니다. |
| **21.2.3** - **21.6.1** | 충돌 또는 안정성 문제. |
