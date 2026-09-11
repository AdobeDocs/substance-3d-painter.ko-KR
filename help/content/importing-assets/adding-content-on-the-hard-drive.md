---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/content/importing-assets/adding-content-on-the-hard-drive.html"
breadcrumb-title: ''
description: 하드 드라이브에서 Substance 3D Painter으로 콘텐츠를 추가하여 로컬 파일로 리소스 라이브러리를 확장하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Content > Importing assets > Adding content on the hard drive
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 하드 드라이브에 콘텐츠 추가
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 1%

---


# 하드 드라이브에 콘텐츠 추가

하드 드라이브의 올바른 위치에 새 콘텐츠를 직접 배치하여 라이브러리에 리소스를 추가할 수 있습니다.

사용자 에셋에 대한 기본 폴더는 애플리케이션 인터페이스를 통하거나 다음 위치에 수동으로 놓아 새 콘텐츠를 추가할 수 있는 위치에 기본적으로 제공됩니다. 이 기본 라이브러리는 브러시, 도구, 스마트 재질 등과 같은 새 사전 설정을 만들 때도 사용됩니다. 자세한 내용은 [사전 설정](../../painting/presets/presets.md) 설명서를 참조하세요.

## 에셋을 어디에 넣어야 합니까?

아래는 기본적으로 사용자 지정 콘텐츠가 만들어지는 기본 **내 에셋** 라이브러리의 위치입니다.

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>플랫폼</th><th>버전</th><th>경로</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong> 이상</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">레거시</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> 이상</td><td colspan="1">/Users/사용자 이름/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">레거시</td><td colspan="1">/Users/사용자 이름/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>리눅스</strong></td><td colspan="1"><strong>7.2</strong> 이상</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>레거시</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

>[!WARNING]
>
> 애플리케이션과 함께 제공되는 **스타터 에셋**&#x200B;은(는) 설치 폴더 내에 있으며 각각의 새 버전에서 대체됩니다. 개인 콘텐츠는 **모든 업데이트에서 지워지며** 읽기/쓰기 권한 문제가 발생할 수 있으므로 이 위치에 넣지 않는 것이 좋습니다.\
> **내 에셋** 위치 또는 다른 사용자 지정 위치를 사용하는 것이 가장 좋습니다. 사용자 지정 라이브러리 위치를 추가하는 방법에 대한 자세한 내용은 [새 라이브러리 추가](../../interface/assets/adding-a-new-library.md)를 참조하십시오.

## 파일 형식 및 사용

다양한 유형의 파일을 Substance 3D Painter 라이브러리로 가져올 수 있습니다. 지정된 폴더(예: *알파*, *색조*, *효과*...)에 배치하는 중 에서는 사용 유형을 에셋에 할당하므로, 새 콘텐츠를 추가할 때 적합한 폴더를 선택하는 것이 중요합니다. 사용자 정의 라이브러리 위치를 추가하면 해당 위치에 적절한 폴더가 자동으로 만들어집니다.

| *파일 형식* | *사용* | *폴더* |
| --- | --- | --- |
| **SBSAR** | Substance 재질 | 에셋/재질 |
| **SBSAR** | 필터 | 에셋/효과 |
| **SBSAR** | Generators | 에셋/생성기 |
| **PNG, TGA, JPEG 등** | 텍스처 또는 Alpha | 에셋/텍스처 **또는** 선반/Alpha |
| **HDR, EXR** | 환경 또는 색상 Lut | 에셋/환경 **또는** 셸프/Colorlut |
| **GLSL** | 셰이더 | 에셋/셰이더스 |
| **SPPR** | 브러시 사전 설정 | 에셋/사전 설정/브러시 |
| **SPPR** | 입자 사전 설정 | 에셋/사전 설정/파티클 |
| **SPPR** | 재질 사전 설정 | 에셋/사전 설정/재질 **또는** 에셋/재질 |
| **SPPR** | 도구 사전 설정 | 에셋/사전 설정/도구 |
| **SPSM** | 스마트 재질 | 에셋/스마트 재질 |
| **SPMSK** | 스마트 마스크 | 에셋/스마트 마스크 |
| **SPEXP** | 내보내기 사전 설정 | Shelf/Export-presets |

>[!NOTE]
>
> 버전 7.2.0부터 사용자 정의 폴더 및 범주는 라이브러리에서 사용할 수 있습니다. 에셋 창에서 [경로별 필터링](../../interface/assets/filter-by-path.md) 또는 [탐색 경로](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/navigating-in-the-shelf-147095659.html)를 통해 액세스할 수 있습니다.

>[!WARNING]
>
> **SBS**(SBSAR 아님) 파일은 직접 사용할 수 없습니다. Substance 3D Designer에서 SBSAR로 내보내야 합니다.
