---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/color-profile.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 색상 프로필 후처리를 사용하여 색상 그레이딩 및 LUT 변형을 적용하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Color Profile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 색상 프로필
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---


# 색상 프로필

![](../../assets/doc-lut-example.jpg){width="700px"}

Substance 3D Painter에서 **LUT** 텍스처를 로드하여 **뷰포트**&#x200B;에 **색상 프로필**&#x200B;을 할당할 수 있습니다.\
색상 프로필은 특정 카메라와 같은 대상을 일치시키기 위해 화면의 최종 색상을 교정하는 데 사용할 수 있습니다. 프로필이 밝기, 감마, 대비 또는 색상 균형을 변경하여 색상을 조정하는 경우가 많습니다.

>[!NOTE]
>
> **LUT**&#x200B;은 &quot;**테이블 찾기**&quot;을(를) 나타냅니다. 사후 효과로 색 보정을 수행하는 최적화된 방법입니다. LUT는 소스와 결과 사이의 차이를 구성하는 데 사용됩니다.\
>  Substance 3D Painter에서는 가능한 모든 해상도의 **2D 텍스처**(부동)으로 저장된 **3D** LUT를 사용합니다(기본값은 **2048x128 픽셀** ). 즉, 색상 작업을 저장하는 육면체가 나란히 표시되는 분할 영역으로 분리됩니다. 자세한 기술 정보는 **GPU Gem** 문서 <http://http.developer.nvidia.com/GPUGems2/gpugems2_chapter24.html>을(를) 참조하십시오.

## 색상 프로파일 사용

디스플레이 설정 창을 통해 색상 프로필을 로드할 수 있습니다.\
뷰포트에 영향을 주고 색상 프로필을 활성화하려면 &quot; **색상 프로필 활성화**&quot; 확인란을 선택합니다.

![](../../assets/color-profile-ui.png)

* &quot;색상 프로필 활성화&quot;가 **비활성화**&#x200B;된 경우 재질 보기(일부 특정 채널의 경우 선형)의 경우 뷰포트 렌더링은 **sRGB**&#x200B;에서 수행됩니다
* &quot;Activate Color Profile&quot;이 **enabled**&#x200B;인 경우 뷰포트 렌더링은 모든 보기(솔로 채널 포함)에 대해 **Linear/Raw**&#x200B;에서 수행됩니다

LUT 텍스처가 리소스 슬롯에 로드되면 **질감 모드**&#x200B;에 있을 때 뷰포트의 렌더링을 조작하는 데 사용됩니다.\
그렇지 않으면 렌더링이 [선형/원시]로 표시됩니다(예: 솔로 채널 보기).

**흰 점** 설정을 사용하여 (LUT가 적용되기 전에) 입력 이미지의 톤 매핑을 변경할 수 있습니다.\
예를 들어 태양을 보고 있는 경우 값은 1(기본값)보다 커야 합니다. 완벽한 노출을 위해서는 흰 점을 이미지의 높은 값으로 설정해야 합니다.

흰 점 수식은 다음과 같습니다.

```
float Value = 1.0f / WhitePoint; // Value from the user interface 

float3 Output = clamp( HDR.rgb * Value, 0.0f, 1.0f );
```


색상 프로필을 사용하기 전에 특정 톤 매핑을 적용할 수 있습니다. [톤 매핑](tone-mapping.md)에서 사용할 수 있는 함수를 확인하십시오.\
Substance 3D Painter에서 흰 점 설정 이외의 다른 입력 색상을 처리하지 않습니다. 예를 들어 적용된 Shaper LUT는 없습니다.

## 색상 프로필 만들기

Substance 3D Painter은 &quot;**색상 프로필 활성화**&quot;가 활성화되면 뷰포트를 **선형** 렌더링으로 이동합니다. 즉, LUT가 적용될 때 선형 프로필에서 원하는 대상으로 색상을 변환해야 합니다.

### 방법 1 : ID LUT 수정

신원 LUT 편집은 <b>Substance 3D Designer</b>와 같은 <b>32비트 부동</b> 텍스처를 지원하는 소프트웨어에서 수행할 수 있습니다. 새 프로필을 만들기 위한 시작점으로 ID LUT를 다운로드합니다.

[color\_profile\_linear.exr 다운로드](https://github.com/AdobeDocs/painter-python-api/raw/refs/heads/main/static/misc/color_profile_linear.exr)

### 방법 2 : OpenColor IO를 사용하여 LUT 텍스처 생성

**OpenColor IO** 도구를 설치합니다. 그런 다음 <http://opencolorio.org/downloads.html>에서 사용할 수 있는 샘플 OCIO 구성을 다운로드합니다.\
여기에서 다음 인수를 사용하여 **ociolutimage** 프로그램을 실행합니다.

```
ociolutimage --generate --cubesize 64 --config nuke-default/config.ocio --colorconvert linear srgb --output lutLinearToSRGB.exr
```


**참고**: 이 LUT에 색상 변환을 적용하기 위해 **ocioconvert** 프로그램을 사용하여 **OpenColor IO**&#x200B;로 ID LUT를 수정할 수도 있습니다.

### 새 색상 프로필 가져오기

간단히 가져오기 창을 열거나 LUT를 선반에 드래그하여 놓습니다. Substance 3D Painter에서 LUT 텍스처를 가져올 때 새 리소스에 &quot; **colorlut** &quot; **사용량**&#x200B;을 할당해야 합니다. 그렇지 않으면 리소스가 선반에 제대로 표시되지 않습니다.

자세한 내용은 새 리소스 가져오기에 대한 설명서를 참조하십시오. [가져오기 창을 통해 리소스 추가](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/adding-content-via-the-import-window-151584824.html)
