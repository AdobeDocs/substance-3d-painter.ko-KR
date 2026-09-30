---
title: Height 조정
description: Substance 3D Painter의 Height 조정 필터를 사용하는 방법에 대해 알아봅니다.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 1%
---

# Height 조정

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![Height 조정 아이콘](./Resources/icon_height_adjust.png "Height 조정")

<b>인:</b> 효과/조정, 크기 조정, 오프셋, 반전

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 설명

[Height 조정] 필터는 Height 채널을 선택한 값으로 반전, 오프셋 또는 곱합니다.

이 효과는 텍스처 레이어나 마스크 내부(흑백 출력)에 사용되어 Height 정보를 비파괴적으로 조정합니다.

</td>
</tr>
</table>

<a name="parameters"></a>

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| <b>반전:</b> | 결과의 반전을 토글합니다. |
| <b>오프셋:</b> | 지정된 양을 더하거나 빼면서 Height 값을 조정합니다. |
| <b>곱하기:</b> | Height 값에 이 값을 곱합니다. 이는 승수로서 높은 영역은 더 높게, 낮은 영역은 더 낮게 만든다. |

>[!NOTE]
>
> 오프셋이 먼저 적용된 **곱하기** 및 **오프셋** 매개 변수 스택입니다. 만약 오프셋의 결과로 주어진 점에서 Height 값이 0이 되면, 곱은 0으로 곱해진다. 이것은 그 점에서 아무런 변화가 일어나지 않는다는 것을 의미한다. 곱하고 곱해진 값을 오프셋하려면 두 번째 Height 조정 필터를 추가합니다.
