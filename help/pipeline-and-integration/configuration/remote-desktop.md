---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/pipeline-and-integration/configuration/remote-desktop.html"
breadcrumb-title: ''
description: 원격 작업 과정 및 공동 작업을 활성화하기 위해 원격 데스크톱 액세스용 Substance 3D Painter을 구성하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Remote Desktop
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 원격 데스크톱
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---


# 원격 데스크톱

이 페이지에서는 Substance 3D Painter을 Windows에서 원격 데스크탑(RDP)을 통해 실행할 수 있도록 하는 솔루션과 대안에 대해 설명합니다.

기본적으로 Windows의 RDP는 존재하지 않거나 너무 낮은 OpenGL 컨텍스트에서 실행되어 응용 프로그램이 제대로 작동하지 않거나 충돌합니다. Substance 3D Painter에는 OpenGL 3.3 컨텍스트가 필요합니다. 다음은 문제를 완화할 수 있는 해결책이지만 초기 문제가 Windows 및 일부 GPU 드라이버에 따라 달라지므로 작동되는 보장은 없습니다.

>[!NOTE]
>
> Nvidia Quadro GPU는 기본적으로 RDP 모드로 애플리케이션을 실행할 수 있지만 Nvidia GeForce GPU는 OpenGL 1.4 컨텍스트(Substance 3D Painter에 비해 너무 낮음)만 제공합니다. 이를 해결하기 위한 실행 파일을 설치할 수 있습니다. <https://developer.nvidia.com/designworks> 참조

## Windows 정책 구성

Windows 10에서는 RDP 모드에 있는 동안 GPU를 실행할 수 있도록 **그룹 정책**&#x200B;을 변경해야 할 수 있습니다.

이를 위해 다음을 수행합니다.

1. **Win + R**&#x200B;을 눌러 실행 창을 엽니다.
1. &quot; **gpedit.msc** &quot;을 입력한 다음 Enter 키를 누릅니다.
1. **로컬 컴퓨터 정책\컴퓨터 구성\관리 템플릿\Windows 구성 요소\원격 데스크톱 서비스\원격 데스크톱 세션 호스트\원격 세션 환경**(으)로 이동
1. **모든 원격 데스크톱 서비스 세션에 하드웨어 기본 그래픽 어댑터 사용** 옵션을 활성화합니다.

## Windows TSCON 명령

이전 정책 변경이 작동하지 않으면 **tscon** 명령줄을 사용해 보십시오. 이 명령은 원격 컴퓨터를 분리하고 새 컴퓨터를 물리적 하드웨어(마우스, 키보드 등)에 연결합니다. 그런 다음 간단히 응용 프로그램을 실행하고 원격으로 다시 연결하면 GPU에서 응용 프로그램으로 작업할 수 있습니다.

1. **Windows+R** 키를 눌러 **실행** 창을 엽니다.
1. **cmd**&#x200B;를 입력하고 **Enter** 키를 누릅니다.
1. 명령줄 유형 및 다음 명령: **tscon 1 /dest:console**
1. Enter 키를 누릅니다
1. 명령줄에 다음 명령을 입력합니다. **시작 &quot;Path/To/Path/Folder/Painter/Folder/Substance 3D Painter.exe&quot;**(컴퓨터와 일치하도록 경로를 변경해야 함)
1. Enter 키를 누릅니다

이 단계 후에 응용 프로그램이 시작되도록 잠시 기다렸다가 세션에 다시 연결합니다.

이 절차가 작동하지 않는 경우 관리자 모드에서 Windows 명령줄을 실행해야 할 수도 있습니다.

## 대안

이전 제안이 여전히 작동하지 않으면 원격 연결을 통해 GPU를 지원하는 VNC 또는 Teamviewer와 같은 대체 솔루션을 사용하는 것이 좋습니다.
