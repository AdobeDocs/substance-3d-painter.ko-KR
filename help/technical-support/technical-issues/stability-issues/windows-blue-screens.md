---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/technical-issues/stability-issues/windows-blue-screens.html"
breadcrumb-title: ''
description: 안정적인 시스템 운영을 위해 Substance 3D Painter을 사용할 때 Windows 블루 스크린 오류를 방지하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Windows Blue Screens
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Windows 블루 스크린
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---


# Windows 블루 스크린

Windows [BSOD(Blue Screens Of Death)](https://en.wikipedia.org/wiki/Blue_screen_of_death)에서는 일반적으로 드라이버 또는 하드웨어 오작동과 관련이 있습니다. Substance 3D Painter은 이러한 BSOD에 대해 책임을 지지 않지만, 애플리케이션의 집약성 때문에 컴퓨터 자체의 문제에 약간의 빛을 줄 수 있습니다. Substance 3D Painter의 경우 다음과 같은 문제로 인해 BSOD가 발생할 수 있습니다.

## 불안정한 GPU 드라이버

Substance 3D Painter은 다양한 계산을 수행하기 위해 GPU에 많이 의존합니다. GPU 드라이버가 불안정하거나 회귀될 수 있습니다. 최신 수정 사항 및 성능 개선을 얻으려면 GPU를 최신 상태로 유지하는 것이 좋습니다. 참조: [GPU에 오래된 드라이버가 있음](../gpu-issues/gpu-has-outdated-drivers.md).

### 불안정한 Windows 설치

일부 업데이트 후 Windows 자체가 불안정할 수 있습니다. Windows와 함께 제공되는 진단 도구를 사용하여 시스템에서 잠재적인 오류를 감지합니다.

**배포 이미지 서비스 및 관리**(DISM) 및 **시스템 파일 검사기**(SFC) 도구를 실행하는 것이 좋습니다. DISM은 손상되거나 누락 된 시스템 파일을 수정하기 위해 SFC에 필요한 대체 파일을 복구하는 데 유용합니다.

**DISM** 실행 중:

1. **시작 메뉴** 열기
1. **명령 프롬프트** 검색
1. **결과를 마우스 오른쪽 단추로 클릭**&#x200B;하고 &quot; **관리자 권한으로 실행** &quot;을(를) 선택합니다.
1. 다음 명령을 입력합니다. **DISM /Online /Cleanup-Image /RestoreHealth**
1. **Enter** 누르기

**SFC** 실행 중:

1. **시작 메뉴** 열기
1. **명령 프롬프트** 검색
1. **결과를 마우스 오른쪽 단추로 클릭**&#x200B;하고 &quot; **관리자 권한으로 실행** &quot;을(를) 선택합니다.
1. 다음 명령을 입력하십시오. **sfc /scannow**
1. **Enter** 누르기

두 명령 모두 업데이트 적용 후 컴퓨터를 다시 시작합니다.

이 제목에 대한 자세한 내용은 [시스템 파일 검사기 도구를 사용하여 누락 또는 손상된 시스템 파일 복구](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system)를 참조하십시오.

### 디스크 공간 부족

Substance 3D Painter에 [스파스 가상 텍스처](../../../features/sparse-virtual-textures.md)가 도입되었기 때문에 응용 프로그램은 이제 작업 중에 디스크를 사용하여 텍스처를 캐시합니다. 시스템의 공간이 부족하면 불안정해질 수 있다.

이 문제에 대한 두 가지 간단한 해결 방법이 있습니다.

* 캐시 시스템에 더 많은 공간을 확보하기 위해 디스크의 일부 공간을 비웁니다.
* 캐시 디렉터리를 공간이 더 많은 다른 드라이브로 이동합니다. 이 위치는 응용 프로그램의 기본 설정으로 이동하여 변경할 수 있습니다. [&quot;임시 파일&quot; 설정](https://docs.substance3d.com/display/SPDOC/General)을 참조하세요.

### 결함이 있는 디스크(HDD 또는 SSD)

이전 시점에서 언급했듯이 캐시 시스템은 디스크에 크게 의존합니다. 디스크 드라이브에 결함이 있으면 데이터를 쓰거나 읽을 때 시스템이 불안정해질 수 있습니다.

디스크에 결함이 있는지 검사하려면 Windows에서 CHKDSK를 실행합니다.

1. **별모양 메뉴** 열기
1. **컴퓨터/이 PC** 선택
1. 하드 드라이브에서 **마우스 오른쪽 단추**&#x200B;를 클릭하고 **속성**&#x200B;을 선택합니다.
1. **도구** 탭으로 전환합니다.
1. **오류 검사** 아래의 **지금 검사/확인**&#x200B;을 클릭합니다.

### 잘못된 메모리

프로그램이 메모리를 안전하게 읽거나 쓸 수 없는 경우 메모리(RAM)가 잘못되면 시스템이 불안정해질 수 있습니다. 메모리 무결성을 확인하려면 **MemTest**&#x200B;을(를) 실행하는 것이 좋습니다.

MemTest를 설치하고 사용하는 방법은 [이 가이드](https://www.memtest86.com/technical.htm)를 참조하십시오.
