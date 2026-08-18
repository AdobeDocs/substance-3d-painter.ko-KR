---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/installation-and-preferences/retrieving-the-installation-path.html"
breadcrumb-title: ''
description: 스크립팅 및 파이프라인 통합을 위해 Substance 3D Painter의 설치 경로를 검색하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Retrieving the installation path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 설치 경로 검색
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 5%

---


# 설치 경로 검색

이 페이지에서는 버전 및 플랫폼에 따라 애플리케이션의 설치 경로를 검색하는 방법에 대한 정보를 다시 그룹화합니다.

## Windows

### Creative Cloud 데스크톱

1. Windows 레지스트리 편집기(**regedit**)를 엽니다.
1. 레지스트리 키로 이동합니다. ** HKEY\_LOCAL\_MACHINE\Software\Microsoft\Windows\CurrentVersion\App 경로\**
1. 이름이 **Adobe Substance 3D Painter.exe**&#x200B;인 하위 키를 엽니다.
1. 키 값에는 키가 설치된 응용 프로그램 실행 파일의 경로가 포함됩니다

>[!NOTE]
>
> 이 레지스트리 키는 버전 7.2 이후에만 사용할 수 있습니다.\
>  이전 버전의 경우 **HKEY\_CURRENT\_USER\Software\Microsoft\Windows\CurrentVersion\ Explorer\FileExts**&#x200B;의 파일 연결에서 설치 경로를 검색할 수 있습니다.

### Substance 3D Standalone

1. Windows 레지스트리 편집기(**regedit**)를 엽니다.
1. 레지스트리 키로 이동합니다. **HKEY\_LOCAL\_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall**
1. 애플리케이션 버전의 AppID와 일치하는 하위 키를 찾습니다(아래 표 참조).
1. 키 값에는 응용 프로그램 설치 위치에 대한 경로가 포함됩니다

| 버전 | AppId |
| --- | --- |
| **버전 1.x** | `{410F5B6E-A29C-4F43-9DE3-44A1357D6AF5}` |
| **버전 2.x** | `{f42b7a996fa1d13a1d0a2e33eea2c0800bb5d1b8}` |
| **3.x(2017.x) ~ 7.1** | `{33C3E9E2-0675-4196-9019-28AB9C5E9BB0}` |
| **7.2 이상** | `{2a8bbb68-725b-477c-9194-60efc5ece348}` |

### 증기

Steam 설치 폴더의 **steamapps/common/** 하위 폴더에 응용 프로그램이 설치되어 있습니다.

## Mac

Mac에서 애플리케이션은 다음 위치에 설치됩니다.

| 버전 | 경로 |
| --- | --- |
| **7.2 이상** | **/Applications/Adobe Substance 3D Painter.app** |
| **레거시** | **/Applications/Substance Painter.app** |

## 리눅스

Linux에서 rpm 패키지는 다음 경로에 설치됩니다.

| 버전 | 경로 |
| --- | --- |
| **7.2 이상** | **/opt/Adobe/Adobe\_Substance\_3D\_Painter** |
| **레거시** | **/opt/Allegorithmic/Substance\_Painter** |
