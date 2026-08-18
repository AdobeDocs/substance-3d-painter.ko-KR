---
title: 회색 음영 전환
description: Substance 3D Painter의 회색 음영 변환 생성기를 사용하는 방법에 대해 알아봅니다.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 5%

---


# 회색 음영 전환

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_grayscale_conversion.png" alt=""/><br><strong>인:</strong> 생성기, 회색 음영, 색상</td>
    <td style="border: 0;" valign="top"><strong>설명</strong><br>회색 음영 변환 생성기는 텍스처나 맵을 회색 음영 값으로 변환합니다.<br><br>회색 음영 변환 생성기는 단색(흑백) 텍스처를 출력합니다. 따라서 전체 색상 입력 맵에서 마스크를 생성하는 데 유용합니다.</td>
  </tr>
</table>

## 입력

| 입력 이름 | 설명 |
| --- | --- |
| **소스** 색상 | 사용자 정의 색상 텍스처 또는 고정점을 사용합니다. |

## 매개변수

<table>
  <tr>
    <th>매개 변수 이름</th>
    <th>설명</th>
  </tr>
  <tr>
    <td><strong>회색 음영 유형</strong></td>
    <td>회색 음영 변환 방법을 설정합니다. <br><ul><li><strong>채도 감소</strong>: RGB 채널의 가장 강한 것과 가장 약한 것 사이의 절반 값을 사용합니다.</li><li><strong>루마</strong>: 사람의 눈으로 인지된 밝기(녹색을 선호함)와 일치하는 가중 RGB 계수를 사용합니다.</li><li><strong>평균</strong>: 빨강, 녹색 및 파랑 채널을 같은 양으로 혼합합니다.</li><li><strong>최대</strong>: RGB 채널에서 가장 높은 값을 사용합니다.</li><li><strong>분</strong>: RGB 채널의 가장 낮은 값을 사용합니다.<ul><li>빨강 채널: 빨강 채널만 사용합니다.</li><li>녹색 채널: 녹색 채널만 사용합니다.</li><li>파란색 채널: 파란색 채널만 사용합니다.</li></ul></li></ul></td>
  </tr>
  <tr>
    <td><strong>반전</strong></td>
    <td>마스크를 반전합니다.</td>
  </tr>
  <tr>
    <td><strong>균형</strong></td>
    <td>명도 컨트롤처럼 중간점을 검정 또는 흰색으로 이동하며 변환된 소스 이미지의 균형을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>대비</strong></td>
    <td>변환된 소스 이미지의 대비/밝기 감소를 정의합니다.</td>
  </tr>
  <tr>
    <td><strong>타일</strong></td>
    <td>변환된 소스 이미지의 타일링을 설정합니다.</td>
  </tr>
  <tr>
    <td><strong>회전</strong></td>
    <td>변환된 소스 이미지의 각도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>안전한 회전</strong></td>
    <td>안전 회전 모드를 켜거나 끕니다. true이면 [안전 회전]은 회전을 45도 각도로 잠급니다.</td>
  </tr>
</table>
