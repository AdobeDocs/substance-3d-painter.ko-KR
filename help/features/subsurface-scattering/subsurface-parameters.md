---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/subsurface-scattering/subsurface-parameters.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 서브서피스 스캐터링 매개변수를 구성하여 사실적인 반투명 재질을 만드는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Features > Subsurface Scattering > Subsurface Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 서브서피스 매개변수
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---


# 서브서피스 매개변수

Substance 3D Painter 실시간 서브서피스 구현은 스크린-공간 서브서피스 스캐터링 효과입니다. 이를 제어하는 매개변수에 대해서는 이 페이지에서 설명합니다.\
현재 구현은 PIXAR에서 [발표한 ](http://graphics.pixar.com/library/ApproxBSSRDF/)효율적인 서브표면 산란을 위한 대략적인 반사도 프로파일&quot;방법을 기반으로 합니다.

이러한 매개 변수를 기반으로 한 재질 예제는 [표면 아래 재질 유형](subsurface-material-type.md)을 참조하세요.

## 셰이더/MDL 매개 변수

![](../../assets/shader-parameters.png)

[셰이더 설정](../../interface/shader-settings/shader-settings.md) 창에서 사용할 수 있습니다.

| *설정* | *설명* |
| --- | --- |
| **사용** | 이 셰이더/mdl 인스턴스에서 서브서피스 분산 효과를 활성화하거나 비활성화합니다.  필요하지 않은 재질에 SSS 효과를 사용하지 않도록 설정하는 데 사용할 수 있습니다. |
| **분산 유형** | 재질에 있는 조명 흡수의 동작을 정의합니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong> 반투명</strong>: 빛이 개체 내부로 깊이 침투할 수 있는 옥이나 대리석과 같은 일반 재질에 적합합니다.</li><li data-preserve-html="true"><strong> 피부</strong>: 빛이 빠르게 흡수되고 표면 근처의 산란으로 유지되는 유기적인 피부에 적합합니다.</li><li data-preserve-html="true"><strong>적색 이동/광선</strong>: 사람 또는 생물의 표면 피부를 시뮬레이션하는 피부 설정보다 더 정확합니다.</li></ul> |
| **크기 조절** | 재질에 있는 조명 흡수의 반경/깊이를 제어합니다. 이 매개 변수 동작은 장면에 있는 메쉬의 크기에 따라 달라집니다.사람 크기의 머리에 0.0, 0.2 및 1.0 척도의 비교:   <div><img data-preserve-html="true" src="../../assets/scale-sss.jpg" width="650"/></div> |
| **색상** | 재료에 흡수될 때의 빛의 색상입니다.세 가지 색상 비교 :   <div><img data-preserve-html="true" src="../../assets/color-sss.jpg" width="650"/></div> |

### 디스플레이 설정 매개변수

![](../../assets/display-settings-1.png)

[표시 설정](../../interface/display-settings/display-settings.md) 창에서 사용할 수 있습니다.

>[!NOTE]
>
> 이 매개 변수 **은(는) 하위 표면 분산 효과의**&#x200B;실시간&#x200B;**버전에만 영향을 줍니다**.

| *설정* | *설명* |
| --- | --- |
| **샘플 수** | 화면 공간에서 하위 표면 흐림 효과를 생성하기 위해 수행할 샘플 양을 제어합니다. 샘플이 많을수록 노이즈가 적지만 성능에 영향이 있습니다.표면을 가까이 볼 때 8, 32 및 64 샘플 간의 비교 :   <div><img data-preserve-html="true" src="../../assets/samples-sss-v2.jpg" width="650"/></div>  **참고:** 샘플의 양을 늘리지 않고 [카메라 설정](../../interface/display-settings/camera-settings.md)을 사용하도록 설정하면 노이즈의 양을 줄일 수도 있습니다. |
