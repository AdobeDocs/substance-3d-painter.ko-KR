---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-when-opening-or-saving-a-file.html"
breadcrumb-title: ''
description: 안정적인 프로젝트 관리를 위해 파일을 열거나 저장할 때 Substance 3D Painter 충돌을 해결하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash when opening or saving a file
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 파일을 열거나 저장할 때 충돌
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# 파일을 열거나 저장할 때 충돌

파일 대화 상자를 열 때 Windows에서 Substance 3D Painter이 충돌을 하는 몇 가지 이유가 있습니다. 이 페이지에서는 이 문제에 대한 이유와 해결 방법을 다시 그룹화합니다.

## 소프트웨어 충돌

일부 프로그램은 불안정성이나 충돌을 초래할 수 있는 사용자 정의 셸 확장을 추가할 수 있습니다. 자세한 내용은 [소프트웨어 충돌](../startup-issues/software-conflicts.md) 목록을 확인하세요.

## 셸 확장/사용자 지정 테마

사용자 정의 테마는 GUI 프레임워크에서 지원되지 않으므로 Substance 3D Painter을 사용하기 전에 현재 테마를 제거하는 것이 좋습니다.

**Alienware**/**Dell** 컴퓨터는 Substance 3D Painter과 호환되지 않는 것으로 알려진 일부 셸 확장을 기본적으로 통합합니다. 제거하는 것이 좋습니다. 호환되지 않는 모든 확장 기능은 정확히 알 수 없지만 대부분의 경우 다음에 해당합니다.

* DBROverlayIconBackuped.DBROverlayIconBackuped 클래스
* DBROverlayIconNotBackuped.DBROverlayIconNotBackuped 클래스

다음 도구를 사용하여 컴퓨터에 설치된 확장 프로그램을 확인할 수 있습니다. 진행 방법에 대한 대략적인 절차는 다음과 같습니다.

1. NirSoft에서 ShellExView 다운로드 및 설치: <http://www.nirsoft.net/utils/shexview.html>
1. 프로그램 실행
1. **옵션**&#x200B;을 클릭하고 **확장 유형별 필터링**&#x200B;을 선택합니다.
1. **아이콘 오버레이 처리기** 선택
1. **Alien Respawn**&#x200B;에 대한 두 개의 항목이 표시됩니다.
1. **둘 다**&#x200B;를 선택하고 빨간색 단추를 클릭하여 사용하지 않도록 설정합니다.
