---
title: 밝게
description: Substance 3D Painter의 빛 생성기를 사용하는 방법을 알아봅니다.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 3%

---


# 밝게

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_light.webp" alt=""/><br><strong>인:</strong> 마스크, 생성기</td>
    <td style="border: 0;" valign="top"><strong>설명</strong><br>조명 생성기는 월드 스페이스 표준 및 위치 맵을 기반으로 메쉬에 비추는 직접 조명을 만듭니다.<br><br>광발생기는 채우기 레이어에서 사용하거나 마스크를 만드는 데 사용할 수 있습니다. 칠 레이어에서 사용할 경우 생성기는 색상, 금속도, Specular 거칠기, 일반 및 Height 채널을 출력하며 다양한 조합으로 사용하여 다양한 효과를 만들 수 있습니다. 각 채널이 빛 생성기의 영향을 받는 방식을 이해하려면 뷰포트의 채널 보기를 순환하는 것이 좋습니다.<br><br>구겨진 위치 및 월드 공간 표준 맵이 이미지 입력으로 필요합니다. <a href="../../../baking/baking.md">여기서 굽는 방법에 대해 자세히 알아보세요</a>.</td>
  </tr>
</table>

## 입력

| 입력 이름 | 설명 |
| --- | --- |
| **월드 스페이스 표준** 색상 | 구워진 World Space Normals 지도를 사용합니다. |
| **위치** 색상 | 구워진 위치 맵을 사용합니다. |

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| **반전** | 출력 색상 맵을 반전합니다. |
| **수평 각도** | 페이크 라이트의 수평 각도를 설정합니다. |
| **수직 각도** | 페이크 라이트의 수직 각도를 설정합니다. |
| **강조 표시 광택도** | 강조 표시된 영역의 밝기 감소 스프레드를 조정합니다. |
| **밝은 영역 수준** | 밝은 영역의 대비를 조정합니다. |
| **빛 감쇠** | 빛의 감소를 조정합니다. |
