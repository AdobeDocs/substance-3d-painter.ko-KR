---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/workflow-issues/export-issues/texture-dilation-or-padding.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 텍스처 확장 및 패딩을 사용하여 내보낸 텍스처에서 가장자리 아티팩트를 방지하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Export Issues > Texture dilation or Padding
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 텍스처 확장 또는 패딩
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---


# 텍스처 확장 또는 패딩

**패딩**(**확장**&#x200B;이라고도 함)은 텍스처 생성 후 발생하는 프로세스입니다. 이는 UV 섬의 테두리를 확장하여 빈 영역을 유사한 픽셀로 채우는 데 사용됩니다.

좋은 품질의 패딩을 생성하는 것은 나중에 게임 엔진이나 오프라인 렌더러가 [밉맵](../../../getting-started/glossary.md)을 잘 생성하도록 하는 데 중요합니다.\
Substance 3D Painter에서는 무한 패딩을 생성할 수 있습니다. 즉, 픽셀이 텍스처의 다른 UV 섬에 도달하거나 경계에 도달할 때까지 늘리다가 생성됩니다.

## 무한 패딩 생성

다음은 무한 패딩의 작동 방식에 대한 예입니다.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/padding.gif){width="512px"}

</td>
<td style="border: 0;" valign="top">

![](../../../assets/padding-zoom.gif)

</td>
</tr>
</table>

## MipMap

3D 컴퓨터 그래픽에서 **밉맵**&#x200B;은 미리 계산되어 최적화된 텍스처 시퀀스입니다. 각 프로필은 동일한 이미지의 저해상도 표현입니다. 이 효과는 렌더링 속도를 높이고 앨리어싱 아티팩트를 줄이기 위한 것입니다. 카메라에 가까운 객체에는 고해상도 밉맵 이미지가 사용됩니다. 저해상도 이미지는 개체가 더 멀리 나타날 때 사용합니다. 이는 대신 렌더링하는 효율적인 방법이며 원본 텍스처에서 모든 픽셀을 읽을 수 있습니다. 밉맵(각 레벨)은 파일 형식에서 지원하는 경우 텍스처 자체에 포함됩니다.

패딩은 텍스처 해상도를 낮출 때 메시의 UV 내에서 잘못된 색상이 번지지 않도록 하기 때문에 밉맵에 매우 중요합니다.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/mipmap-padding.gif){width="400px"}

</td>
<td style="border: 0;" valign="top">

![](../../../assets/mipmap-nopadding.gif){width="400px"}

</td>
</tr>
</table>

위의 예시에서 회색 배경은 UV에 번지고(오른쪽 이미지), 패딩은 색상을 깔끔하게 유지합니다(왼쪽 이미지).

3D 애플리케이션 내에서 이러한 결과는 다음과 같습니다.

![](../../../assets/padding-toggle.gif)

## 패딩 컨트롤

Substance 3D Painter에서는 다른 위치에서 패딩 생성 동작(예: 비활성화)을 변경할 수 있습니다.

* **굽는 중**: 자세한 내용은 [굽기 설명서](../../../baking/baking.md)를 참조하십시오.
* **텍스처 집합에 대한 텍스처를 생성할 때**: 자세한 내용은 [텍스처 집합 설정](../../../interface/texture-set/texture-set-settings.md) 설명서를 참조하십시오.
* **텍스처를 내보낼 때**: 자세한 내용은 [내보내기 설정](../../../export/export-window/export-window.md) 설명서의 &quot;패딩 설정&quot; 섹션을 참조하세요.
