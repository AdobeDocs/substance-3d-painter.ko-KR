---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/technical-issues/gpu-issues/crash-when-working-with-overclocked-gpu.html"
breadcrumb-title: ''
description: 안정적인 애플리케이션 성능을 위해 오버클럭된 GPU로 작업할 때 Substance 3D Painter 충돌을 해결하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > GPU Issues > Crash when working with overclocked GPU
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 오버클럭된 GPU로 작업할 때 충돌 발생
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# 오버클럭된 GPU로 작업할 때 충돌 발생

오버클럭된 GPU는 처음에 GPU 생성자가 설계하지 않은 주파수를 실행하므로 불안정할 수 있습니다. GPU가 오버클럭되어 있고 안정성 문제가 있는 경우 잠시 동안 공장 기본 주파수로 돌아가는 것이 좋습니다.

## Nvidia GPU

Nvidia GPU의 경우 드라이버 355.82부터 드라이버 설정에서 디버그 모드를 활성화하여 GPU 오버클럭킹을 일시적으로 비활성화할 수 있습니다. 이를 통해 그래픽 카드와 관련된 문제를 확인하고 판단할 수 있다.

디버그 모드를 사용하려면 다음을 수행하십시오.

1. **Nvidia 제어판**&#x200B;을 엽니다(데스크탑의 오른쪽 클릭).
1. **도움말** 메뉴를 클릭합니다.
1. **디버그 모드**&#x200B;를 클릭합니다.

>[!NOTE]
>
> GPU가 참조 카드인 경우 디버그 모드를 사용할 수 없습니다. GPU가 비표준 시계에서 실행되거나 수정된 BIOS와 함께 실행되는 경우에만 사용할 수 있습니다. 이 경우 오버클럭킹을 수동으로 비활성화하는 것이 좋습니다.
