---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/getting-started/export.html"
breadcrumb-title: ''
description: Substance 3D Painter의 텍스처를 다양한 포맷으로 내보내 다른 애플리케이션과 게임 엔진에 사용하는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Getting Started > Export
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 내보내기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# 내보내기

## 텍스처 내보내기

텍스처는 비트맵 컬렉션으로 내보내집니다. Painter은 출력 템플릿 덕분에 텍스처를 내보낼 때 많은 유연성을 제공합니다. 출력 템플릿을 사용하면 내보낸 파일의 이름 지정, 텍스처가 채널에 압축되는 방식, 내보낸 파일의 형식 및 비트 심도 등을 제어할 수 있습니다. 두렵지만 걱정하지 마십시오. Painter에는 일반적으로 사용되는 3D 출력 템플릿 및 사용 사례로 구성된 수십 개의 기본 애플리케이션이 포함되어 있습니다.

<b>내보내기 창</b>을 열고 <b>파일 > 텍스처 내보내기</b>를 사용하여 텍스처 내보내기를 시작하거나 키보드 단축키 <b>CTRL + SHIFT + E</b>를 사용합니다. 다음 링크를 사용하여 텍스처 내보내기에 대해 자세히 알아보십시오.

* [내보내기 창](../export/export-window/export-window.md)
* [출력 템플릿](../export/export-presets/export-presets.md)
* [출력 템플릿 수정 또는 만들기](creating-export-presets.md)

### 메시 내보내기

Painter은 예를 들어 자동으로 UV를 생성하여 가져온 메쉬를 수정할 수 있습니다. Painter에서 망을 변경한 경우 <b>파일 > 망 내보내기</b>를 사용하여 망을 내보낼 수 있습니다.

메시를 내보낼 때 다음과 같은 몇 가지 옵션이 제공됩니다.

* <b>변위/테셀레이션 없이</b>: 재질을 기반으로 형상을 수정하지 않고 기본 메시를 내보냅니다.
  * <b>삼각측정 적용</b>: 가져온 메시가 쿼드나 다각형으로 구성된 경우 이 옵션을 활성화하여 Painter 삼각측정 버전의 메시를 내보낼 수 있습니다. 이렇게 하면 다른 응용 프로그램이 다르게 삼각형을 설정하는 경우 시각적 삼각측정 기반 버그를 방지하는 데 도움이 될 수 있습니다.
* <b>변위/테셀레이션 사용</b>: Painter은 메쉬를 테셀레이션하여 다각형을 더 추가하고 변위 또는 Height을 사용하여 메쉬의 표면 형상을 변경합니다.
  * <b>정점 수직 다시 계산</b>: 메시 표면을 수정하면 기존 정점의 수직이 잘못될 수 있습니다. 이 옵션을 활성화하면 Painter에서 정점 표준을 새 서피스에 대한 올바른 값으로 자동으로 업데이트합니다.

![](../assets/export-render.jpg){width="500px"}
