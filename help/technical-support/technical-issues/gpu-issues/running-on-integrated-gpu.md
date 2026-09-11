---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/technical-issues/gpu-issues/running-on-integrated-gpu.html"
breadcrumb-title: ''
description: 성능 향상을 위해 통합 그래픽 대신 전용 GPU를 사용하도록 Substance 3D Painter을 구성하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Running on integrated GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 통합 GPU에서 실행
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# 통합 GPU에서 실행

![](../../../assets/integrated-gpu.png){width="500px"}

일부 컴퓨터는 전용 GPU가 아닌 통합 칩셋에서 실행되도록 기본적으로 설정된 경우가 있을 수 있습니다.\
통합 칩셋의 성능은 매우 낮으므로 대신 전용 GPU를 사용하는 것이 좋습니다. 팝업이 나타나면 이에 대한 경고가 표시됩니다.

NVIDIA GPU를 사용하는 경우 NVIDIA GPU로의 전환은 응용 프로그램 프로필에 따라 달라집니다. 애플리케이션에 이러한 프로필이 없는 경우 그래픽 카드를 수동으로 할당할 수 있습니다.

1. 바탕 화면을 마우스 오른쪽 단추로 클릭하고 NVIDIA 제어판을 선택합니다. **또는** 제어판으로 이동하여 NVIDIA 제어판을 검색합니다.
1. **3D 설정**&#x200B;에서 **3D 설정 관리**(으)로 이동
1. **프로그램 설정** 탭에서 **Substance 3D Painter**&#x200B;에 대한 새 프로필을 추가합니다.
1. 기본 설정 그래픽 프로세서 설정을 고성능 NVIDIA 프로세서 로 변경합니다.
