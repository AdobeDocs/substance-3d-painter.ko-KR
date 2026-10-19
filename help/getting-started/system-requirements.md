---
breadcrumb-title: ""
description: Substance 3D Painter에 대한 시스템 요구 사항을 검토하여 컴퓨터가 하드웨어 및 소프트웨어 사양을 충족하는지 확인하십시오.
title: 시스템 요구 사항
user-guide-description: ""
user-guide-title: ""
source-git-commit: fbfe7e52b226b5a92f5b46ebbf82728f0ff9e3c5
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 1%
---

# 지원되는 시스템

다음은 애플리케이션에서 지원하는 하드웨어 및 시스템 목록입니다.

## Windows

|  | 최소 | 권장 | 최적 |
| --- | --- | --- | --- |
| **OS** | Windows 11 64비트 버전 23H2 | Windows 11 64비트 버전 24H1 | Windows 11 64비트 버전 24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8GB | 16GB | 24GB |
| **RAM** | 16GB | 32GB | 64GB |
| **저장소** | 30GB의 사용 가능한 공간이 있는 SSD | 50GB의 사용 가능한 공간이 있는 SSD | 70GB의 사용 가능한 공간이 있는 SSD |

### macOS

|  | 최소 | 권장 | 최적 |
| --- | --- | --- | --- |
| **OS** | macOS 세쿼이아 | macOS 골든 게이트 | macOS 골든 게이트 |
| **CPU** | Apple | Apple | Apple M4 Pro |
| **GPU** | Apple | Apple | Apple M4 Pro |
| **RAM** | 16GB | 32GB | 64GB |
| **저장소** | 30GB의 사용 가능한 공간이 있는 SSD | 50GB의 사용 가능한 공간이 있는 SSD | 70GB의 사용 가능한 공간이 있는 SSD |

