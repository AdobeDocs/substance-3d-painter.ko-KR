---
title: UV 테두리 거리
description: Substance 3D Painter의 UV 테두리 거리 생성기를 사용하는 방법에 대해 알아봅니다.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 1%

---


# UV 테두리 거리

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_uv_border_distance.png" alt=""/><br><strong>내부:</strong> 메시, uv, 거리</td>
    <td style="border: 0;" valign="top"><strong>설명</strong><br>UV 테두리 거리 생성기는 UV 섬 테두리에 회색 음영 마스크를 만들어 UV의 테두리를 따라 다양한 효과를 쉽게 추가할 수 있도록 합니다.<br><br>UV 테두리 거리 생성기는 단색(흑백) 텍스처를 출력합니다. 따라서 UV 테두리 근처 영역을 강조하는 마스크를 생성하는 데 유용합니다.</td>
  </tr>
</table>

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| **반전** | 생성기 출력을 반전시킵니다. |
| **균형** | 명도 컨트롤처럼 중간점을 검정 또는 흰색으로 이동하여 효과의 균형을 조정합니다. |
| **대비** | 효과의 대비/감소를 조정합니다. |
| **Smoothness** | 효과의 원형률을 조정합니다. 낮은 **Smoothness** 값을 사용하는 경우 가장 많이 표시됩니다. |
| **거리** | 효과가 UV 테두리에서 얼마나 멀리 확장되는지 조정합니다. |
