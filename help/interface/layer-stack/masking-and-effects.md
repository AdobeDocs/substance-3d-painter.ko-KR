---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/interface/layer-stack/masking-and-effects.html"
breadcrumb-title: ''
description: Substance 3D Painter 레이어 스택에서 마스크 및 효과를 사용하여 레이어 가시성을 제어하고 레이어 효과를 적용하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Masking and effects
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 마스크 및 효과
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---


# 마스크 및 효과

## 마스크

레이어는 텍스처의 특정 부분에만 내용을 표시/적용하기 위해 마스킹할 수 있습니다. 마스크는 레이어 콘텐츠에 대해 강도 매개 변수로 작동합니다. 어떤 내용을 사용하여 마스크에 페인트를 지정하든 레이어의 마스크는 항상 회색 음영으로 표시됩니다. 따라서 모든 색상은 칠하기 전에 회색 음영 값으로 변환됩니다.

마우스 오른쪽 버튼을 클릭하거나 전용 버튼 을 사용하여 마스크를 추가할 수 있습니다.

![](../../assets/layer-mask.gif)

마스크에 대해 가능한 작업 :

* 마스크 축소판에서 **ALT + 왼쪽 마우스 클릭**&#x200B;하면 마스크 자체를 시각화할 수 있습니다. 그러면 뷰포트가 이 레이어에서 마스크의 격리된 보기로 전환됩니다. 이 작업은 뷰어 설정을 통해서도 사용할 수 있습니다.
* 축소판에서 **SHIFT+왼쪽 마우스 클릭**&#x200B;을 수행하면 마스크를 일시적으로 사용하지 않도록 설정할 수 있습니다. 동일한 작업을 다시 실행하여 다시 활성화합니다. 이 작업은 마우스 오른쪽 버튼 클릭 메뉴(&quot;마스크 전환&quot;)를 통해서도 가능합니다.
* 축소판 위로 **마우스 오른쪽 단추 클릭 > 마스크 내용 복사**&#x200B;를 수행한 다음 두 번째 마스크의 축소판에서 **마우스 오른쪽 단추 클릭 > 마스크에 붙여넣기**&#x200B;를 수행하여 마스크 내용을 다른 마스크로 복사할 수 있습니다.
* **마우스 오른쪽 버튼 클릭 > 마스크 배경 반전**&#x200B;을 수행하면 마스크 배경을 반전할 수 있습니다. 이 기능은 마스크에 첨부된 효과가 손상되지 않도록 하려는 경우에 유용합니다.

>[!WARNING]
>
> 마스크를 다시 추가하거나 제거하면 마스크 및 마스크에 연결된 모든 효과가 제거됩니다.

**CTRL** 키를 누르면 드래그하여 놓기를 통해 칠 레이어를 만들 때 마스크를 즉시 만들 수 있습니다.

![](../../assets/mask-material-optimized.gif)

## 효과

효과는 언제든지 편집할 수 있는 특수 작업입니다. 효과는 레이어 내용의 마스크에 배치할 수 있습니다.\
따라서 효과는 다른 효과보다 효과에서 더 적절합니다. 예를 들어 &quot;generators&quot;는 마스크에 적합합니다.

레이어의 각 축소판 아래에 있는 선은 효과가 존재하는지 여부를 나타냅니다. 회색은 효과가 없고 빨간색은 적어도 하나의 효과와 같습니다. 마스크 및 콘텐츠 각각에 대한 효과 스택이 있습니다.

![](../../assets/effect.gif)

자세한 내용은 [전용 페이지](../../features/effects/effects.md)를 참조하세요.

## 스마트 마스크

스마트 마스크는 마스크 및 해당 효과를 저장하여 다른 레이어나 다른 프로젝트에서 쉽게 다시 사용할 수 있는 방법입니다. 스마트 마스크를 만들려면 마스크를 마우스 오른쪽 단추로 클릭하고 &quot;**스마트 마스크 만들기**&quot;를 선택하면 됩니다.\
스마트 마스크를 레이어로 드래그하여 놓을 때 없는 경우에는 검정 마스크가 만들어지고, 없는 경우에는 효과 목록이 기존 마스크에 병합됩니다. 스마트 마스크를 놓을 때 &quot;**CTRL**&quot;을(를) 눌러 효과 목록을 완전히 덮어쓸 수 있습니다.

![](../../assets/smart-mask-new-optimized.gif)

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/smart-mask-add-optimized.gif)

</td>
<td style="border: 0;" valign="top">

![](../../assets/smart-mask-overwrite-optimized.gif)

</td>
</tr>
</table>
