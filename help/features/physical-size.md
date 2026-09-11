---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/physical-size.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 물리적 크기를 설정하여 정확한 텍스처 비율을 위한 실제 치수를 정의하는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Features > Physical size
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 실제 크기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 2%

---


# 실제 크기

![](../assets/banner-physicalsize-2.png)

물리적 크기는 Substance 재질 내부의 속성으로 실제 크기를 정의합니다. 3D 표면에 걸쳐 재료의 크기와 모양을 정확하게 일치시키는 데 사용할 수 있습니다. Painter은 센티미터를 기본 내부 단위로 사용합니다.

물리적 크기를 사용하려면 이 속성이 0,0,0이 아닌 값을 가지는 재질을 적용한 다음 UV 변형 > 비율 조정 아래의 레이어(또는 효과)에서 물리적 크기 모드를 활성화하십시오.

자세한 내용은 다음 항목을 참조하세요.

* [채우기 예측](../painting/fill-projections/fill-projections.md)의 <b>물리적 크기</b> 매개 변수
* [뷰포트 설정](../interface/display-settings/viewport-settings.md)의 <b>격자</b> 매개 변수
* [셰이더 설정](../interface/shader-settings/shader-settings.md)의 <b>물리적 크기 기반 변위</b>

>[!NOTE]
>
> * Painter 버전 8.3에서는 모든 유형의 투영에 대해 물리적 크기를 사용할 수 있습니다.
> * 대부분의 메시 파일 형식은 메시 생성 중에 사용되는 단위를 지정합니다. 이 단위는 가져오기 중에 자동으로 센티미터로 변환됩니다.
> * .obj와 같은 일부 형식에는 단위 정보가 없으므로 .obj 메시를 사용하여 프로젝트를 만들면 변환 없이 기본적으로 센티미터 단위로 측정됩니다.
