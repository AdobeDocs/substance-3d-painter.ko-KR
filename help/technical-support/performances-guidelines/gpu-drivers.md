---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/performances-guidelines/gpu-drivers.html"
breadcrumb-title: ''
description: 렌더링 성능과 안정성을 최적화하기 위한 Substance 3D Painter의 GPU VRAM 및 드라이버 요구 사항에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > GPU Drivers
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: GPU VRAM 및 드라이버
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---


# GPU 드라이버

권장 드라이버를 사용하지 않으면 성능을 보장할 수 없습니다. WHQL이 아닌 드라이버는 사용하지 않아야 합니다.\
GPU 드라이버는 다른 소프트웨어와 마찬가지로 새로운 릴리스마다 성능 문제가 발생할 수 있습니다. 최신 드라이버 버전으로 업데이트한 후 문제가 발생하면 드라이버를 이전 버전으로 다운그레이드하는 것이 좋습니다.

## NVIDIA 드라이버 설정

일부 기본 NVIDIA 설정은 성능에 영향을 줄 수 있습니다. 프로필을 만들고 다음 매개 변수를 비활성화하는 것이 좋습니다(비활성화로 설정).

* 스레드 최적화
* 세로 동기화

## 다른 응용 프로그램에서 GPU를 활용하는 방법

Substance 3D Painter만 GPU를 사용하는 것이 아니라 다른 응용 프로그램도 동일한 작업을 수행합니다. Blender, Maya, Unreal Engine, Unity, C4D 등 Painter과 함께 일반적으로 사용되는 것을 포함하여 거의 모든 3D 응용 프로그램이 GPU 및 VRAM을 사용하여 실행됩니다. 이러한 응용 프로그램을 열어 둔 상태에서 좋은 성능을 보장하기 위한 솔루션은 자체 VRAM 할당을 요청하기 위해 Substance 3D Painter이 먼저 시작되었는지 확인하는 것입니다. 여전히 일부 소프트웨어는 VRAM의 일부를 동적으로 얻을 수 있으며 Painter 이후에 시작하더라도 Substance 3D Painter과 충돌할 수 있습니다.

일반적으로 Painter에서 VRAM을 더 많이 액세스할 수 있을수록 더 빨리 실행될 것이므로 Painter과 동시에 실행되는 다른 응용 프로그램에서 사용하는 VRAM의 양을 최소화하려고 합니다.

## GPU VRAM 양 및 대역폭

Substance 3D Painter은 대부분의 계산을 GPU에 의존합니다. [시스템 요구 사항](../../getting-started/system-requirements.md)을 준수하는 GPU가 중요한 이유가 여기에 있습니다.

Painter은 최종 텍스처를 만들기 위한 혼합 작업과 같은 계산을 수행하기 위해 텍스처를 GPU 메모리(VRAM)로 전송하여 작동합니다. 그러나 VRAM이 꽉 차기 시작하면 사용하지 않은 텍스처가 컴퓨터의 RAM으로 다시 전송되어 VRAM 공간을 확보합니다. Substance 3D Painter은 작업 시 GB의 데이터를 쓰고 읽습니다. 즉, 전송 시 VRAM 용량(양)과 대역폭 속도가 모두 중요합니다. [MSI AfterBurner](https://www.msi.com/page/afterburner)와 같은 도구를 사용하여 이 동작을 모니터링할 수 있습니다.

>[!NOTE]
>
> <b>Nvidia GTX 970</b>은 Substance 3D Painter에 영향을 주는 GPU 메모리와 관련하여 문제가 있는 디자인으로 알려져 있습니다. 마지막 500MB의 전체 4GB는 나머지 3.5GB보다 느린 속도로 작동합니다. Substance 3D Painter이 이러한 마지막 500MB에서 작동하면 성능을 10배까지 줄일 수 있습니다(측정한 값에서). 자세한 기술 정보는 <https://www.pcper.com/news/Graphics-Cards/NVIDIA-Responds-GTX-970-35GB-Memory-Issue>을(를) 참조하십시오.
