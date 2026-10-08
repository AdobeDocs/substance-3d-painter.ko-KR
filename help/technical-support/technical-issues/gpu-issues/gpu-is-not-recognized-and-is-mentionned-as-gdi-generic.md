---
breadcrumb-title: ""
description: 적절한 GPU 가속을 위해 Substance 3D Painter에서 GDI 일반으로 표시되는 GPU 인식 문제를 해결하는 방법에 대해 알아보십시오.
title: GPU가 인식되지 않으며 GDI 일반으로 언급됨
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%
---

# GPU가 인식되지 않으며 GDI 일반으로 언급됨

이 문제는 추적하기가 약간 복잡하며 여러 소스로 인해 발생할 수 있습니다.

* Nvidia Optimus가 설치된 컴퓨터에 있는 경우 다음 링크를 참조하십시오. [GPU가 인식되지 않음](gpu-is-not-recognized.md)
* 모니터가 기본 GPU에 연결되어 있는지, 그리고 Windows에서 이 모니터가 기본 디스플레이로 설정되어 있는지 확인합니다.
* Windows에서 기본 디스플레이의 색상 비트 심도가 32비트로 설정되어 있는지 확인하세요.
* 여전히 문제가 있는 경우 GPU 드라이버를 다시 새로 설치해 보십시오(Windows 레지스트리의 나머지 부분을 정리하는 동시에 전체 제거).
