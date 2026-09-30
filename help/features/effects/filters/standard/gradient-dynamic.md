---
title: 동적 그레이디언트
description: Substance 3D Painter의 그레이디언트 동적 필터를 사용하는 방법에 대해 알아봅니다.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 4%
---

# 동적 그레이디언트

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![동적 그레이디언트 아이콘](./Resources/icon_gradient_dynamic.png "동적 그레이디언트")

<b>내부:</b> 효과/그레이디언트, 회색 음영, 다시 매핑

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 설명

[그레이디언트 동적] 필터는 이미지의 회색 음영 값을 그레이디언트를 따라 특정 지점에 배치된 색상으로 정의된 그레이디언트에 다시 매핑합니다.

이 효과는 텍스처 레이어나 마스크 내부(흑백 출력)에서 다른 이미지에서 샘플링한 그레이디언트로 회색 음영 값을 다시 매핑하는 데 사용됩니다.

</td>
</tr>
</table>

## 입력

| 입력 이름 | 설명 |
| --- | --- |
| <b>그레이디언트 소스:</b> 색상 | 사용자 정의 색상 맵 또는 고정점을 사용합니다. |

<a name="parameters"></a>

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| <b>그레이디언트 방향:</b> | 그레이디언트 소스를 가로로 샘플링할지 세로로 샘플링할지 선택합니다. |
| <b>그라디언트 입력 위치:</b> | 그레이디언트 입력에서 샘플링된 위치를 조정합니다. |
