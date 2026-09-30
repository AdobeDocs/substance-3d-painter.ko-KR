---
title: MatFX Edge Damage
description: Substance 3D Painter의 MatFX Edge Damage 필터를 사용하는 방법에 대해 알아보십시오.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 1%
---

# MatFX Edge Damage

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![MatFX 가장자리 손상 아이콘](./Resources/icon_matfx_edge_damages.png "MatFX 가장자리 손상")

<b>인:</b> 효과/흐림 효과, 회색 음영

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 설명

MatFX 가장자리 손상 필터는 벗겨진 손상된 가장자리 세부 묘사를 만듭니다. [가장자리 손상]은 [MatFX 세부 Edge Wear] 필터와 다르게 작동하므로 가장자리 손상이 손상된 영역의 색상을 변경하지 않습니다. 이는 페인팅된 금속과 같은 재료에 더 잘 사용되는 Edge Wear 보다는 플라스틱이나 수지와 같은 재료의 손상을 시뮬레이션하는 데 더 유용할 수 있음을 의미합니다.

MatFX 가장자리 손상 은 텍스처 레이어나 재질 스택에 사용되어 마모되거나 긁히거나 손상된 가장자리 세부 묘사를 추가합니다.

</td>
</tr>
</table>

>[!NOTE]
>
> MatFX 가장자리 손상 필터가 Height 채널을 수정하려면 채널에 기존 Height 데이터가 있어야 합니다. 즉, 필터 레이어 아래에 Height 데이터를 포함하는 레이어가 없으면 필터가 Height 채널에 미치는 영향을 확인할 수 없습니다.

<a name="parameters"></a>

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| <b>흐림 강도:</b> | 흐림 효과 강도를 조정합니다. |
| <b>흐림 효과 줄 바꿈:</b> | 흐림 효과 감싸기를 전환합니다. 이 효과를 활성화하면 텍스처 반대쪽의 픽셀이 샘플링됩니다. |
| <b>수준:</b> | 전체 손상 수준을 조정합니다. |
| <b>대비:</b> | 결과의 대비 또는 감소를 조정합니다. |
| <b>Scratches 강도:</b> | 스크래치 강도를 조정합니다. |
| <b>손상 거칠음:</b> | 손상된 영역의 거칠기를 조정합니다. |
| <b>손상 깊이:</b> | 손상된 영역의 깊이를 조정합니다. |
