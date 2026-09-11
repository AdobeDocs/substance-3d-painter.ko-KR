---
title: 3D 거리
description: Substance 3D Painter의 3D Distance Generator 사용 방법을 알아봅니다.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 1%

---


# 3D 거리

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_3d_distance.webp" alt=""/><br><strong>인:</strong> 마스크, 생성기</td>
    <td style="border: 0;" valign="top"><strong>설명</strong><br>3D 거리 생성기는 3D 공간에서 점(소스 점)을 정의하고 해당 점으로부터의 거리를 단색 그레이디언트로 표시합니다. 메시 표면에서 해당 점과 더 가까운 영역은 더 어둡고 더 멀리 있는 영역은 더 밝습니다(기본적으로).<br><br>이미지 입력에는 구워진 위치 맵이 필요합니다. <a href="../../../baking/baking.md">여기서 굽는 방법에 대해 자세히 알아보세요</a>.<br><br>3D 거리는 흑백 텍스처를 출력합니다. 따라서 지정된 위치에서 멀리 떨어진 그레이디언트를 만드는 마스크를 생성하는 데 유용합니다.<br><br></td>
  </tr>
</table>

## 입력

| 입력 이름 | 설명 |
| --- | --- |
| **위치** | 구워진 위치 맵을 사용하여 거리를 계산합니다. |

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| **반전** | 그레이디언트를 반전시킵니다. |
| **위치 X** | x축 |
| **위치 Y** | y축 |
| **위치 Z** | z축 |
| **반경** | 거리 감소의 크기를 조정합니다. |
| **오프셋** | 그레이디언트의 시작 및 끝 위치를 소스 포인트 앞이나 뒤로 이동합니다. 소스 포인트 반대 방향으로 이동(오프셋 증가)하면 소스 포인트 근처의 어두운 영역이 더 커집니다. 소스 포인트에 가깝게 이동하면 그레이디언트가 밝아져 **오프셋**&#x200B;이 0으로 설정된 경우 그레이디언트가 모두 제거될 수 있습니다. |
| **대비** | 구형 그레이디언트의 대비를 조정합니다. |
