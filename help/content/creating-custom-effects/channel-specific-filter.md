---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/content/creating-custom-effects/channel-specific-filter.html"
breadcrumb-title: ''
description: Substance 3D Painter이 개별 텍스처 채널을 처리할 수 있도록 채널별 필터 효과를 만드는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Content > Creating custom effects > Channel specific filter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 채널별 필터
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---


# 채널별 필터

효과는 특정 채널에 따라 다를 수 있습니다. 이 경우 특정 채널에 영향을 주려면 이 채널을 식별하는 입력 및 출력을 만들어야 합니다. 일반적인 규칙으로서 입출력 구조는 항상 1:1 규칙을 존중해야 한다. 특정 채널을 입력하려면 동일한 채널을 출력해야 합니다.

**기본 색상** 채널에만 영향을 주는 필터의 예:

![](../../assets/specific-filter-basecolor.png)

>[!NOTE]
>
> 일반 설정(입력/출력 노드)과 특정 채널(기본 색상/기본 색상)을 결합할 수 없습니다.

## Alpha 구성 요소 관리

RGBA로 저장된 채널은 알파(예: 기본 색상)를 지원합니다. 이러한 채널의 경우 알파 입력/출력을 Substance 색상 출력에 바로 저장할 수 있습니다. 그러나 Substance 엔진에서는 회색 음영 이미지에 대한 Alpha을 지원하지 않습니다. 보조 맵을 사용하여 관리해야 합니다. Substance 그래프에서 특정 채널의 알파 구성 요소를 가져오려면 이름이 &#39;**channelname\_Alpha**&#39;인 회색 음영 입력을 만듭니다(예: **basecolor\_Alpha**, **거칠기\_Alpha**).\
이 알파 구성 요소를 출력하려면 동일한 이름 규칙을 사용하여 출력 노드를 만듭니다.

>[!NOTE]
>
> 채널당 특정 &quot;**\_Alpha**&quot; 출력은 일반 **재질**&#x200B;에서 작동하지 않습니다. 마스크를 사용하여 채널을 숨기려면 다음과 같은 명명 규칙을 사용하여 특정 출력을 만들어야 합니다.
> 
> * 식별자 : **채널\_Alpha**
> * 사용법: **채널\_Alpha**

## 입력/출력 용도 및 식별자 목록

>[!NOTE]
>
> 입력 노드에서 **사용량** 또는 **식별자**&#x200B;를 사용할 수 있습니다(사용량에 우선 순위가 있음).

| 채널 이름 | 사용 | 식별자/식별자 Alpha |
| --- | --- | --- |
| *주변 오클루전* | **ambientOcclusion** | **ambientOcclusion / ambientOcclusion\_Alpha** |
| *비등방성 각도* | **anisotropyangle** | **anisotropyAngle / anisotropyAngle\_Alpha** |
| *비등방성 수준* | **anisotropylevel** | **anisotropyLevel / anisotropyLevel\_Alpha** |
| *기본 색상* | **기본 색상** | **baseColor/baseColor\_Alpha** |
| *혼합 마스크* | **blendingmask** | **blendingmask / blendingmask\_Alpha** |
| *확산* | **확산** | **확산/확산\_Alpha** |
| *변위* | **변위** | **변위/변위\_Alpha** |
| *발광* | **발광** | **방출/방출\_Alpha** |
| *광택* | **광택** | **광택/광택\_Alpha** |
| *Height* | **Height** | **Height/Height\_Alpha** |
| *IOR* | **ior** | **ior / ior\_Alpha** |
| *금속* | **금속** | **금속/금속\_Alpha** |
| *표준* | **표준** | **보통/보통\_Alpha** |
| *불투명도* | **불투명도** | **불투명도/불투명도\_Alpha** |
| *반사* | **반사** | **반사/반사\_Alpha** |
| *거칠음* | **거칠음** | **거칠음/거칠음\_Alpha** |
| *분산* | **분산** | **분산/분산\_Alpha** |
| *Specular* | **Specular** | **Specular/Specular\_Alpha** |
| *Specular level* | **specularlevel** | **반사 레벨/반사 레벨\_Alpha** |
| *전송* | **전송** | **전송/전송\_Alpha** |
| *사용자 0* | **사용자0** | **사용자0/사용자0\_Alpha** |
| *사용자 1* | **사용자1** | **사용자1/사용자1\_Alpha** |
| *사용자 2* | **사용자2** | **사용자2/사용자2\_Alpha** |
| *사용자 3* | **사용자3** | **사용자3/사용자3\_Alpha** |
| *사용자 4* | **사용자4** | **사용자4/사용자4\_Alpha** |
| *사용자 5* | **사용자5** | **사용자5/사용자5\_Alpha** |
| *사용자 6* | **사용자6** | **사용자6/사용자6\_Alpha** |
| *사용자 7* | **사용자7** | **사용자7/사용자7\_Alpha** |

## 예

![](../../assets/single-channel.png){width="650px"}

이 예제에서는 회색 음영 노드를 통해 [기본 색상 알파] 채널을 추출하여 **거칠음** 채널을 덮어씁니다.

![](../../assets/mix-channel.png){width="650px"}

이 예제에서는 **거칠기** 채널을 **기본 색상**&#x200B;에 곱합니다.
