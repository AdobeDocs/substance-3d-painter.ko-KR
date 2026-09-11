---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/startup-issues/application-failed-to-start-because-of-qt.html"
breadcrumb-title: ''
description: 적절한 애플리케이션 실행을 위해 Qt 프레임워크 문제로 인한 Substance 3D Painter 시작 오류를 수정하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Startup Issues > Application failed to start because of Qt
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Qt 때문에 응용 프로그램을 시작하지 못했습니다.
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '130'
ht-degree: 0%

---


# Qt 때문에 응용 프로그램을 시작하지 못했습니다.

애플리케이션을 시작할 때 다음과 같은 오류 메시지가 표시될 수 있습니다.

>> 

Qt 플랫폼 플러그인을 초기화할 수 없으므로 이 애플리케이션을 시작하지 못했습니다. 애플리케이션을 다시 설치하면 이 문제가 해결될 수 있습니다.

사용 가능한 플랫폼 플러그인: minimal, offscreen, webgl, windows.

다른 소프트웨어가 애플리케이션과 충돌하는 환경 변수를 정의했기 때문에 이 오류가 발생할 수 있습니다.

응용 프로그램을 시작하기 전에 현재 환경에서 다음 변수를 제거하십시오.

```
QT_PLUGIN_PATH 

QML2_IMPORT_PATH
```


>[!NOTE]
>
> 이러한 변수는 Python 컨텍스트에서도 상속될 수 있습니다(예: **pyinstaller** 사용). 응용 프로그램이 실행되는 컨텍스트에서 제거해야 합니다.
