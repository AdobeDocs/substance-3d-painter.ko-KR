---
title: UV 체커
description: Substance 3D Painter의 UV 검사기 생성기를 사용하는 방법에 대해 알아봅니다.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 3%

---


# UV 체커

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_uv_checker.png" alt=""/><br><strong>내부:</strong> uv, 테두리, 무작위</td>
    <td style="border: 0;" valign="top"><strong>UV 검사기 생성기는 모형에 격자와 같은 검사기 패턴을 적용하므로 UV 문제(예: 늘리다, 고르지 않은 비율, 왜곡)를 쉽게 발견할 수 있습니다. </strong><br><br><br>UV 검사기 생성기는 일반적으로 UV 왜곡을 보기 위해 채우기 레이어에서 직접 사용됩니다.</td>
  </tr>
</table>

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
    <td><strong>검사기 색상 모드</strong></td>
    <td>색상 할당 방법 선택:<br><ul><li><strong>균일</strong>: 텍스처 집합에서 동일한 색상을 적용합니다.</li><li><strong>무작위</strong>: 각 UV 섬에 무작위 색상을 적용합니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>검사기 색상</strong></td>
    <td>체커 패턴의 색상을 설정합니다.</td>
  </tr>
  <tr>
    <td><strong>체크무늬 격자 타일</strong></td>
    <td>체커 패턴의 크기를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>체크무늬 격자 불투명도</strong></td>
    <td>격자의 불투명도를 조정합니다. 불투명도가 0이면 격자 없이 체커 텍스처만 표시됩니다.</td>
  </tr>
  <tr>
    <td><strong>UV 테두리 색상</strong></td>
    <td>UV 테두리 색상을 설정합니다.</td>
  </tr>
  <tr>
    <td><strong>UV 테두리 너비</strong></td>
    <td>UV 테두리의 폭을 조정합니다.</td>
  </tr>
</table>
