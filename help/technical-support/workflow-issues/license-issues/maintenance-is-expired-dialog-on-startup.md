---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/workflow-issues/license-issues/maintenance-is-expired-dialog-on-startup.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 라이선스 관리를 위해 시작할 때 표시되는 유지 관리 만료 대화 상자를 해결하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > License Issues > Maintenance is expired dialog on startup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 시작할 때 [유지 관리 만료] 대화 상자 표시
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---


# 시작할 때 [유지 관리 만료] 대화 상자 표시

![](../../../assets/expired-mainteance-message.png)

애플리케이션을 시작하면 &quot;현재 유지 관리가 만료되었습니다&quot;라는 메시지가 있는 대화 상자가 나타날 수 있습니다. 이 페이지에서는 이 대화 상자를 방지하는 방법에 대한 해결 방법을 나열합니다.

## 해결 방법 1: 라이선스 파일 업데이트

라이선스 파일이 너무 오래되어 업데이트해야 하므로 경고 메시지가 표시됩니다. 이렇게 하려면 응용 프로그램 마법사를 통해 **제품을 다시 활성화**&#x200B;하면 됩니다. 라이선스 파일은 Substance 3D 웹 사이트 <https://www.substance3d.com/>을(를) 통해 수동으로 다운로드할 수도 있습니다.

## 해결 방법 2: 환경 설정을 편집하여 대화 상자 숨기기

>[!NOTE]
>
> 이 대체 솔루션을 사용하기 전에 라이선스 파일을 먼저 업데이트하는 것이 좋습니다.

또 다른 해결책은 특정 설정을 적절하게 배치하여 경고 메시지를 숨기는 것입니다.

응용 프로그램 기본 설정 위치로 이동합니다.

<table data-preserve-html="true"><colgroup> <col/> <col/> <col/> </colgroup><tbody><tr><th>시스템</th><th>버전</th><th>경로</th></tr><tr><td rowspan="2"><p><strong>Windows</strong></p><p>(레지스트리)</p></td><td><strong>7.2</strong> 이상</td><td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td></tr><tr><td>레거시</td><td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><p><strong>Mac</strong></p><p>(라이브러리)</p></td><td><strong>7.2</strong> 이상</td><td>/Users/[사용자 이름]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td></tr><tr><td>레거시</td><td>/Users/[사용자 이름]/Library/Preferences/com.substance3d.Substance Painter.plist</td></tr><tr><td rowspan="2"><strong>리눅스</strong></td><td><strong>7.2</strong> 이상</td><td>/home/[사용자 이름]/.config/Adobe/Adobe Substance 3D Painter.conf</td></tr><tr><td>레거시</td><td>/home/[사용자 이름]/.config/Allegorithmic/Substance Painter.conf</td></tr></tbody></table>

### Windows

Windows에서 변수를 설정하려면 다음 단계를 따르십시오.

1. 시작 메뉴를 엽니다.
1. 레지스트리 편집기를 열려면 **Regedit**&#x200B;을(를) 검색하십시오.
1. 위 표에 나열된 레지스트리 키로 이동합니다.
1. 왼쪽에 있는 트리 보기에서 소프트웨어로 명명된 레지스트리 키를 클릭합니다.
1. 오른쪽 패널의 빈 영역을 마우스 오른쪽 단추로 클릭하고 **새로 만들기 > 문자열 값**&#x200B;을 선택합니다.
1. 새 값의 이름을 **DisableLicenseWarningPopup**(으)로 지정하고 Enter 키를 눌러 유효성을 검사합니다.
1. 방금 만든 값을 두 번 클릭합니다.
1. 값 데이터 필드를 **true**(으)로 설정
1. 변경 사항을 저장합니다.
1. 애플리케이션을 시작합니다.

### MacOS

1. 새 **파인더** 창 열기
1. 위 표에 나열된 경로로 이동합니다.
1. **plist** 파일을 마우스 오른쪽 단추로 클릭하고 **연결 프로그램 > Xcode**&#x200B;을 선택합니다.
1. 목록의 맨 위에 **DisableLicenseWarningPopup**&#x200B;이라는 새 키를 추가합니다.
1. 키 유형을 **문자열**(으)로 설정
1. 키 값을 **true**(으)로 설정
1. 파일을 저장하고 닫습니다.
1. 애플리케이션을 시작합니다.

### 리눅스

Linux에서 변수를 설정하려면 다음 단계를 수행하십시오.

1. 위 표의 경로 목록으로 이동합니다.
1. 폴더에 있는 **.conf** 파일을 엽니다.
1. 줄 **[일반]** 아래에 새 줄 추가
1. 새 줄에 다음 텍스트를 붙여넣습니다. **DisableLicenseWarningPopup=true**
1. 파일을 저장합니다.
1. 애플리케이션을 시작합니다.
