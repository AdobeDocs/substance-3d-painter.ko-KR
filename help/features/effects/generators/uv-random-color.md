---
title: UV 무작위 색상
description: Substance 3D Painter의 UV Random Color Generator 사용 방법을 알아보십시오.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 2%

---


# UV 무작위 색상

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_uv_random_color.png" alt=""/><br><strong>인:</strong> 유틸리티, 마스크</td>
    <td style="border: 0;" valign="top"><strong>설명</strong><br>UV 무작위 색상 생성기는 각 UV 섬에 고유한 단색을 할당합니다. 이는 복잡한 메쉬를 포함하는 진단 도구로 유용합니다.<br><br>UV 임의 색상은 마스크(흑백 출력)를 만들거나 UV 섬을 기반으로 메쉬에 색상 변화를 적용하기 위한 채우기 레이어로 직접 사용할 수 있습니다. 예를 들어 나무 바닥의 각 판자를 임의로 지정할 수 있습니다.</td>
  </tr>
</table>

## 입력

| 입력 이름 | 설명 |
| --- | --- |
| **사용자 지정 그레이디언트** | 그레이디언트 맵을 사용하여 색상 범위를 정의합니다. |

## 매개변수

<table>
  <tr>
    <th>매개 변수 이름</th>
    <th>설명</th>
  </tr>
  <tr>
    <td><strong>시드</strong></td>
    <td>Dirt 텍스처 생성에 사용되는 시드 값을 설정합니다. <br><ul><li>[임의]를 클릭하여 다른 임의 시드로 전환합니다.</li><li>연필을 클릭하여 현재 시드 값을 보고 원하는 경우 특정 값을 입력합니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>색상 소스 모드</strong></td>
    <td>사용된 색상 소스 모드를 결정합니다. <br><ul><li><strong>무작위</strong>: 무작위 모드에서 색상은 임의로 정의되고 할당됩니다.</li><li><strong>사용자 지정 그레이디언트</strong>: 사용자 지정 그레이디언트 모드에서 색상을 선택할 수 있는 사용자 지정 그레이디언트 맵을 추가하는 추가 입력이 있습니다.</li></ul></td>
  </tr>
</table>
