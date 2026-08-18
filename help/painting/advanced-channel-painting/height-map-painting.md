---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/painting/advanced-channel-painting/height-map-painting.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 직접 Height 맵을 페인트하여 변위 및 표면상승 효과를 만드는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Painting > Advanced channel painting > Height Map Painting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Height 맵 페인팅
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---


# Height 맵 페인팅

## 일반 아이디어

일반 작업을 직접 수행하는 대신 하이맵을 사용하면 품질 향상, 제어 기능 향상, 유연성, 에셋 간의 일관성 향상과 같은 여러 가지 이점을 얻을 수 있습니다.

프로세스는 다음과 같습니다.

* 높은 폴리 메쉬로부터 베이킹되는 정상 맵이 낮은 폴리 메쉬 상에 로딩된다.
* 하이트맵 채널에 추가 세부 사항을 페인팅합니다.
* 페인트한 Height은 모든 레이어를 통해 합성되고 실시간으로 표준 맵으로 변환되며, 최종적으로 높은 폴리 메쉬에서 표준과 혼합됩니다.

Height 페인팅만 하면 나머지 모든 작업은 자동으로 수행됩니다.

### HDR 형식 Height

Height 채널은 **HDR** 색상 형식을 사용하므로 채도가 0에서 255 사이인 기존의 Height 맵과는 달리 밝기의 한계에 도달하지 않고도 양수 및 음수 값을 페인팅할 수 있습니다.

* Height에서 비트맵 또는 Substance로 페인팅하면 해당 소스가 원래 [0,255] 범위에서 [-1,1] 범위로 다시 매핑됩니다.

중간 회색은 0으로 다시 매핑됩니다. 따라서 127 미만의 값은 하이트맵에서 **빼기**&#x200B;되고, 127 이상의 값은 Height 맵에 설정된 기본 혼합 모드 **선형 닷지(추가)**&#x200B;를 사용할 때 하이트맵에 **추가**&#x200B;됩니다.

* 일반 색상으로 페인트할 때 -1과 1 사이의 값을 직접 선택할 수 있습니다.

### Height 시각화

[단독] 모드에서 Height 맵을 시각화할 때 기본 미리 보기에는 양수 값만 표시되며 음수 값에는 강한 검정 채도가 표시됩니다.

**+/- 색상** 설정을 사용하면 양수 값과 음수 값에 대해 다른 색상을 사용하여 전체 범위를 시각화할 수 있습니다.

**비율** 설정을 사용하면 기본 [-1,1] 범위보다 많이 추가하거나 뺀 경우 해당 HDR 맵의 표시 범위를 수정할 수 있습니다.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/height1.png)

</td>
<td style="border: 0;" valign="top">

![](../../assets/height2.png)

</td>
</tr>
</table>
