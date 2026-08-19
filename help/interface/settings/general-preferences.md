---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/interface/settings/general-preferences.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 일반 환경 설정을 구성하여 응용 프로그램 동작 및 사용자 경험을 사용자 정의하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Interface > Settings > General preferences
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 일반 환경 설정
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 1%

---


# 일반 환경 설정

![](../../assets/settings-general_1.png)

이 페이지에서는 응용 프로그램의 기본 설정을 설명합니다.

## 인터페이스 옵션

![](../../assets/settings-interface.png)

| 설정 | 설명 |
| --- | --- |
| **언어** | 응용 프로그램에서 인터페이스에 사용되는 언어를 정의합니다. 이 설정을 적용하려면 응용 프로그램을 다시 시작해야 합니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>기본(시스템 언어)</strong>: 운영 체제에서 호환되는 언어를 검색합니다.</li><li data-preserve-html="true"><strong>영어</strong></li><li data-preserve-html="true"><strong>독일어</strong></li><li data-preserve-html="true"><strong>프랑스어</strong></li><li data-preserve-html="true"><strong>일본어</strong></li><li data-preserve-html="true"><strong>중국어</strong>(간체)</li></ul> |
| **키보드 도우미 표시** | 활성화한 경우 키를 누를 때(예: CTRL 또는 SHIFT) 뷰포트의 왼쪽 하단에 키보드 단축키를 표시합니다. |
| **세계 축 표시** | 활성화하면 세계 축이 3D 보기의 오른쪽 하단에 표시됩니다. |
| **배경색** | 뷰포트의 배경으로 사용되는 색상을 선택합니다. 두 가지 색상을 사용하여 그라디언트를 만들 수 있습니다. |
| **페인팅할 때 선택한 재질만 표시** | 이 옵션을 활성화하면 현재 선택한 [텍스처 세트]만 3D 보기에서 페인팅하여 다른 [텍스처 세트]를 일시적으로 숨깁니다.  **참고:** 뷰포트에서 빠르게 보기를 변경하면 [스파스 가상 텍스처](../../features/sparse-virtual-textures.md)의 성능에 영향을 줄 수 있으므로 이 설정을 사용하지 않는 것이 좋습니다. |
| **뷰포트 비율** | HDPI/Retina 화면에 대한 뷰포트의 해상도를 줄여 성능을 향상시킬 수 있습니다.가능한 값:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>없음</strong>: 비율 조정이 없으며 뷰포트가 기본 화면 해상도로 렌더링됩니다.</li><li data-preserve-html="true"><strong>자동</strong>: 화면 해상도를 2로 나눕니다(HDPI 화면에서만).</li></ul> |

## 레이어 스택 옵션

![](../../assets/settings-layerstack.png)

| 설정 | 설명 |
| --- | --- |
| **기본 재질 UV 비율** | 재질을 적용할 때 레이어 스택의 칠 레이어 및 칠 효과에 대한 기본 타일링/반복 값을 정의합니다. |
| **단순화된 축소판 사용** | 활성화되면 썸네일을 계산하는 대신 레이어 스택에 아이콘만 표시됩니다. 아이콘을 사용하면 성능이 향상됩니다. UV 타일 워크플로우를 사용하는 프로젝트에는 항상 아이콘이 표시되므로 이 설정은 적용되지 않습니다. |

## 카메라 옵션

![](../../assets/settings-camera.png)

| 설정 | 설명 |
| --- | --- |
| **회전 속도** | 뷰포트에서 카메라의 기본 회전 속도의 승수입니다. |
| **확대/축소 속도** | 뷰포트에서 카메라의 기본 확대/축소 속도의 승수입니다.역방향을 사용하면 마우스 움직임에 따라 확대/축소 방향을 반전할 수 있습니다. |
| **휠 속도** | 마우스 휠의 확대/축소 속도에 대한 승수입니다.역방향은 휠 움직임을 기반으로 확대/축소 방향을 반전할 수 있습니다. |

## 베이킹 옵션

![](../../assets/settings-baking.png)

