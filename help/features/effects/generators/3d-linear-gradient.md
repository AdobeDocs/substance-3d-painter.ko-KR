---
title: 3D Linear gradient
description: Substance 3D Painter의 3D Linear gradient 생성기 사용 방법을 알아봅니다.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---


# 3D Linear gradient

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_3d_linear_gradient.webp" alt=""/><br><strong>인:</strong> 그레이디언트, 회색 음영</td>
    <td style="border: 0;" valign="top"><strong>설명</strong><br>3D Linear gradient 생성기는 위치 맵을 사용하여 메시의 두 점 사이에 그레이디언트를 만듭니다. <br><br>3D Linear gradient은 단색(흑백) 텍스처를 출력합니다. 따라서 특정 영역에 선형 그레이디언트를 배치하기 위한 마스크를 생성하는 데 유용합니다.<br><br>이미지 입력에는 구워진 위치 맵이 필요합니다. <a href="../../../baking/baking.md">여기서 굽는 방법에 대해 자세히 알아보세요</a>.<br><br>위치 맵은 X, Y 및 Z축을 따라 0과 1 사이의 위치에 해당하는 메쉬의 각 점에 색상을 할당합니다. 이는 메시의 각 점이 고유한 색상을 가진다는 것을 의미합니다. 시작 및 종료 위치의 위치 맵 색상을 선택하여 선형 그레이디언트의 시작점 및 끝점을 설정할 수 있습니다.</td>
  </tr>
</table>

## 입력

| 입력 이름 | 설명 |
| --- | --- |
| **위치** | 구워진 위치 맵을 사용합니다. |

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| **반전** | 선형 그레이디언트를 반전합니다. |
| **균형** | 선형 그레이디언트 중간점 위치를 이동합니다. |
| **대비** | 선형 그레이디언트의 대비를 조정합니다. |
| **3D 위치 시작** | 위치 맵의 색상을 기반으로 그레이디언트의 시작점을 설정합니다. 시작점을 쉽게 정의하려면 뷰포트에서 화면에 위치 맵을 표시하고 색상 피커를 사용하여 시작점을 선택합니다. |
| **3D 위치 끝** | 위치 맵의 색상을 기반으로 그레이디언트의 끝점을 설정합니다. 끝점을 쉽게 정의하려면 뷰포트에서 화면에 위치 맵을 표시하고 색상 피커를 사용하여 끝점을 선택합니다. |
