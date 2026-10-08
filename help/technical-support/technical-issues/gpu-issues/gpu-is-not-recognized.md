---
breadcrumb-title: ""
description: Substance 3D Painter에서 GPU 인식 문제를 해결하여 적절한 하드웨어 가속 및 성능을 활성화하는 방법을 알아봅니다.
title: GPU가 인식되지 않음
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '79'
ht-degree: 0%
---

# GPU가 인식되지 않음

![](../../../assets/not-recognized-gpu.png){width="500px"}

일부 **NVIDIA Optimus** 사용자는 Substance 3D Painter을 올바른 GPU에서 실행하는 데 문제가 있을 수 있습니다. 해결 방법: Windows 레지스트리의 다음 키를 0으로 설정합니다.

* HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
* HKEY\_LOCAL\_MACHINE\SOFTWARE\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Windows\RequireSignedAppInit
