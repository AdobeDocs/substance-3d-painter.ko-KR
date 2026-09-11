---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/home.html"
breadcrumb-title: ''
description: Substance 3D Painter으로 시작하여 3D 모델에 텍스처를 직접 페인트 하고 사실적인 재질 표면을 만들어 보세요.
helpx_creative_field: ""
helpx_description: Painter > Home
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 9%

---


# Substance 3D Painter

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

Substance 3D Painter은 3D 페인팅 소프트웨어로서 3D 메시를 텍스처 및 렌더링할 수 있습니다.

이 설명서는 기본 기술부터 고급 기술까지 이 소프트웨어를 사용하는 방법을 배우는 데 도움이 되도록 작성되었습니다.

이 설명서에서 답변되지 않은 질문이 있는 경우 당사의 [포럼](https://community.adobe.com/t5/substance-3d-painter/bd-p/substance-3d-painter)에서 자유롭게 질문해 주십시오. PBR에 대해 자세히 알아보려면 [Physically Based Rendering 안내서](https://helpx.adobe.com/kr/substance-3d/unlisted/tutorials.html)를 다운로드할 수도 있습니다.

</td>
<td width="58.30%" style="border: 0;" valign="top">

![](assets/2021.jpg){width="600px"}

</td>
</tr>
</table>

## 시작하기

* [활성화 및 라이선스](getting-started/activation-and-licenses.md) - 이 페이지에는 Painter 사용을 시작할 수 있도록 라이선스를 활성화하고 관리하는 방법에 대한 정보가 있습니다.
* [시스템 요구 사항](getting-started/system-requirements.md) - 시스템 요구 사항 및 하드웨어 호환성 정보를 다시 그룹화합니다.
* [프로젝트 만들기](getting-started/project-creation.md) - 새 프로젝트 만들기 창에서 3D 모델 및 해당 텍스처링 정보를 저장하는 프로젝트 파일을 만들 수 있습니다.
* [내보내기](export/export.md) - 프로젝트를 비트맵 텍스처으로 내보내 다른 소프트웨어와 함께 사용할 수 있습니다. 3D 모델의 형상을 내보낼 수도 있습니다.
* [용어집](getting-started/glossary.md) - 이 페이지에는 응용 프로그램에 사용된 가장 일반적인 키워드와 그 뒤에 있는 개념에 대한 간단한 설명이 나열됩니다.
* [성능](technical-support/performances-guidelines/performances-guidelines.md) - 이 페이지에서는 성능을 최대화하고 작업이 원활하게 실행되도록 하는 방법에 대한 팁과 요령을 다시 그룹화합니다.

### 인터페이스

* [에셋](interface/assets/assets.md)
* [색상 피커](interface/color-picker.md)
* [디스플레이 설정](interface/display-settings/display-settings.md)
* [작업 내역](interface/history.md)
* [레이어 스택](interface/layer-stack/layer-stack.md)
* [메인 메뉴](interface/main-menu/main-menu.md)
* [프로젝트 구성](interface/project-configuration.md)
* [속성](interface/properties.md)
* [설정](interface/settings/settings.md)
* [셰이더 설정](interface/shader-settings/shader-settings.md)
* [텍스처 세트](interface/texture-set/texture-set.md)
* [도구 모음](interface/toolbars.md)
* [뷰포트](interface/viewport/viewport.md)

### 페인팅 도구

* [도구 목록](painting/tool-list/tool-list.md) - 이 페이지에서는 사용 가능한 모든 페인팅 도구와 사용 방법에 대해 자세히 설명합니다.
* [직선](painting/straight-line.md) — 직선은 모든 페인팅 도구로 클릭 수를 줄이고 보다 정밀하게 선을 그리는 쉬운 방법입니다.
* [레이지 마우스](painting/lazy-mouse.md) - 레이지 마우스는 마우스 커서와 실제 페인팅 사이의 거리 오프셋으로, 이를 통해 보다 정밀하거나 매끄러운 획을 페인트 할 수 있습니다.
* [대칭](painting/symmetry/symmetry.md) — 대칭은 기하학적 제약 조건을 기반으로 여러 위치에서 동시에 페인팅하는 작업입니다.
* [칠 투영](painting/fill-projections/fill-projections.md) — 칠 레이어 및 칠 효과는 특정 모드를 기준으로 메시에 직접 텍스처를 투영합니다. 이러한 유형의 레이어/효과는 3D 모델에 텍스처를 수동으로 페인트 하는 것을 방지합니다. 속성 창에서 투영 설정을 편집할 수 있습니다.
* [사전 설정](painting/presets/presets.md) — 사전 설정은 페인팅 도구의 저장된 구성입니다. 이 페이지에서는 이러한 유틸리티를 사용하는 방법과 이유를 설명합니다.
* [역동적인 획](painting/dynamic-strokes/dynamic-strokes.md) - 역동적인 획은 Substance 파일로 구동되는 일반 브러시 획으로, 브러시 획 내의 각 스탬프마다 변경할 수 있습니다.
* [고급 채널 페인팅](painting/advanced-channel-painting/advanced-channel-painting.md) - 셰이더에서 사용되는 일부 기본 채널을 페인팅하여 고급 또는 복잡한 효과를 만들 수 있습니다. 예를 들어, 표준 맵으로 변환되는 페인팅 Height 정보가 있습니다.

### 베이킹

* [메시 맵을 분리하는 방법](baking/how-to-bake-mesh-maps.md)
* [굽기 시각화 설정](baking/baking-visualization-settings.md)

### 콘텐츠

* [사용자 정의 효과 만들기](content/creating-custom-effects/creating-custom-effects.md)
* [에셋 가져오기](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/adding-content-to-the-shelf-142213317.html)

### 기능

* [자동 UV 풀기](features/automatic-uv-unwrapping.md)
* [효과](features/effects/effects.md)
* [실제 크기](features/physical-size.md)
* [스마트 재질 및 마스크](features/smart-materials-and-masks.md)
* [서브서피스 스케터링](features/subsurface-scattering/subsurface-scattering.md)
* [동적 재질 레이어](features/dynamic-material-layering.md)
* [UV 재투영](features/uv-reprojection.md)
* [UV 타일](features/uv-tiles/uv-tiles.md)
* [색상 관리](features/color-management/color-management.md)
* [후처리](features/post-processing/post-processing.md)
* [Iray 렌더러](features/iray-renderer/iray-renderer.md)
* [플러그인](features/plugins/plugins.md)
* [스파스 가상 텍스처](features/sparse-virtual-textures.md)
* [사용자 정의 셰이더](features/custom-shaders.md)
* [SpaceMouse® by 3Dconnection](features/spacemouse-by-3dconnexion.md)
* [Universal Scene Description (USD)](features/universal-scene-description-usd.md)

### 파이프라인 및 통합

* [설치 및 환경 설정](pipeline-and-integration/installation-and-pre/preferences-and-application-data-location.md)
* [구성](pipeline-and-integration/configuration/command-lines.md)
* [리소스 관리](pipeline-and-integration/resource-management/adding-resource-paths-edi/adding-resource-paths-by-editing-preferences-manually.md)

### 스크립팅 및 개발

* [스크립트 및 플러그인](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/script-and-plugins-197427392.html)

### 기술 지원

* [성능 지침](technical-support/performances-guidelines/performances-guidelines.md)
* [펜 및 태블릿 구성](technical-support/configuring-pens-and-tablets.md)
* [로그 파일 내보내기](technical-support/exporting-the-log-file.md)
* [DXDiag 내보내기](technical-support/exporting-a-dxdiag.md)

### 릴리스 정보

* [모든 변경 내용](release-notes/all-changes.md)
* [버전 11.1](release-notes/version-11-1.md)
* [버전 11.0](release-notes/version-11-0.md)
* [버전 10.1](release-notes/version-10-1.md)

