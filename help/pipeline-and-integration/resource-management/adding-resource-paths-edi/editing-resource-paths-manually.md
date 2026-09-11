---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/adding-resource-paths-by-editing-preferences-manually/editing-resource-paths-manually.html"
breadcrumb-title: ''
description: Substance 3D Painter 환경 설정에서 리소스 경로를 수동으로 편집하여 쉘프 리소스 위치를 사용자 정의하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding resource paths by editing preferences manually > Editing resource paths manually
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 수동으로 리소스 경로 편집
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 1%

---


# 수동으로 리소스 경로 편집

이 페이지는 응용 프로그램을 시작하지 않고 리소스 경로를 추가 또는 제거하기 위해 환경 설정을 편집하는 방법에 대한 안내서입니다.

## 환경 설정 위치

리소스 위치는 응용 프로그램 환경 설정으로 관리되며 플랫폼에 따라 변경될 수 있습니다.

<table data-preserve-html="true"> <colgroup> <col/> <col/> <col/> </colgroup> <tbody> <tr> <th>시스템</th> <th>버전</th> <th>경로</th> </tr> <tr> <td rowspan="2"><p><strong>Windows</strong></p><p>(레지스트리)</p></td> <td><strong>7.2</strong> 이상</td> <td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td>레거시</td> <td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><p><strong>Mac</strong></p><p>(라이브러리)</p></td> <td><strong>7.2</strong> 이상</td> <td>/Users/[사용자 이름]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td> </tr> <tr> <td>레거시</td> <td>/Users/[사용자 이름]/Library/Preferences/com.substance3d.Substance Painter.plist</td> </tr> <tr> <td rowspan="2"><strong>리눅스</strong></td> <td><strong>7.2</strong> 이상</td> <td>/home/[사용자 이름]/.config/Adobe/Adobe Substance 3D Painter.conf</td> </tr> <tr> <td>레거시</td> <td>/home/[사용자 이름]/.config/Allegorithmic/Substance Painter.conf</td> </tr> </tbody> </table>

## Windows에서 패스 추가

Windows에서는 Windows 레지스트리를 통해 경로를 관리할 수 있습니다.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/reg-shelf-pathinfos.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/reg-content.png)

</td>
</tr>
</table>

1. **시작 > 실행**&#x200B;을 클릭하거나 **Windows + R** 을 누릅니다.
1. 대화 상자에 &quot;**regedit**&quot;(따옴표 제외)을 입력하고 **확인**&#x200B;을 누릅니다.
1. **레지스트리 편집기** 창의 왼쪽에 있는 트리 보기에서 이동하여 위에 언급된 레지스트리 키로 이동합니다.
1. **숫자**&#x200B;를 이름으로 사용하여 **pathInfos** 아래에 **키를 추가합니다**. 기존의 키(1부터 시작)를 기준으로 숫자를 증가시킵니다.
1. 창의 오른쪽 부분에서 **마우스 오른쪽 단추** > **새로 만들기** > **문자열 값**&#x200B;을 수행합니다. 이름을 **사용 안 함**&#x200B;으로 지정하고 값을 **false**(으)로 설정합니다.
1. 창의 오른쪽 부분에서 **마우스 오른쪽 단추** > **새로 만들기** > **문자열 값**&#x200B;을 수행합니다. 이름을 **이름**&#x200B;으로 지정하고 사용자 지정 셸프의 이름을 입력합니다.
1. 창의 오른쪽 부분에서 **마우스 오른쪽 단추** > **새로 만들기** > **문자열 값**&#x200B;을 수행합니다. 이름을 **path**&#x200B;로 지정하고 값을 셸프가 있는 path로 설정합니다.
1. &quot; **pathInfos** &quot; 내에서 &quot; **size**&quot; 키를 1씩 증가시킵니다.
1. 창을 닫습니다.
1. 애플리케이션을 시작합니다.

**writableShelf** 항목의 값을 새 위치의 이름으로 변경하여 새 경로를 기본 경로(사전 설정과 같이 새 리소스가 생성된 경우)로 정의할 수 있습니다.

![](../../../assets/default-shelf.png)

## Linux에서 경로 추가

**Linux**&#x200B;에서는 홈 디렉터리에 저장된 사용자 응용 프로그램 기본 설정 구성 파일을 통해 추가 경로를 만들 수 있습니다(참조).

1. 위에 언급된 경로로 이동합니다.
1. **Substance 3D Painter.config** 파일 열기
1. **[Shelf]** 섹션까지 아래로 스크롤

표시되는 마지막 숫자를 증분하여 새 셸프 경로를 추가합니다. 예:

```
pathInfos2disabled=false  

pathInfos2name=custom_resources 

pathInfos2path=/home/Username/Documents/custom_path 

writableShelf=custom_resources
```


**writableShelf** 변수를 사용하여 기본 경로가 될 경로(사전 설정과 같은 새 리소스가 생성된 경우)를 지정합니다.

변경 사항을 저장하고 애플리케이션을 다시 시작합니다.
