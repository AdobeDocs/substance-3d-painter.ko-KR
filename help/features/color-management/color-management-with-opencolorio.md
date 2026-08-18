---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/color-management/color-management-with-opencolorio.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 OpenColorIO 색상 관리를 사용하여 파이프라인 간에 일관된 색상 작업 과정을 만드는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management > Color management with OpenColorIO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: OpenColorIO를 사용한 색상 관리
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 8%

---


# OpenColorIO를 사용한 색상 관리

이 페이지에는 OpenColorIO(OCIO)와 관련된 색상 관리 설정이 나열됩니다.

## 프로젝트 설정

![](../../assets/project-settings-3.png)

프로젝트 설정은 [새 프로젝트](../../getting-started/project-creation.md) 창을 통해 또는 [프로젝트 구성](../../interface/project-configuration.md) 창을 사용하여 새 프로젝트를 만들 때 설정할 수 있습니다.

>[!NOTE]
>
> **OCIO** 환경 변수가 있고 유효한 구성 파일을 지정하는 경우 UI의 설정을 재정의하고 비활성화합니다.

사용 가능한 설정은 다음과 같습니다.

<table data-preserve-html="true" style="width: 99.9039%;"><colgroup><col style="width: 12.512%;"/><col style="width: 21.1742%;"/><col style="width: 66.3122%;"/></colgroup><tbody><tr><th style="width: 12.5%;">섹션</th><th style="width: 21.1538%;">설정</th><th style="width: 66.25%;">설명</th></tr><tr><td rowspan="3" style="width: 12.5%;"><strong>구성</strong></td><td style="width: 21.1538%;"><strong>색상 관리</strong></td><td style="width: 66.25%;"><p>색상 관리에 사용할 엔진을 정의합니다.</p><p>가능한 값:</p><ul><li><strong>레거시</strong>(기본값): 미리 정의된 sRGB/선형 sRGB 감마 색상 교정을 사용합니다.</li><li><strong>OpenColorIO</strong>: OCIO 통합을 사용합니다.</li><li><strong>Adobe ACE</strong>: ICC 프로필을 지원하는 Adobe Color Engine.</li></ul></td></tr><tr><td style="width: 21.1538%;"><strong>OpenColorIO 구성</strong></td><td style="width: 66.25%;"><p>색상 관리 설정을 제어하는 데 사용할 구성 파일입니다.</p><p>가능한 값:</p><ul><li><strong>Substance</strong>(기본값): 작업 영역으로 선형 감마를 사용합니다.</li><li><strong>ACES 1.0.3</strong>: 작업 공간으로 ACEScg를 사용합니다.</li><li><strong>ACES 1.2</strong>: 작업 공간으로 ACEScg를 사용합니다.</li><li><strong>사용자 지정</strong>: 사용자 지정 구성 파일을 사용합니다.</li></ul></td></tr><tr><td style="width: 21.1538%;"><strong>구성 파일</strong></td><td style="width: 66.25%;">OCIO 구성 파일 경로 구성 모드가 <strong>사용자 지정</strong>(으)로 설정되어 있지 않으면 사용할 수 없습니다.</td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="2" style="width: 12.5%;"><strong>색상 설정</strong></td><td style="width: 21.1538%;"><strong>작업 색상 공간</strong></td><td style="width: 66.25%;">엔진이 응용 프로그램 내에서 작업하는 데 사용하는 색상 공간입니다. 텍스처가 변환(가져오기) 또는 변환(내보내기)될 수 있는 색상 공간입니다.</td></tr><tr><td colspan="1"><strong>표준 sRGB 색상 공간</strong></td><td colspan="1"><p>[표준 sRGB](https://en.wikipedia.org/wiki/SRGB) 색상 공간과 일치하는 색상 공간입니다(IEC 61966-2-1:1999).</p><p>이 색상 공간은 응용 프로그램 내의 여러 위치에서 사용됩니다.</p><ul><li>색상 피커의 16진수 필드에 있는 색상 세트를 변환합니다.</li><li>색상 피커에서 색상 견본을 저장하고 불러옵니다.</li><li>색상 피커 목록에 표시로 나열될 수 있습니다.</li></ul></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="4" style="width: 12.5%;"><strong>색상 공간 기본값 비트맵 가져오기</strong></td><td style="width: 21.1538%;"><strong>8비트 이미지</strong></td><td style="width: 66.25%;">8비트 이미지 파일을 가져올 때 기본적으로 사용하는 색상 공간입니다.</td></tr><tr><td style="width: 21.1538%;"><strong>16비트 이미지</strong></td><td style="width: 66.25%;">16비트 이미지 파일을 가져올 때 기본적으로 사용하는 색상 공간입니다.</td></tr><tr><td style="width: 21.1538%;"><strong>부동 소수점 이미지</strong></td><td style="width: 66.25%;">HDR/EXR 이미지 파일을 가져올 때 기본적으로 사용할 색상 공간.</td></tr><tr><td style="width: 21.1538%;"><strong>색상 공간 자동 감지</strong></td><td style="width: 66.25%;"><p>특정 설정을 기반으로 리소스의 색상 공간을 정의할 수 있습니다.</p><p>가능한 값:</p><ul><li><strong>사용 안 함</strong>: 기본 색상 설정을 사용하고 리소스 구성을 무시합니다.</li><li><strong>파일 이름 구문 분석</strong>(기본값): OCIO [명명 규칙](https://opencolorio.readthedocs.io/en/latest/guides/authoring/rules.html?highlight=filename#strictparsing)을 사용하여 리소스가 사용하는 색상 공간의 이름을 추출합니다.</li><li><strong>구성 파일 규칙 사용</strong>: OCIO 구성을 사용하여 색상 공간을 할당하는 방법을 결정합니다. 이 매개 변수는 이전 이미지 파일 색상 공간 설정보다 우선합니다.</li></ul></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td style="width: 12.5%;"><strong>Substance 자료</strong></td><td style="width: 21.1538%;"><strong>재질 색상 공간 기본값</strong></td><td style="width: 66.25%;"><p>Substance 재질 색상 관리 입력/출력에 사용할 색상 공간을 정의합니다(채널 목록은 아래 참조).</p></td></tr><tr><th style="width: 12.5%;"><br/></th><th style="width: 21.1538%;"><br/></th><th style="width: 66.25%;"><br/></th></tr><tr><td rowspan="3" style="width: 12.5%;"><strong>색상 공간 내보내기</strong><br/><br/><br/></td><td style="width: 21.1538%;"><strong>8비트 이미지</strong></td><td style="width: 66.25%;">8비트 이미지 파일을 내보낼 때 기본적으로 사용하는 색상 공간입니다.</td></tr><tr><td style="width: 21.1538%;"><strong>16비트 이미지</strong></td><td style="width: 66.25%;">16비트 이미지 파일을 내보낼 때 기본적으로 사용하는 색상 공간입니다.</td></tr><tr><td style="width: 21.1538%;"><strong>부동 소수점 이미지</strong></td><td style="width: 66.25%;">HDR/EXR 이미지 파일을 내보낼 때 기본적으로 사용하는 색상 공간.</td></tr></tbody></table>

### OpenColorIO 역할

다음 역할이 지원되며 색상 공간의 기본 선택을 변경할 수 있습니다.

| 역할 이름 | 설명 |
| --- | --- |
| **substance\_3d\_painter\_standard\_srgb** | [표준 sRGB](https://en.wikipedia.org/wiki/SRGB)과(와) 일치하는 색상 공간을 지정하는 역할입니다(IEC 61966-2-1:1999). |
| **substance\_3d\_painter\_bitmap\_import\_8bit** | 8비트 이미지를 가져오는 데 사용되는 색상 공간을 지정하는 역할입니다. |
| **substance\_3d\_painter\_bitmap\_import\_16bit** | 16비트 이미지를 가져오는 데 사용되는 색상 공간을 지정하는 역할입니다. |
| **substance\_3d\_painter\_bitmap\_import\_floating** | HDR 이미지를 가져오는 데 사용되는 색상 공간을 지정하는 역할입니다. |
| **substance\_3d\_painter\_substance\_material** | Substance 재질에서 색상 관리 채널에 사용되는 색상 공간을 지정하는 역할입니다. |
| **substance\_3d\_painter\_bitmap\_export\_8bit** | 8비트 텍스처를 내보낼 때 사용되는 색상 공간을 지정하는 역할입니다. |
| **substance\_3d\_painter\_bitmap\_export\_16bit** | 16비트 텍스처를 내보낼 때 사용되는 색상 공간을 지정하는 역할입니다. |
| **substance\_3d\_painter\_bitmap\_export\_floating** | HDR 텍스처를 내보낼 때 사용되는 색상 공간을 지정하는 역할입니다. |

>[!NOTE]
>
> 애플리케이션에 제공되는 OCIO 구성은 이러한 특정 역할을 사용하는 방법에 대한 예시로 사용할 수 있습니다.
