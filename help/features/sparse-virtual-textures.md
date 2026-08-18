---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/features/sparse-virtual-textures.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 스파스 가상 텍스처를 사용하여 초고해상도 텍스처를 사용하여 효율적으로 작업하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Features > Sparse Virtual Textures
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 스파스 가상 텍스처
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---


# 스파스 가상 텍스처

![](../assets/svt-header.jpg)

버전 **2018.3**&#x200B;부터 Substance 3D Painter은 실시간 뷰포트에서 **스파스 가상 텍스처**( **SVT**)를 사용하여 많은 양의 텍스처를 관리합니다. 이 기술을 사용하면 GPU 메모리에서 특정 풋프린트를 유지하기 위해 지정된 시점에서만 필요한 텍스처를 스트리밍 인/스트리밍 할 수 있습니다. 많은 양의 텍스처 세트(또는 UDIM)가 있는 프로젝트의 성능을 향상시킵니다.

## 지원되는 플랫폼

![](../assets/sparse-settings.png)

스파스 텍스처는 완전한 성능을 위해 특정 하드웨어 구성에 의존합니다. 현재 구성이 올바르게 지원하지 않는 경우 Substance 3D Painter은 대신 소프트웨어 구현에 **대체**&#x200B;합니다(정확도가 떨어지고 성능이 저하됨).

[설정](../interface/settings/settings.md) 로 이동하여 Substance 3D Painter에서 하드웨어 가속 대신 소프트웨어 폴백을 사용하도록 강제할 수 있습니다.

다음은 하드웨어 가속 스파스 가상 텍스처를 지원하는 구성입니다.

| 플랫폼 | 지원(하드웨어 가속) | 지원되지 않음(소프트웨어 대체) |
| --- | --- | --- |
| **Windows** | <ul data-preserve-html="true"><li data-preserve-html="true">Nvidia GeForce(드라이버 411.63 이상)</li><li data-preserve-html="true">Nvidia Quadro(드라이버 411.63 이상)</li><li data-preserve-html="true">AMD FirePro 및 Radeon Pro(드라이버 18.9.3 이상) <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon(드라이버 18.9.3 이상)&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true"> Nvidia Quadro M2000 </li><li data-preserve-html="true">  Nvidia Geforce GTX 970 </li><li data-preserve-html="true"> Intel GPU </li></ul> |
| **Mac OS** | <ul data-preserve-html="true"><li data-preserve-html="true"> 운영 체제에서 하드웨어 기능을 지원하지 않음 </li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">모든 GPU 모델</li></ul> |
| **Linux** | <ul data-preserve-html="true"><li data-preserve-html="true">Nvidia GeForce(드라이버 410.73 이상)</li><li data-preserve-html="true">Nvidia Quadro(드라이버 410.73 이상)</li><li data-preserve-html="true">AMD FirePro 및 Radeon Pro(드라이버 18.9.3 이상) <strong> &#42; </strong></li><li data-preserve-html="true">AMD Radeon(드라이버 18.9.3 이상)&#42;</li></ul> | <ul data-preserve-html="true"><li data-preserve-html="true">Intel GPU</li></ul> |


* **\*** : 기본적으로 사용하지 않도록 설정된 하드웨어 가속은 [설정](../interface/settings/settings.md)에서 수동으로 사용하도록 설정할 수 있습니다.

## Substance 3D Painter에서 스파스 가상 텍스처를 사용하는 이유는 무엇입니까?

Substance 3D Painter은 뷰포트에 표시되는 텍스처를 계산하기 위해 기본 엔진을 사용합니다. 즉, 엔진과 뷰포트가 이러한 텍스처를 계산하고 표시하기 위한 GPU 메모리(VRam)를 공유해야 합니다. 프로젝트에 **텍스처 집합**(또는 UV 타일)이 많을수록 뷰포트에 더 많은 메모리가 필요합니다. 뷰포트에 GPU의 메모리가 너무 많이 사용되는 경우 주 엔진이 텍스처를 계산할 공간이 충분하지 않아 시스템 메모리(Ram)로 텍스처를 추출해야 합니다. 이로 인해 성능이 저하되고 계산이 느려질 것이다.

SVT의 목표는 메인 엔진이 계산을 수행할 수 있는 공간을 최대한 많이 확보하면서 뷰포트가 GPU 메모리에서 사용할 수 있는 양을 예산으로 책정하는 것입니다. 이 시스템의 장점은 훨씬 더 큰 프로젝트를 Substance 3D Painter에 로드할 수 있는 기능을 잠금 해제하고 정상적으로 작업할 수 있다는 것입니다.

## 스파스 텍스처는 어떻게 작동하나요?

Sparse Virtual Textures는 완료되지 않은 텍스처의 유형입니다. 즉, 애플리케이션에서 텍스처의 일부만 메모리에 로드합니다. 필요한 것만 로드하고 나머지는 시스템 메모리나 디스크(캐시)에 넣습니다. 다시 필요한 경우 캐시에서 텍스처를 읽어들여 뷰포트에 다시 배치합니다. 전송을 충분히 빠르게 하기 위해 시스템은 **밉맵**&#x200B;을 사용하여 다른 텍스처 해상도 사이를 빠르게 이동합니다. 이 때문에 뷰포트로 빠르게 이동하면 처음에 흐릿한 텍스처가 표시되고 몇 초 후에 품질이 향상될 수 있습니다.

자세한 기술 정보는 [스파스 가상 텍스처](https://silverspaceship.com/src/svt/) 를 참조하십시오.

## 캐시 위치

![](../assets/settings-temp.png)

SVT 캐시를 저장할 수 있는 시스템 메모리(Ram)가 충분하지 않으면 Substance 3D Painter이 캐시를 저장하는 대신 컴퓨터 하드 드라이브로 전환됩니다.\
이 캐시의 위치는 기본적으로 운영 체제 임시 파일 폴더로 이동합니다. 응용 프로그램의 기본 설정으로 이동하여 이 위치를 변경할 수 있습니다. [일반 환경 설정](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/general-71008262.html) 을 참조하세요.

## 셰이더 호환성

SVT를 최대한 활용하기 위해 Shaders는 Sparse 시스템에서 텍스처를 요청하고 읽어야 합니다. 따라서 **vec2 텍스처 좌표** 및 **샘플러**&#x200B;에 기반한 이전 함수는 사용되지 않습니다. 이제 스파스 텍스처를 사용하기 위해 도우미 함수가 대신 제공됩니다.

셰이더를 업데이트하려면:

* **기본 Substance 3D Painter 셰이더**&#x200B;의 경우: [셰이더 업데이트](../interface/shader-settings/updating-a-shader.md) 페이지의 단계별 절차를 따르십시오.
* **사용자 지정 셰이더**&#x200B;의 경우: 로그의 오류 메시지와 [셰이더 API](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html) 페이지를 확인합니다.

>[!WARNING]
>
> 이전 프로젝트의 셰이더가 최신 버전이 아닌 경우 흰색 섬광이 표시될 수 있습니다. 자세한 내용은 이 페이지 [카메라를 이동할 때 플래시가 흰색으로 바뀜](../technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.md)을 참조하십시오.
