---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/layer-stack/layer-instancing.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 레이어 인스턴싱을 사용하여 여러 텍스처 세트에서 레이어를 효율적으로 재사용하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Interface > Layer stack > Layer instancing
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 레이어 인스턴싱
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---


# 레이어 인스턴싱

**레이어 인스턴싱**&#x200B;에서는 메시 종속 결과를 계속 생성할 수 있는 동안 여러 레이어 및 [텍스처 집합](../texture-set/texture-set.md)에서 레이어 매개 변수를 동기화할 수 있습니다.

레이어 인스턴스가 만들어지면 원본 레이어(또는 소스 레이어)를 사용하여 모든 기존 인스턴스에서 매개변수를 복제합니다. **원본 레이어만 수정할 수 있습니다**.

>[!WARNING]
>
> 모든 페인트 액션(브러시 획, 다각형 칠 등) 소스 레이어가 있는 [텍스처 세트]에서만 작동합니다. 이 레이어의 인스턴스가 있는 다른 텍스처 세트는 페인트 작업을 버리기만 합니다.

## 레이어 인스턴스 만들기

레이어 인스턴스를 만들려면 다음과 같이 하십시오.

1. 기존 레이어 선택
1. 레이어 복사(**CTRL+C**)
1. 인스턴스로 붙여넣습니다(**CTRL+SHIFT+V**&#x200B;를 사용하거나 마우스 오른쪽 단추를 클릭하여 컨텍스트 메뉴를 열고 **인스턴스로 붙여넣기**&#x200B;를 선택합니다).

![](../../assets/paste-as-layer-instance.png)

>[!NOTE]
>
> 인스턴스는 **그룹**&#x200B;을 포함한 모든 레이어에서 만들 수 있습니다. 폴더를 인스턴스화하면 다양한 텍스처 세트에서 여러 레이어를 쉽게 복제할 수 있습니다. 인스턴스 폴더 내에 레이어를 추가하면 기존 인스턴스로 복제됩니다.

인스턴스가 생성되면 소스 및 대상 레이어에 새 아이콘이 표시됩니다. 이 아이콘은 텍스처 세트(아래 참조) 간에 수동으로 전환할 필요 없이 소스 레이어와 해당 인스턴스 사이를 보다 쉽게 탐색할 수 있는 버튼입니다.

| 이름 | 아이콘 |
| --- | --- |
| **인스턴스화되지 않은 레이어** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/non-instanced.png"/></div> |
| **인스턴스 원본** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/instance-source.png"/></div> |
| **인스턴스 대상** | <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c1_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/instance-target.png"/></div> |

## 텍스처 세트 간에 인스턴스 만들기

여러 텍스처 세트에서 레이어 인스턴스를 한 번에 만들 수 있으므로 수동으로 복사하거나 붙여넣지 않아도 됩니다.

여러 텍스처 세트에서 인스턴스를 만들려면 다음을 수행하십시오.

1. 기존 레이어 선택
1. 레이어를 마우스 오른쪽 버튼으로 클릭하여 컨텍스트 메뉴를 엽니다
1. **텍스처 집합 간에 인스턴스화**&#x200B;를 선택합니다.
1. 새 창에서 인스턴스를 받아야 하는 텍스처 세트를 선택합니다.
1. 확인을 눌러 인스턴스를 검증하고 생성합니다.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../assets/instance-across-texture-sets.png)

</td>
<td style="border: 0;" valign="top">

![](../../assets/instance-across-texture-sets-dialog.png)

</td>
</tr>
</table>

>[!NOTE]
>
> 텍스처 집합 이름 옆의 느낌표는 채널 **불일치**&#x200B;를 나타냅니다. 이것은 인스턴스가 이 텍스처 세트에서 만들어지면 채널이 없기 때문에 올바르게 렌더링되지 않는다는 것을 의미합니다.

## 인스턴스와 해당 소스 간 전환

기술적인 이유로 인해 인스턴스는 **소스 편집**&#x200B;을 통해 **전용**&#x200B;으로 업데이트할 수 있으므로 속성을 편집하려면 소스 레이어를 선택해야 합니다.\
이 작업은 레이어 스택의 레이어에서 **인스턴스 속성 버튼**&#x200B;을 클릭하여 수행할 수 있습니다.

![](../../assets/instance-properties-optim.gif)

인스턴스 속성 단추를 클릭하면 **속성 창**&#x200B;이 현재 도구/레이어에서 **목록**(소스 레이어 및 해당 인스턴스 표시)으로 전환됩니다.\
목록의 **모든 요소**&#x200B;를 클릭하여 자동으로 **이 레이어로 이동** 합니다. 그러면 현재 **선택한 텍스처 집합이 자동으로**&#x200B;변경&#x200B;**되며**&#x200B;도 오른쪽 집합으로 변경됩니다.

**인스턴스 트리** 목록을 사용하면 동시에 **종속성**&#x200B;을 보면서 인스턴스에서 해당 소스로 **빠르게** 이동하는 가장 좋은 방법입니다.

## 인스턴스 주기(및 해결 방법)

사이클은 소스 레이어 자체에 직접 또는 간접적으로 사용되는 인스턴스입니다. Substance 3D Painter 엔진에서 주기 **을(를) 계산할 수 없습니다**. 따라서 고정 또는 제거할 때까지 **사용 안 함**&#x200B;해야 합니다.

예:\
![](../../assets/instance-cycle-optim.gif)

이 예제에서는 소스 레이어의 인스턴스가 폴더이므로 해당 인스턴스로 이동됩니다. 인스턴스를 생성하려면 인스턴스의 매개 변수에 따라 달라지는 소스의 매개 변수를 쿼리해야 하므로 인스턴스가 손상됩니다. 이것은 자동적으로 해결될 수 없는 순환을 만든다. 인스턴스가 비활성화됩니다.

주기를 수정하는 유일한 방법은 폴더 밖으로 인스턴스를 **이동**&#x200B;하거나 인스턴스를 **삭제**&#x200B;하는 것입니다.

레이어 인스턴스는 인스턴스 자체가 다른 소스 레이어를 참조하는 한 소스 레이어에서 사용할 수 있습니다.
