---
title: 임계값
description: Substance 3D Painter의 임계값 필터 사용 방법을 알아봅니다.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 3%
---

# 임계값

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![임계값 아이콘](./Resources/icon_threshold.png "임계값")

<b>인:</b> 효과/조정

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 설명

[한계값] 필터는 [한계값]을 기준으로 입력 픽셀 값에 대해 [모드] 매개 변수에 설정된 비교 기준이 충족되면 흰색을 반환합니다. [히스토그램 스캔]과 유사하지만, 대비가 항상 최대 수준인 경우 유사한 결과를 얻을 수 있는 더 빠르고 정확한 방법을 제공합니다.

이 효과는 칠 레이어나 마스크(흑백 출력)에서 직접 사용하여 특정 채널에서 고대비 마스크를 빠르게 만듭니다.

</td>
</tr>
</table>

<a name="parameters"></a>

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| <b>임계값:</b> | 입력 픽셀 값과 비교할 광도 값을 조정합니다. |
| <b>모드:</b> | 임계값에 대해 사용되는 비교 기준(보다 큼, 보다 큼 또는 같음, 보다 작음 또는 보다 낮음 또는 같음)을 선택합니다. |
| <b>_모드:</b> | 내부 모드 값을 선택합니다. |
| <b>_threshold:</b> | 내부 임계값을 조정합니다. |
| <b>_threshold_min:</b> | 내부 최소 임계값을 조정합니다. |
| <b>_threshold_max:</b> | 내부 최대 임계값을 조정합니다. |
