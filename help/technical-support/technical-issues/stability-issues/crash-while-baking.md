---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-while-baking.html"
breadcrumb-title: ''
description: 안정적인 텍스처 제빙 워크플로우를 위해 제빙 작업 중에 Substance 3D Painter 충돌을 수정하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash while baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 굽는 동안 충돌
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# 굽는 동안 충돌

일부 구성의 베이킹 프로세스 중에 Substance 3D Painter이 충돌 될 수 있습니다. 이 페이지에서는 알려진 문제 및 이러한 문제를 완화하는 방법에 대한 목록을 다시 그룹화합니다.

## 베이킹 미리 보기 충돌

기본적으로 Substance 3D Painter은 텍스처 굽기의 진행 중 상태를 뷰포트에 표시합니다. 일부 컴퓨터에서는 이 기능이 불안정하게 될 수 있습니다.

이 기능을 비활성화하려면:

1. **편집 > 설정**&#x200B;을 사용하여 기본 설정 열기
1. **일반**&#x200B;에서 **굽기 옵션** 섹션으로 스크롤합니다.
1. **실시간 미리 보기 굽기 프로세스 사용** 옵션을 선택/사용 안 함으로 설정합니다.

## GPU 광선 추적 충돌

드라이버가 불안정한 일부 GPU에서는 GPU 광선 추적 기능으로 인해 베이킹 프로세스가 충돌으로 이어질 수 있습니다.

이 기능을 비활성화하려면:

1. **편집 > 설정**&#x200B;을 사용하여 기본 설정 열기
1. **일반**&#x200B;에서 **굽기 옵션** 섹션으로 스크롤합니다.
1. **GPU 광선 추적 사용** 옵션을 선택/사용 안 함으로 설정합니다.

## Ryzen CPU를 사용한 충돌

애플리케이션은 Ryzen CPU로 실행되는 일부 컴퓨터 구성에서 베이킹 프로세스 동안 충돌 될 수 있다. 일반적으로 BIOS 업데이트로 문제가 해결됩니다.

이는 멀티 스레드 계산과 관련이 있습니다. 많은 마더보드 생성자가 이 문제를 해결하기 위해 새로운 BIOS 업데이트를 발행했으므로 업데이트를 적용하는 것이 좋습니다. 자세한 내용은 마더보드 설명서 및 생성자 웹 사이트를 참조하십시오.

## 호환되지 않는 Assbin 파일

베이킹 시 기본적으로 하이 폴리 메시는 **\*.assbin** 파일로 사전 처리되어 나중에 다시 베이킹 속도를 높일 수 있습니다. 드문 경우지만 이러한 파일은 다른 버전으로 생성된 경우 애플리케이션에 충돌을 줄 수 있습니다. 이러한 파일을 삭제하면 문제가 해결됩니다. 그러면 다시 생성됩니다.
