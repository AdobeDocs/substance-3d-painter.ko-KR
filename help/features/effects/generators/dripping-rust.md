---
title: 드리핑 녹
description: Substance 3D Painter의 드리핑 녹 생성기를 사용하는 방법에 대해 알아봅니다.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 2%

---


# 드리핑 녹

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_dripping_rust.webp" alt=""/><br><strong>인:</strong> 생성기, 회색 음영, 색상</td>
    <td style="border: 0;" valign="top"><strong>설명</strong><br>드리핑 녹 생성기는 아래로 흐르는 녹 줄무늬를 만들어 중력과 물 유출로 인한 부식을 시뮬레이션합니다.<br><br>드리핑 녹 생성기는 흑백 텍스처를 출력합니다. 따라서 물방울 녹 효과를 만들기 위한 마스크를 생성하는 데 유용합니다.<br><br>구겨진 위치, 곡률 및 주변 오클루전이 이미지 입력으로 필요합니다. <a href="../../../baking/baking.md">여기서 굽는 방법에 대해 자세히 알아보세요</a>.</td>
  </tr>
</table>

## 입력

| 입력 이름 | 설명 |
| --- | --- |
| **곡률** 회색 음영 | 구워진 곡률 맵을 사용합니다. |
| **주변 오클루전** 회색 음영 | 구워진 Ambient 오클루전 맵을 사용합니다. |
| **위치** 색상 | 구워진 위치 맵을 사용합니다. |

## 매개변수

<table>
  <tr>
    <th>매개 변수 이름</th>
    <th>설명</th>
  </tr>
  <tr>
    <td><strong>시드</strong></td>
    <td>Dirt 텍스처를 생성하는 데 사용되는 시드 값을 설정합니다. <br><ul><li>[임의]를 클릭하여 다른 임의 시드로 전환합니다.</li><li>연필을 클릭하여 현재 시드 값을 보고 원하는 경우 특정 값을 입력합니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>반전</strong></td>
    <td>특정 내부 맵(예: 곡률, AO)을 최종 마스크로 결합하기 전에 반전합니다.</td>
  </tr>
  <tr>
    <td><strong>녹 확산</strong></td>
    <td>드리핑 녹 효과의 확장을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>녹 대비</strong></td>
    <td>드리핑 녹 효과의 대비를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>스프레딩 Smoothness</strong></td>
    <td>드리핑 녹 효과의 확대 부드러움을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>물방울 강도</strong></td>
    <td>드리핑 녹 효과의 길이를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>Smoothness 물방울</strong></td>
    <td>드리핑 녹 효과의 부드러움을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>샘플 양 드립</strong></td>
    <td>효과의 품질을 조정합니다(더 나은 품질을 위해 더 많은 샘플이 필요합니다).</td>
  </tr>
  <tr>
    <td><strong>위치 축</strong></td>
    <td>Y-녹색 채널, X-빨강 채널 및 B-파랑 채널 간을 전환하여 드리핑 녹 효과의 방향을 변경합니다.</td>
  </tr>
</table>
