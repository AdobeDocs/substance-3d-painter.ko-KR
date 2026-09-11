---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/content/creating-custom-effects/mesh-based-input.html"
breadcrumb-title: ''
description: Substance 3D Painter의 사용자 정의 효과에서 메쉬 기반 입력을 사용하여 모양 인식 텍스처 효과를 만드는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Mesh Based Input
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메시 기반 입력
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 1%

---


# 메시 기반 입력

망 기반 입력은 Substance 3D Painter 엔진이 현재 프로젝트 내의 망에서 추출한 텍스처를 제공합니다. 이러한 텍스처를 사용하여 메시 토폴로지를 기반으로 고급 효과를 만들 수 있습니다.

>[!NOTE]
>
> 이러한 메시 정보는 토폴로지 자체를 기반으로 하며 메시 맵(구운 텍스처)을 고려하지 않습니다.
> 
> 엔진에 의해 제공된 입력은 Substance 그래프에서 입력의 값으로 다운스케일/클램핑될 32 비트 부동 소수점 텍스처가다.

| 메시 정보 | 식별자 | 사용 | 설명 |
| --- | --- | --- | --- |
| *위치(RGB)* | **메시\_위치** | **meshPosition** | 교점 위치를 포함하는 텍스처를 읽어들입니다. |
| *월드 스페이스 표준(RGB)* | **mesh\_world\_space\_normal** | **meshNormalWS** | 월드 공간에서 교점 수직을 포함하는 텍스처를 읽어들입니다. |
| *월드 공간 접선(RGB)* | **mesh\_world\_space\_tangent** | **meshTangentWS** | 월드 공간에서 교점 탄젠트를 포함하는 텍스처를 읽어들입니다. |
| *월드 스페이스 비트 전송률(RGB)* | **mesh\_world\_space\_bitangent** | **meshBitangentWS** | 월드 공간에서 정점 bi-tangent(bi-normal)를 포함하는 텍스처를 검색합니다. |
| *텍스트 크기(회색 음영)* | **메시\_텍셀\_크기** | **meshTexelSize** | 텍셀 크기(픽셀 밀도와 메쉬 UV의 차이)를 포함하는 텍스처를 읽어들입니다. |
| *UV 마스크(회색 음영)* | **메시\_uv\_mask** | **meshUVMask** | 망 UV 섬의 텍스처를 검은색(외부) 및 흰색(내부) 마스크로 읽어들입니다. |
