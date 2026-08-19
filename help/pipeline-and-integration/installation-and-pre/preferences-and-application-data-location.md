---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/pipeline-and-integration/installation-and-preferences/preferences-and-application-data-location.html"
breadcrumb-title: ''
description: 설정 및 사용자 데이터를 관리하기 위한 Substance 3D Painter의 환경 설정 및 애플리케이션 데이터 위치에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Preferences and application data location
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 환경 설정 및 응용 프로그램 데이터 위치
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 4%

---


# 환경 설정 및 응용 프로그램 데이터 위치

이 페이지에서는 버전 및 플랫폼별로 응용 프로그램 환경설정이 저장되는 위치에 대한 정보를 다시 그룹화합니다.\
**사용자 지정 셸프**(스튜디오 설치용)를 추가하거나 이러한 환경 설정을 제거하여 응용 프로그램의 **깨끗한 설치**&#x200B;를 수행하려는 경우 환경 설정이 저장된 위치를 알고 있으면 유용합니다.

## 환경 설정

이 경로는 애플리케이션 환경 설정(저장된 단축키, 셸프/에셋 경로, 인터페이스 레이아웃 등)의 위치입니다.

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> </colgroup><tbody><tr><th>시스템</th><th>버전</th><th>경로</th></tr><tr><td rowspan="2"><p><strong>Windows</strong></p><p>(레지스트리)</p></td><td><strong>7.2</strong> 이상</td><td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td></tr><tr><td>레거시</td><td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><p><strong>Mac</strong></p><p>(라이브러리)</p></td><td><strong>7.2</strong> 이상</td><td>/Users/[사용자 이름]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td></tr><tr><td>레거시</td><td>/Users/[사용자 이름]/Library/Preferences/com.substance3d.Substance Painter.plist</td></tr><tr><td rowspan="2"><strong>리눅스</strong></td><td><strong>7.2</strong> 이상</td><td>/home/[사용자 이름]/.config/Adobe/Adobe Substance 3D Painter.conf</td></tr><tr><td>레거시</td><td>/home/[사용자 이름]/.config/Allegorithmic/Substance Painter.conf</td></tr></tbody></table>

## 응용 프로그램 데이터

이 경로는 추가 응용 프로그램 데이터(에셋 축소판, 로그 파일 등)의 위치입니다.

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> <col/> </colgroup><tbody><tr><th>플랫폼</th><th>버전</th><th colspan="2">경로</th></tr><tr><td rowspan="4"><strong>Windows</strong></td><td rowspan="2"><strong>7.2</strong> 이상</td><td colspan="1">앱 데이터(로컬)</td><td colspan="1">C:\Users\[사용자 이름]\AppData\Local\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">앱 데이터(로밍)</td><td colspan="1">C:\Users\[사용자 이름]\AppData\Roaming\Adobe\Adobe Substance 3D Painter</td></tr><tr><td rowspan="2">레거시</td><td colspan="1">앱 데이터(로컬)</td><td colspan="1">C:\Users\[사용자 이름]\AppData\Local\Allegorithmic\Substance Painter</td></tr><tr><td colspan="1">앱 데이터(로밍)</td><td colspan="1">C:\Users\[사용자 이름]\AppData\Roaming\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> 이상</td><td colspan="2">/Users/[사용자 이름]/Library/Application Support/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">레거시</td><td colspan="2">/Users/[사용자 이름]/Library/Application Support/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>리눅스</strong></td><td colspan="1"><strong>7.2</strong> 이상</td><td colspan="2">/home/[사용자 이름]/.local/share/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>레거시</td><td colspan="2">/home/[사용자 이름]/.local/share/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!NOTE]
>
> 위에서 언급한 경로의 일부 디렉터리는 기본적으로 숨겨져 있을 수 있습니다. 파일 탐색기에서 경로를 수동으로 입력하거나 숨겨진 파일을 표시하여 확인합니다.
