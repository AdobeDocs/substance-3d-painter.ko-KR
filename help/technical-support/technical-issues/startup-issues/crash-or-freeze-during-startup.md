---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/technical-issues/startup-issues/crash-or-freeze-during-startup.html"
breadcrumb-title: ''
description: 안정적인 애플리케이션 실행을 위해 Substance 3D Painter 시작 시 충돌과 작동 중지를 해결하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Crash or freeze during startup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 시작 중 충돌 또는 멈춤
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---


# 시작 중 충돌 또는 멈춤

이 페이지에는 응용 프로그램이 제대로 시작되지 않는 알려진 문제와 해결 방법이 나열되어 있습니다.

## 소프트웨어 충돌

충돌을 일으킬 수 있는 알려진 모든 소프트웨어 목록을 보려면 다음 페이지를 살펴보십시오. [소프트웨어 충돌](software-conflicts.md).

## 잘못된 GPU에서 실행 중

응용 프로그램이 올바른 GPU에서 시작되지 않으면 안정성 문제가 발생할 수 있습니다. 자세한 내용은 이 페이지를 참조하십시오. [Painter이 올바른 GPU에서 시작되지 않습니다](../gpu-issues/painter-doesn-t-start-on-the-right-gpu.md).

## 오래된 GPU 드라이버

이전 GPU 드라이버를 사용하면 정지 및/또는 충돌이 발생할 수 있습니다. 가능한 경우 최신 GPU 드라이버를 사용하는 것이 좋습니다. 참조: [GPU에 오래된 드라이버가 있음](../gpu-issues/gpu-has-outdated-drivers.md).

## 흰색 화면 및 응답하지 않음

Windows에서 시작할 때 애플리케이션이 바로 멈추면(흰색 화면으로 이어짐) 다음과 같은 몇 가지 이유가 있을 수 있습니다.

* 외부 응용 프로그램에서 충돌을 만들고 있습니다. 충돌을 확인하려면 [소프트웨어 충돌](software-conflicts.md)을 참조하세요.
* 응용 프로그램의 일부 창이 다른 모니터에서 열렸습니다. 인터페이스를 기본 레이아웃으로 복원하면 응용 프로그램을 정상적으로 시작할 수 있습니다.
  1. 시작 메뉴에서 레지스트리 편집기(**regedit**)를 엽니다.
  1. 응용 프로그램 기본 설정으로 이동합니다([기본 설정 및 응용 프로그램 데이터 위치](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html) 참조).
  1. **Adobe Substance 3D Painter** 키 확장
  1. **주 창 2018** 키를 선택하고 삭제합니다.
  1. 애플리케이션을 다시 시작합니다

## 잘못된 시스템 경로/Python 경로로 인해 충돌 발생

애플리케이션은 시스템 경로를 확인하여 Python 모듈과 환경 설정을 로드합니다. 시스템에 잘못된 설정이 있으면 시작하는 동안 충돌이 발생할 수 있습니다.

Windows에서:

1. **시작** 메뉴 열기
1. **시스템(제어판)** 검색 및 선택
1. **고급 시스템 설정**&#x200B;을 클릭합니다.
1. **환경 변수**&#x200B;를 클릭합니다.
1. **시스템 변수**&#x200B;에서 **PATH** 변수를 찾습니다.

그런 다음 변수를 편집하여 내용을 확인할 수 있습니다. 예를 들어 충돌에 다음과 같은 문자가 포함되어 있으면 변수가 생성됩니다

```
ï–›éŒ à €è¸€ì‡ì‡ç¿¹
```


## Windows 10 업데이트

Windows 10의 일부 업데이트는 때때로 불안정을 초래할 수 있습니다. Windows와 함께 제공되는 진단 도구를 사용하여 시스템에서 잠재적인 오류를 감지합니다.

**배포 이미지 서비스 및 관리**(DISM) 및 **시스템 파일 검사기**(SFC) 도구를 실행하는 것이 좋습니다. DISM은 손상되거나 누락 된 시스템 파일을 수정하기 위해 SFC에 필요한 대체 파일을 복구하는 데 유용합니다.

**DISM** 실행 중:

1. 시작 메뉴 열기
1. 명령 프롬프트 검색
1. 결과를 마우스 오른쪽 버튼으로 클릭하고 &quot;관리자로 실행&quot;을 선택합니다.
1. 다음 명령을 입력합니다. **DISM /Online /Cleanup-Image /RestoreHealth**
1. Enter 키를 누릅니다

**SFC** 실행 중:

1. 시작 메뉴 열기
1. 명령 프롬프트 검색
1. 결과를 마우스 오른쪽 버튼으로 클릭하고 &quot;관리자로 실행&quot;을 선택합니다.
1. 다음 명령을 입력하십시오. **sfc /scannow**
1. Enter 키를 누릅니다

두 명령 모두 업데이트 적용 후 컴퓨터를 다시 시작합니다.

이 제목에 대한 자세한 내용은 [시스템 파일 검사기 도구를 사용하여 누락 또는 손상된 시스템 파일을 복구하십시오](https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system).

## 이전 버전에서 시작할 때 충돌

Windows에서 설치 폴더와 함께 제공된 dll 파일 중 하나가 운영 체제에 비해 너무 오래되어 버전 2018(4.x) 이상이 시작되지 않을 수 있습니다. 이 충돌은 수동으로 파일을 최신 버전으로 대체하여 해결할 수 있습니다.

이를 위해 다음을 수행합니다.

1. Substance Painter 설치 폴더로 이동합니다.
1. <b>backup\_libeay32.dll</b>에서 <b>libeay32.dll</b> 파일의 이름을 바꿉니다.
1. [updated\_libeay32.zip](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/182266673/225968681/1/1644000679697/updated-libeay32.zip) 파일을 다운로드합니다.
1. zip 파일에서 dll 파일의 압축을 Substance Painter.exe 파일 옆에 있는 설치 폴더로 풉니다.
1. 애플리케이션을 시작합니다.
