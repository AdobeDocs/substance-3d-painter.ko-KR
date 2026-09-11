---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/features/color-management/color-management-with-adobe-ace-icc.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 Adobe ACE 및 ICC 색상 관리를 사용하여 일관된 색상 작업 과정을 만드는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management > Color management with Adobe ACE - ICC
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Adobe ACE을 사용한 색상 관리 - ICC
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Adobe ACE을 사용한 색상 관리 - ICC

이 페이지에서는 ICC 프로필이 있는 이미지를 사용할 수 있도록 Adobe Color Engine(ACE)와 관련된 색상 관리 설정을 나열합니다.

## 프로젝트 설정

![](../../assets/cm-ace.png)

프로젝트 설정은 [새 프로젝트](../../getting-started/project-creation.md) 창을 통해 또는 [프로젝트 구성](../../interface/project-configuration.md) 창을 사용하여 새 프로젝트를 만들 때 설정할 수 있습니다.

>[!NOTE]
>
> 환경 변수(아래 참조) 또는 사전 설정 파일을 로드하면 UI의 설정이 비활성화됩니다.

사용 가능한 설정은 다음과 같습니다.

| 섹션 | 설정 | 설명 |
| --- | --- | --- |
| **구성** | **색상 관리** | 색상 관리에 사용할 엔진을 정의합니다.가능한 값:<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>레거시</strong>(기본값): 미리 정의된 sRGB/선형 sRGB 감마 색상 교정을 사용합니다.</li> <li data-preserve-html="true"><strong>OpenColorIO</strong>: OCIO 통합을 사용합니다.</li> <li data-preserve-html="true"><strong>Adobe ACE</strong>: Adobe Color Engine, ICC 프로필을 지원합니다.</li> </ul> |
|  | **사전 설정 파일 사용** | 활성화되면 json 구성 파일을 통해 색상 관리 설정을 제어할 수 있습니다. |
|  | **사전 설정 파일** | 사전 설정 파일의 경로(json 포맷) 자세한 내용은 아래를 참조하십시오. |
|  |  |  |
| **색상 설정** | **작업 색상 공간** | 엔진이 응용 프로그램 내에서 작업하는 데 사용하는 색상 공간입니다. 이는 텍스처를 변환(가져오기) 또는 변환(내보내기)할 수 있는 색상 공간입니다.가능한 값은 다음과 같습니다.<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>선형 sRGB IEC61966-2.1</strong>(기본값)</li> <li data-preserve-html="true"><strong>ACEScg ACE 작업 영역 AMPAS S-2014-004</strong></li> <li data-preserve-html="true"><strong>선형 Adobe RGB(1998)</strong></li> </ul> |
|  | **렌더링 의도** | 색상 공간 간에 색상을 변환하는 데 사용되는 방법을 지정합니다.가능한 값:<ul data-preserve-html="true"> <li data-preserve-html="true"><strong>가시 범위</strong></li> <li data-preserve-html="true"><strong>채도</strong>(기본값)</li> <li data-preserve-html="true"><strong>상대 색</strong></li> <li data-preserve-html="true"><strong>절대 색수차</strong></li> </ul> |
|  |  |  |
| **비트맵 가져오기 색상 공간 기본값** | **8비트 이미지** | 8비트 이미지 파일을 가져올 때 기본적으로 사용하는 색상 공간입니다. |
|  | **16비트 이미지** | 16비트 이미지 파일을 가져올 때 기본적으로 사용하는 색상 공간입니다. |
|  | **부동 소수점 이미지** | HDR/EXR 이미지 파일을 가져올 때 기본적으로 사용할 색상 공간입니다. |
|  | **사용 가능한 경우 포함된 ICC 프로필 사용(권장)** | 활성화되면 이미지 파일 이후 ICC 프로필을 사용하여 해당 색상을 조정합니다. |
|  |  |  |
| **Substance 자료** | **재질 색상 공간 기본값** | Substance 재질 색상 관리 입력/출력에 사용할 색상 공간을 정의합니다. |
|  |  |  |
| **색상 공간 내보내기** | **8비트 이미지** | 8비트 이미지 파일을 내보낼 때 기본적으로 사용하는 색상 공간입니다. |
|  | **16비트 이미지** | 16비트 이미지 파일을 내보낼 때 기본적으로 사용하는 색상 공간입니다. |
|  | **부동 소수점 이미지** | HDR/EXR 이미지 파일을 내보낼 때 기본적으로 사용하는 색상 공간. |

## 사전 설정 파일 사용

![](../../assets/cm-ace-env-var.png)

새 프로젝트를 만들 때 사전 설정 파일(json 형식)을 사용하여 ACE 설정을 구동시킬 수 있습니다.

### 환경 변수

환경 변수 **PAINTER\_ACE\_CONFIG**&#x200B;를 사용하여 사전 설정 파일의 경로를 지정할 수 있습니다. 사전 설정이 있는 경우 응용 프로그램은 항상 사전 설정 파일을 사용하여 색상 관리 설정을 구동합니다. 인터페이스에서 설정이 비활성화됩니다.

자세한 내용은 [환경 변수](../../pipeline-and-integration/configuration/environment-variables.md) 페이지를 참조하십시오.

### 사전 설정 예

아래는 사전 설정 파일에서 사용할 수 있는 json 파일의 예입니다.

```
{ 

  "color settings": { 

    "working color space": "Linear Adobe RGB (1998)", 

    "rendering intent": "Saturation" 

  }, 

  "bitmap import color space defaults" : { 

    "8 bit images": "image P3", 

    "16 bit images": "image P3", 

    "floating point images": "Raw", 

    "use embedded ICC profiles when available": false 

  }, 

  "substance material": { 

    "material color space default": "image P3" 

  }, 

  "export colors spaces" : { 

    "8 bit images": "image P3", 

    "16 bit images": "image P3", 

    "floating point images": "Raw" 

  } 

} 
```
