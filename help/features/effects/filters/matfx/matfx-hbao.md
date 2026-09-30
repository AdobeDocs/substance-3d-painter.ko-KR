---
title: MatFX HBAO
description: Substance 3D Painter의 MatFX HBAO 필터 사용 방법을 알아보십시오.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%
---

# MatFX HBAO

<table>
<tr style="border: 0;">
<td width="33.33%" style="border: 0;" valign="top">

![MatFX HBAO 아이콘](./Resources/icon_matfx_hbao.png "MatFX HBAO")

<b>내부:</b> 효과/앰비언트 오클루전, Height, 음영

</td>
<td width="100.00%" style="border: 0;" valign="top">

## 설명

MatFX HBAO 필터는 Height 정보로부터 수평선 기반 앰비언트 오클루전을 생성합니다.

소스 채널이나 텍스처 정보를 기반으로 깊이 및 연락처 그림자를 추가하는 데 Height 레이어나 마스크에 사용됩니다.

</td>
</tr>
</table>

<a name="parameters"></a>

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| <b>흐림 강도:</b> | 결과의 흐림 효과 강도를 조정합니다. |
| <b>흐림 효과 줄 바꿈:</b> | 흐림 효과 감싸기를 전환합니다. 이 효과를 활성화하면 텍스처 반대쪽의 픽셀이 샘플링됩니다. |
| <b>채널 원본:</b> | 채널 생성에 사용할 오클루전 소스를 선택합니다. |
| <b>세계 단위 사용:</b> | 월드 공간 단위 사용을 전환합니다. |
| <b>Height 깊이:</b> | Height 입력의 인식된 깊이를 조정합니다. |
| <b>반경:</b> | 오클루전 효과의 샘플링 반경을 조정합니다. |
| <b>강도:</b> | 오클루전 강도를 조정합니다. |
| <b>부조 균형:</b> | 부조 기여도의 균형을 조정합니다. |
