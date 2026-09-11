---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/impossible-to-use-the-alt-keyboard-shortcut-on-linux.html"
breadcrumb-title: ''
description: 적절한 키보드 탐색을 위해 Substance 3D Painter에서 Linux의 ALT 키보드 단축키 문제를 해결하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Impossible to use the ALT keyboard shortcut on Linux
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Linux에서 ALT 키보드 단축키 사용 불가
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---


# Linux에서 ALT 키보드 단축키 사용 불가

**Gnome**&#x200B;을(를) 사용자 인터페이스로 사용하는 Linux 배포(**Ubuntu** 또는 **CentOS**)를 실행하는 경우, **ALT** 키의 기본 동작을 비활성화하여 뷰포트를 탐색할 수 있습니다.

## 센트OS

1 - **시스템 > Windows**(으)로 이동

![](../../../assets/centos-window.png){width="250px"}

2 - &quot;이동 키&quot; 설정을 &quot; **Alt**&quot; 이외의 설정으로 변경합니다. 예를 들어 키보드의 &quot;Windows&quot; 키를 선택하려면 &quot; **Super**&quot;을(를) 사용합니다.

![](../../../assets/centos-setting.png){width="350px"}

## 우분투

1 - 터미널을 열고 다음 명령을 실행합니다.

```
sudo apt-get install dconf-tools
```


이렇게 하면 고급 구성 도구가 설치됩니다. 이 도구를 실행하려면 추가 종속성을 설치해야 할 수 있습니다.

2 - 시작 메뉴를 열고 &quot; **Dconf-tools** &quot;을(를) 찾습니다. 실행.

3 - 다음 경로로 이동하여 왼쪽에 있는 트리 메뉴를 확장합니다. **조직 > 그놈 > 데스크탑 > wm > 환경 설정**

4 - &quot;마우스-버튼-수정자&quot;를 편집하고 값을 변경합니다. 또는 대신 설정하지만 *비워 두지 마세요* . Super는 &quot;Windows&quot; 키에 해당합니다.

![](../../../assets/ubuntu-setting.png){width="500px"}
