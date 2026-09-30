---
title: PBR 유효성 검사
description: Substance 3D Painter의 PBR 유효성 검사 필터 사용 방법을 알아봅니다.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 2%
---

# PBR 유효성 검사

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![PBR 유효성 검사 아이콘](./Resources/icon_pbr_validate.png "PBR 유효성 검사")

<b>내부:</b> 효과/pbr, 금속성, 거칠음

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 설명

상기 PBR 유효성 검사 필터는 알베도 암부 값 및 금속 반사율 범위를 확인하여 PBR 데이터를 검증한다.

이 레이어는 채우기 레이어에서 재질 값이 예상 PBR 범위 내에 유지되는지 확인하는 데 사용됩니다. 재질을 내보낼 때는 PBR 유효성 검사를 사용하도록 설정해서는 안 됩니다.

</td>
</tr>
</table>

<a name="parameters"></a>

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| <b>유효성 검사 모드:</b> | 알베도, 금속 반사율을 검증할지 또는 둘 다 검증할지 선택합니다. |
| <b>알베도 어두운 범위 임계값:</b> | 알베도 유효성 검사에 허용되는 최소 어두운 값 임계값을 선택합니다. |
| <b>금속 반사율 범위:</b> | 금속값을 검증하는 데 사용할 반사도 범위를 선택합니다. |
| <b>오버레이 맵:</b> | 맵 데이터 위에 유효성 검사 오버레이를 전환합니다. |

