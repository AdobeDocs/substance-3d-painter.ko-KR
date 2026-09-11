---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/error-with-missing-api-ms-crt-dll.html"
breadcrumb-title: ''
description: 적절한 Windows 런타임 라이브러리 지원을 위해 Substance 3D Painter에서 누락된 api-ms-crt DLL 오류를 해결하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Error with missing api-ms-crt dll
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: api-ms-crt dll 누락 오류
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# api-ms-crt dll 누락 오류

컴퓨터에 **api-ms-win-crt-runtime-l1-1-0.dll**&#x200B;이(가) 없기 때문에 Substance 3D Painter을 시작할 수 없습니다.\
이는 Visual Studio 2015용 **Visual C++ 재배포 가능**&#x200B;에 포함된 업데이트 KB2999226을 설치하지 못했기 때문일 수 있습니다.

## 문제를 해결하는 방법

### 1 - Windows가 최신 상태인지 확인

1. 시작 메뉴 열기
1. 제어판 선택
1. **Windows 업데이트**&#x200B;를 클릭합니다.
1. **업데이트 확인**&#x200B;을 클릭합니다.
1. 사용 가능한 모든 업데이트를 **설치**&#x200B;합니다.
1. 업데이트를 설치한 후 컴퓨터를 **다시 시작**&#x200B;합니다.

다시 시작한 후 더 이상 업데이트를 사용할 수 없을 때까지 위의 단계를 다시 반복합니다.

### 2 - Visual C++ 재배포 가능 패키지 설치

1. Visual C++ 재배포 가능 패키지 다운로드 :
   1. [Windows 64비트](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x64.exe)용
   1. [Windows 32비트](http://download.microsoft.com/download/9/3/F/93FCF1E7-E6A4-478B-96E7-D4B285925B00/vc_redist.x86.exe)용
1. **vcredist\_x64.exe**(64비트) 또는 **vcredist\_x86.exe**(32비트)를 실행합니다.
1. 제거 를 선택하고 다음 절차를 따르십시오
1. 실행 파일을 다시 실행합니다.
1. 설치 를 선택합니다
