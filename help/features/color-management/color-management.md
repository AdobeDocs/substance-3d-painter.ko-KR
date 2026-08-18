---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/features/color-management.html"
breadcrumb-title: ''
description: 작업 과정에서 일관된 색상 정확도를 보장하기 위해 Substance 3D Painter에서 색상 관리를 구성하는 방법에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Painter > Features > Color management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 색상 관리
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 4%

---


# 색상 관리

![](../../assets/banner-cm-doc.jpg)

색상 관리는 색상을 처리하고 변환하는 것입니다. 리소스 가져오기에서 화면에 색상 표시, 마지막으로 텍스처 내보내기에 이르기까지 다양한 기능을 지원합니다. 색상 보정은 여러 응용 프로그램에서 동일한 모양을 보장하기 위해 중요합니다.

응용 프로그램 색상 관리는 [OpenColorIO](https://opencolorio.org/)&#x200B;(단어의 경우 OCIO) 버전 2의 통합을 통해 처리됩니다. OCIO는 색상을 변환하고 표시하는 필름 및 애니메이션 분야의 표준입니다. 색상 관리를 활성화하려면 새 프로젝트를 만들거나 기존 프로젝트를 열고 전용 설정을 활성화하기만 하면 됩니다.

>[!NOTE]
>
> 색상 관리는 7.4.0 버전 이후에 사용할 수 있습니다.

## 프로젝트 설정

색상 관리 설정:

* [Adobe ACE를 사용한 색상 관리 - ICC](color-management-with-adobe-ace-icc.md)
* [OpenColorIO를 사용한 색상 관리](color-management-with-opencolorio.md)

## 어휘

연관된 작업 과정을 더 잘 이해하려면 색상 관리와 관련된 몇 가지 기술 용어를 아는 것이 도움이 될 수 있습니다.

| 키워드 | 설명 |
| --- | --- |
| **색상 공간** | 색상이 정의된 좌표계입니다. |
| **작업 영역** | 텍스처, 페인트 등을 혼합하기 위해 응용 프로그램 내부에서 사용되는 색상 공간입니다. |
| **변환 표시** | 디스플레이 변환은 작업 공간에서 모니터의 색상 공간으로 선형 색상을 변환하여 육안으로 볼 수 있도록 색상을 지각하여 표시합니다. 표시 변형에는 대개 톤매핑 패스가 포함되어 있어 화면에서 허용하는 제한된 값 범위에 맞게 색상을 압축합니다. |
| **구성** | OCIO 구성 파일입니다. 작업 영역, 색상 공간 목록, 표시 변형 목록을 정의합니다. |
| **ACES** | ACES는 Academy Color Encoding System을 의미하며 디지털 이미지 파일을 교환하는 많은 응용 프로그램에서 표준입니다. 이 표준의 두 버전은 기본적으로 응용 프로그램 내에 포함되어 있습니다. |
| **톤 매핑** | HDR(High Dynamic Range)에서 LDR(낮은 동적 범위)로 색상 값을 매핑하는 프로세스입니다. 이 프로세스를 통해 넓은 범위의 색상을 대략적으로 표시할 수 있습니다. |

## 색상 관리 채널 목록

애플리케이션 내에서 색상이 관리되는 채널과 관리되지 않는 채널(데이터/패스스루)이 미리 정의되어 있습니다.

| 채널 | 색상 관리 여부 |
| --- | --- |
| **주변 오클루전** | 아니요 |
| **음이온화각** | 아니요 |
| **비등방성 수준** | 아니요 |
| **기본 색상** | **예** |
| **혼합 마스크** | 아니요 |
| **코트 색상** | **예** |
| **정상 외투** | 아니요 |
| **코트 불투명도** | 아니요 |
| **코트 거칠음** | 아니요 |
| **코트 Specular level** | 아니요 |
| **확산** | **예** |
| **변위** | 아니요 |
| **광택** | 아니요 |
| **Height** | 아니요 |
| **Ior** | 아니요 |
| **금속** | 아니요 |
| **표준** | 아니요 |
| **불투명도** | 아니요 |
| **반사** | 아니요 |
| **거칠음** | 아니요 |
| **분산** | 아니요 |
| **색상 분산** | **예** |
| **광택 색상** | **예** |
| **광택 불투명도** | 아니요 |
| **광택 거칠음** | 아니요 |
| **Specular** | **예** |
| **Specular edge color** | **예** |
| **Specular level** | 아니요 |
| **투명도** | 아니요 |
| **전송** | **예** |
| **사용자 X(0-15)** | [텍스처 집합 설정](../../interface/texture-set/texture-set-settings.md)에 종속됩니다. 기본적으로 사용자 채널은 색상 관리를 사용하지 않습니다. <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r31-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/user-demo.png"/></div> |

## 색상 피커

색상 관리를 사용하도록 설정하면 [색상 피커](../../interface/color-picker.md) 동작이 약간 변경됩니다.

* 색상은 선택한 현재 디스플레이를 기준으로 편집됩니다.
* 인터페이스에 몇 가지 추가 정보가 추가됩니다.

자세한 내용은 색상 피커 [문서 페이지](../../interface/color-picker.md)를 참조하세요.

## 뷰포트 컨트롤

2D 및 3D 보기는 모두 색상 관리되며 뷰포트 상단에서 사용할 전용 설정을 사용하여 어떤 디스플레이 변형을 제어할 수 있습니다.

![](../../assets/viewport-cm.png)

* **왼쪽 단추**: 뷰포트의 디스플레이 변형을 활성화/비활성화합니다. 비활성화된 경우 뷰포트에 색상이 원시/패스스루로 표시됩니다. 이 버튼은 기본적으로 활성화되어 있습니다.
* **오른쪽 드롭다운**: 색상을 변환하여 화면에 표시하는 데 사용할 표시 변형을 지정합니다. 기본값은 OCIO 구성을 기준으로 합니다. 이 설정은 모니터에 종속될 수 있으므로 프로젝트와 함께 저장되지 않습니다.

>[!NOTE]
>
> 단독 모드(개별적으로 채널 보기)에서는 데이터 채널을 볼 때 색상 관리가 자동으로 비활성화됩니다(위 목록 참조).

## 내보내기 설정

기본 내보내기 설정은 프로젝트 구성에 의해 결정됩니다(위 참조).

[텍스처 내보내기](../../export/export.md) 창에는 텍스처당 사용된 색상 공간 **$colorSpace**&#x200B;의 파일 이름에 추가하는 데 사용할 수 있는 키워드가 있습니다.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/export-list-1.png){width="320px"}

</td>
<td style="border: 0;" valign="top">

![](../../assets/export-list-2.png){width="500px"}

</td>
</tr>
</table>

## 색상 공간 재정의

리소스가 기본값과 달라지도록 대체 색상 공간을 지정해야 할 수 있습니다. 색상 공간 메뉴를 통해 이 작업을 수행할 수 있습니다.

### 리소스의 색상 공간 변경

[속성 창](../../interface/properties.md) 내에서 특정 리소스(현재 사용되는 위치)의 색상 공간을 재정의할 수 있습니다.

이렇게 하려면 색상 공간 섹션을 확장하고 드롭다운을 사용하여 새 색상 공간을 지정합니다.

![](../../assets/color-space-menu.png)

### 환경 맵의 색상 공간 변경

[표시 설정](../../interface/display-settings/display-settings.md) 내에서 **환경 맵 색상 공간 재정의**&#x200B;를 사용하도록 설정한 다음 목록에서 리소스와 일치하는 색상 공간을 선택합니다.

![](../../assets/color-sace-menu-env.png)
