---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/startup-issues/software-conflicts.html"
breadcrumb-title: ''
description: 시스템에서 Substance 3D Painter이 제대로 시작되지 않도록 하는 소프트웨어 충돌을 해결하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Software conflicts
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 소프트웨어 충돌
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---


# 소프트웨어 충돌

이 페이지에는 Substance 3D Painter 실행이 올바르게 실행되지 않도록 충돌 또는 중지할 수 있는 기타 소프트웨어 관련 알려진 문제 목록이 포함되어 있습니다.

| *잠재적 충돌 원본* | *문제* |
| --- | --- |
| **안티바이러스/안티스파이웨어** | 안티바이러스 또는 안티스파이웨어 소프트웨어는 다음과 같은 문제를 일으킬 수 있습니다.<ul data-preserve-html="true"> <li data-preserve-html="true"><b> False positive</b>: Painter이 바이러스 또는 맬웨어로 잘못 플래그 지정되었습니다.</li> <li data-preserve-html="true"><b> 차단된 파일</b>: Painter에서 파일을 읽거나 쓸 수 없습니다(내보내기, 사전 설정 생성 등).</li> <li data-preserve-html="true"><b> 파일 삭제</b>: 필요한 파일이 제거되었으므로 Painter을 시작하거나 정상적으로 작업할 수 없습니다.</li> </ul>이러한 상황 중 하나가 발생하는 경우 안티바이러스를 일시적으로 비활성화하여 도움이 되는지 확인하거나 Painter에 대한 예외를 수동으로 추가하는 것이 좋습니다. |
| **AMD CrossFire 및 NVIDIA SLI** | Painter에서 다중 GPU 구성을 지원하지 않아 충돌이 발생합니다. 이 기능을 비활성화하는 것이 좋습니다. |
| <b> Autodesk 도우미 </b> | Autodesk 길잡이 응용 프로그램은 충돌을 일으키고 시작 시 또는 프로젝트 파일을 열 때 응용 프로그램을 충돌 상태로 만들 수 있습니다. Autodesk 응용 프로그램을 업데이트하여 문제를 해결합니다. |
| Alienware/Dell 컴퓨터 <b>대</b> | 자세한 내용은 [파일을 열거나 저장할 때 충돌](../stability-issues/crash-when-opening-or-saving-a-file.md) 페이지를 참조하십시오. |
| **Paragon Software의 APFS** | 이 소프트웨어는 시작할 때 응용 프로그램을 충돌 할 수 있는 위치를 Windows 경로 환경 변수에 등록할 수 있습니다. 소프트웨어를 제거하기에 충분하지 않을 수 있으며 환경 변수를 수동으로 제거해야 할 수 있습니다. 문제가 있는 위치의 예: `C:Program Files (x86)Paragon SoftwareAPFS for Windowsï–›éŒ à €è¸€ì‡ì‡ç¿¹` |
| **Avecto** | 이전 버전의 Avecto를 실행하면 성능 저하와 충돌이 발생할 수 있습니다. 최신 버전으로 업데이트해야 합니다. |
| **Asus GPU Tweak** | 이 소프트웨어를 사용하면 Substance 3D Painter 내에서 셰이더를 컴파일하는 동안 문제가 발생하거나 셰이더 컴파일이 시작되지 않을 수도 있습니다. 이 문제가 발생하면 소프트웨어를 제거하여 문제가 해결되는지 확인하는 것이 좋습니다. |
| **아수스 RAMCache** | 이 소프트웨어는 Substance 3D Painter이 제대로 실행되지 않거나 실행 중 불안정하게 만들 수 있습니다. 안정성 문제가 있는 경우 Asus RAMCache를 비활성화하거나 설치하는 것이 좋습니다. |
| **에이수스 소닉 스위트** | ASUS 마더보드가 있는 컴퓨터에서는 <b>Asus Sonic Suite</b>를 기본적으로 설치할 수 있습니다. 이 소프트웨어를 제거하면 Substance 3D Painter의 일부 디스플레이/인터페이스 문제가 해결될 수 있습니다. |
| **클라우드 백업 소프트웨어** **(** OneDrive,**GDrive,** **Dropbox,** **Filestream 등)** | 클라우드 백업 소프트웨어는 프로젝트를 저장하는 동안 수많은 충돌의 소스가 될 수 있습니다. 이 경우 프로젝트 파일을 작업하여 동기화되지 않은 폴더에 저장하는 것이 좋으며, 대신 변경 사항이 더 이상 적용되지 않으면 프로젝트 파일을 클라우드 드라이브에 다시 복사하는 것이 좋습니다. |
| **Chitubox** | 이 소프트웨어는 파일 대화 상자를 열 때(프로젝트 열기 또는 저장 등) 충돌을 생성하고 응용 프로그램을 충돌 할 수 있습니다. 이 문제를 방지하려면 Chitubox 환경 설정에서 <b>데스크탑 모델의 축소판 미리 보기 활성화</b> 설정을 비활성화할 수 있습니다. |
| **듀엣 표시** | <b>듀엣 표시</b>는 Substance 3D Painter 동작에 영향을 줄 수 있는 GPU 드라이버 문제를 만드는 것으로 알려져 있습니다. 제거하는 것이 좋습니다. |
| **Google Chrome** | Google Chrome을 사용하면 Substance 3D Painter과 함께 실행할 때 일부 충돌이 발생할 수 있습니다. Substance 3D Painter의 안정성을 개선하려면 Google Chrome 및 GPU 드라이버를 업데이트하는 것이 좋습니다. 충돌이 계속 발생하면 Google Chrome에서 하드웨어 가속을 비활성화하십시오(Chrome의 GPU 사용 중단). |
| **나히믹 오디오 소프트웨어** | <b>나히믹</b>은 Painter을 멈추거나 충돌 할 수 있습니다. 이를 중지하면 도움이 되고, 업데이트하면 문제가 발생하지 않습니다. Nahimic은 애플리케이션을 방해할 수 있으며 중단하거나 비활성화해야 할 수 있는 백그라운드 서비스도 실행합니다. |
| **Openshot 비디오 소프트웨어** | <b>Openshot 비디오 소프트웨어</b>는 선반의 미리 보기로 Substance 3D Painter과 충돌을 일으킬 수 있습니다. Openshot을 업데이트하면 문제가 해결됩니다. |
| **설치 관리자** | 이 응용 프로그램에서 환경 설정이 잘못되어 시작 시 오류가 발생할 수 있습니다. 자세한 내용은 [Qt](application-failed-to-start-because-of-qt.md) 때문에 응용 프로그램을 시작하지 못했습니다. |
| **Rptr / Plays.tv** | 일부 GPU 드라이버에서는 기본적으로 <b>Rptr</b>(또는 <b>[Plays.tv](http://plays.tv/) </b>)이(가) 설치됩니다. 이 소프트웨어는 불안정을 만들고 응용 프로그램을 충돌 할 수 있습니다. 응용 프로그램을 제거하는 것이 좋습니다. |
| **RGBFusion** | 이 소프트웨어는 그래픽 태블릿 드라이버와 충돌을 일으킬 수 있으며, 프로세스를 중지하면 문제를 일시적으로 해결할 수 있습니다 또는 영구 수정을 위해 RGBFusion 제거. |