>[!WARNING]
>
> [VFX 참조 플랫폼](https://vfxplatform.com/)을(를) 염두에 두고 빌드된 파이프라인의 경우 Substance 3D Painter을 macOS 14 Sonoma에 계속 설치할 수 있습니다. 그러나 Painter은 최소 시스템 요구 사항 미만의 OS 버전에서 더 이상 테스트되지 않으므로 안정성이 보장되지 않습니다.

### 리눅스

| 기업 | 증기 |
| --- | --- |
| RHEL 8<br>RHEL 9 | Ubuntu 22.04 |

## 일반 권장 사항

UV 타일 워크플로우를 사용할 때 좋은 성능을 얻으려면 다음을 사용하는 것이 좋습니다.

* 32GB RAM
* VRAM 8GB 지원 GPU
* SSD는 프로젝트와 애플리케이션 캐시를 모두 저장합니다.

기타 사항:

* 대부분의 Substance 앱은 RHEL8/9 호환을 위해 OpenSSL 1.1.1을 사용합니다. 최신 OpenSSL 버전을 사용하는 시스템의 경우 고객은 수동으로 제공해야 합니다
* 편안한 환경에서 작업하려면 수직 해상도가 1000픽셀 이상, 1280픽셀 이상인 모니터를 사용하는 것이 좋습니다.
* **8K**(8192\*8192픽셀)에서 내보내려면 2GB의 VRam이 **개**&#x200B;이상 포함된 GPU가 필요합니다.
* macOS 10.15(Catalina)에서 실행하기 위해 2019.x 이상 버전만 공증되었습니다.
* RDP(원격 데스크톱)를 통해 소프트웨어를 사용하려면 전용 [설명서 페이지](../pipeline-and-integration/configuration/remote-desktop.md)를 참조하십시오.
* 베이킹 시 Ryzen CPU의 충돌은 BIOS를 업데이트하여 해결할 수 있습니다.

## 지원되지 않는 구성

**Windows**

* 가상 컴퓨터가 지원되지 않습니다.
* Windows Server가 지원되지 않습니다.

**Mac**

* 공식 Apple 구성만 지원됩니다.
* eGPU는 현재 지원되지 않으며 안정성 문제가 있을 수 있습니다.

**Linux**

* Linux의 Mesa 드라이버는 지원되지 않습니다.

**모든 플랫폼**

* 통합 GPU는 x86-64(Intel, AMD) CPU에서 지원되지 않습니다.

## 최소 GPU 드라이버 버전

다음은 응용 프로그램을 문제 없이 실행하는 데 필요한 최소 GPU 드라이버 버전 목록입니다. 이 목록은 새 버전이 출시될 때마다 변경될 수 있습니다.

새 드라이버를 다운로드하려면 [GPU에 오래된 드라이버가 있음](../technical-support/technical-issues/gpu-issues/gpu-has-outdated-drivers.md)을 참조하십시오.

| OS | NVIDIA | AMD | Intel |
| --- | --- | --- | --- |
| **Windows** | GeForce 442.50 Quadro 442.50 | Radeon 19.7.1 Radeon Pro / FirePro 18.Q4 | 15.33 |
| **Linux** | 535.171.04 이상 | Radeon 22.40.6 | 지원되지 않음 |

>[!NOTE]
>
> **Mac OS**&#x200B;에서 GPU 드라이버는 운영 체제에서 제공됩니다. 최신 드라이버에 액세스하려면 최신 버전의 OS로 업데이트하십시오.

### 드라이버 호환성 문제

생성자당 GPU 드라이버 문제의 자세한 목록은 [전용 문서 페이지](../technical-support/technical-issues/gpu-issues/gpu-drivers-compatibility.md)를 살펴보십시오.

## 베이킹용 GPU 광선 추적

Optix 또는 DXR을 통해 GPU 광선 추적을 활성화하려면 위에 권장되는 최소 드라이버를 설치해야 합니다.

**DXR**&#x200B;에는 다음과 같은 최소 구성도 필요합니다.

* **Windows 10** 버전 1809에서 자세한 내용은 [이 페이지](https://experienceleague.adobe.com/en/docs/substance-3d/bakers/features/gpu-raytracing)를 참조하세요.
* **Pascal 아키텍처의 GPU**(Nvidia GeForce 10XX)

>[!TIP]
>
> GPU 광선 추적은 NVIDIA GeForce RTX 또는 NVIDIA Quadro RTX GPU와 같은 전용 광선 추적 하드웨어에서 최적으로 실행됩니다.

## 지원되는 그래픽 태블릿

다음은 Substance 3D Painter 버전 **7.4.2**&#x200B;에서 테스트된 호환되는 그래픽 태블릿 목록입니다.

+++Wacom

**모델:** Intuos Pro(M 크기), Intuos(S 크기)

| OS | 드라이버 버전 |
| --- | --- |
| Windows | 6.3.45-1 |
| macOS | 6.3.45-3 |

+++

+++XPen

**모델:** 데코 01

| OS | 드라이버 버전 |
| --- | --- |
| Windows | XP-PENWin_3.2.2.211027 |
| macOS | XP-PENMac_3.2.3_211203 |
| 리눅스 | XP-PEN-PENTABLET-3.2.1.211019-1 |

+++

+++후이온

**모델:** Q11K

| OS | 드라이버 버전 |
| --- | --- |
| Windows | XP-PENWin_3.2.2.211027 |
| macOS | XP-PENMac_3.2.3_211203 |

+++

+++Xencelabs

**모델:** 펜 태블릿 보통

| OS | 드라이버 버전 |
| --- | --- |
| Windows | XencelabsWin_1.2.1-14 |
| macOS | XencelabsMac_1.2.1-18 |
| 리눅스 | XencelabsLinux_1.1.0-2 |

+++

## 지원되는 3Dconnection SpaceMouse 모델

다음은 Substance 3D Painter 버전 **8.1.**&#x200B;에서 테스트된 [3Dconnection Space Mouse](https://3dconnexion.com/us/spacemouse/)의 호환 가능한 드라이버 버전 목록입니다.

드라이버 버전은 **Compact**, **Pro** 및 **Enterprise** 모델에 적용됩니다.

| OS | 드라이버 버전 |
| --- | --- |
| Windows | 10.8.6.3431 |
| macOS | 10.7.2.3454 |

## 언어

소프트웨어 인터페이스는 다음 언어로 제공됩니다.

* 영어(미국)
* 독일어
* 스페인어
* 프랑스어
* 이탈리아어
* 일본어
* 한국어
* 포르투갈어(브라질)
* 중국어(간체)