| 설정 | 설명 |
| --- | --- |
| **사전 처리된 장면 파일 저장** | 활성화되면 베이커가 사용하는 사전 처리된 고-폴리 메시가 향후 재사용을 위해 디스크에 저장됩니다. 이 설정을 사용하면 더 빠르게 다시 굽을 수 있습니다. |
| **실시간 미리 보기 굽기 프로세스 사용** | 활성화되면 3D 및 2D 뷰포트에 메시에서 계산되고 있는 현재 베이커 텍스처가 표시됩니다. |
| **GPU 광선 추적 사용** | 활성화되면 베이커는 CPU 대신 광선 추적을 수행하기 위해 GPU를 사용하려고 합니다. 이 기능을 통해 제빵사는 전반적으로 더 빠른 작업을 수행할 수 있습니다.호환되는 하드웨어에서만 활성화할 수 있습니다. 자세한 내용은 [시스템 요구 사항](../../getting-started/system-requirements.md)을 참조하세요. |

## 미리 보기 옵션

![](../../assets/settings-preview.png)

| 설정 | 설명 |
| --- | --- |
| **로컬 캐시 디렉터리** | 리소스 축소판이 생성될 때 있을 보조 위치를 정의합니다.이 설정은 리소스 경로가 읽기 전용인 경우(읽기 액세스만 있는 네트워크 경로에서와 마찬가지로) 리소스 축소판을 계산하고 저장하는 데 유용합니다. 이렇게 하면 축소판이 디스크에 저장되지 않으므로 시작할 때마다 축소판을 다시 계산하지 않습니다. |
| **로컬 캐시 예산(MB)** | 로컬 캐시에 대한 캐시의 최대 크기를 정의합니다. |
| **재질 미리 보기 셰이더** | 셸프에 재료 축소판을 생성하는 데 사용할 셰이더를 정의합니다. 이는 리소스가 기본 셰이더와 다른 워크플로를 사용하는 경우 유용합니다. 이 설정을 적용하려면 응용 프로그램을 다시 시작해야 합니다. |

## 임시 파일

![](../../assets/settings-temp-1.png)

| 설정 | 설명 |
| --- | --- |
| **캐시 디렉터리** | 임시 파일이 기록되는 위치를 정의합니다. 여기에는 [스파스 가상 텍스처](../../features/sparse-virtual-textures.md) 캐시가 포함됩니다. 이 설정은 [환경 변수](../../pipeline-and-integration/configuration/environment-variables.md)로 재정의할 수 있습니다. |

## 스파스 가상 텍스처

![](../../assets/settings-sparse.png)

| 설정 | 설명 |
| --- | --- |
| **하드웨어 지원 가속** | 활성화되면 애플리케이션은 GPU와 함께 스파스 텍스처를 사용하려고 합니다. 자세한 내용은 [스파스 가상 텍스처](../../features/sparse-virtual-textures.md) 페이지를 참조하십시오. 이 설정은 [환경 변수](../../pipeline-and-integration/configuration/environment-variables.md)로 재정의할 수 있습니다. |

## Iray 하드웨어

![](../../assets/settings-iray.png)

이 섹션에는 Iray로 렌더링할 때 사용할 수 있는 모든 호환 하드웨어가 나열됩니다.

CPU 설정은 모든 컴퓨터에서 사용할 수 있습니다. 컴퓨터에 CUDA 호환 버전이 있는 **Nvidia GPU**&#x200B;가 있는 경우 여기에 나열됩니다.

>[!NOTE]
>
> 최상의 렌더링 성능을 보장하기 위해 CPU를 비활성화하고 GPU 하드웨어만 활성화하는 것이 좋습니다. CPU와 GPU를 함께 활성화하면 렌더링 시간이 늘어날 수 있습니다.

## 개인 정보 보호

![](../../assets/settings-privacy.png)

| 설정 | 설명 |
| --- | --- |
| **사용 통계 자동 전송** | 활성화되면 컴퓨터 하드웨어 구성에 대한 정보를 다른 사용 데이터와 함께 익명으로 전송합니다. 이러한 데이터는 소프트웨어를 개발하고 개선하는 데 도움이 됩니다. |
