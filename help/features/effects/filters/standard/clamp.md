---
title: 클램프
description: Substance 3D Painter의 클램프 필터를 사용하는 방법을 알아보십시오.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 2%
---

# 클램프

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![클램프 아이콘](./Resources/icon_clamp.png "")

<b>인:</b> 효과/조정

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 설명

정의된 값에 대한 클램프 필터

재질의 특정 측면을 제한하기 위해 칠 레이어에서 직접 사용하거나 값을 지정된 범위로 제한하기 위해 마스크에서 사용합니다.

</td>
</tr>
</table>

>[!NOTE]
>
> 채우기 레이어에서 또는 색상 정보의 통과로 사용되는 경우 클램프는 각 색상 채널에 개별적으로 영향을 줍니다. 따라서, 주어진 픽셀의 색상이 (R 0, G 0.5, B 1.0)이고 0.5로 클램핑되면, 그 픽셀의 결과 색상은 (R 0, G 0.5, B 0.5)가 된다. 이는 Blue 채널이 클램프될 수 있을 정도의 높은 값을 가졌으나 다른 채널은 그렇지 않았기 때문이다. 이는 색상 필터가 색조 내용을 변경할 수 있음을 의미합니다.
>
>색조를 수정하지 않으려면 레벨 등 다른 필터를 사용하는 것이 좋습니다.

<a name="parameters"></a>

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| <b>분:</b> | 최소값을 조정합니다. |
| <b>최대:</b> | 최대값을 조정합니다. |
