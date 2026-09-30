---
title: 색상 일치
description: Substance 3D Painter에서 색상 일치 필터를 사용하는 방법을 알아봅니다.
source-git-commit: 644a36a1dde953c1d793821e104049ebb6ec3c19
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%
---

# 색상 일치

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="./Resources/icon_color_match.png" alt="색상 일치 아이콘" title="색상 일치"/><br><strong>인:</strong> 효과/조정</td>
    <td style="border: 0;" valign="top">설명<br>색상 일치 필터는 정의된 소스 색상 범위를 대상 색상 범위와 일치시키고 소스 값과 대상 값을 모두 정의하는 입력 슬롯을 지원합니다. 색상 일치를 사용하면 색조, 크로마, 루마가 처리되는 방식을 제어하여 표면의 색상을 변경하는 동안 세부 사항을 유지할 수 있습니다.<br>색상 일치로 칠 레이어 조정,</td>
  </tr>
</table>

## 입력

| 입력 이름 | 설명 |
| --- | --- |
| **소스 색상:** | 소스 색상에 대한 입력 슬롯입니다. 사용자 정의 색상 맵 또는 고정점을 사용합니다. |
| **대상 색:** | 대상 색상에 대한 입력 슬롯입니다. 사용자 정의 색상 맵 또는 고정점을 사용합니다. |

## 매개변수

<table>
  <tr>
    <th>매개 변수 이름</th>
    <th>설명</th>
  </tr>
  <tr>
    <td><strong>소스 색상 모드:</strong></td>
    <td>소스 색상의 소스를 선택합니다.<br><ul><li><strong>평균</strong>: 기존 재질 색상을 소스 색상으로 사용합니다. 레이어 혼합 모드를 <strong>패스스루</strong>(으)로 설정해야 합니다.</li><li><strong>매개 변수</strong>: 매개 변수를 사용하여 원본 색을 설정합니다.</li><li><strong>입력</strong>: 이미지 입력으로 소스 색상을 설정합니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>소스 색상:</strong></td>
    <td><strong>소스 색상 모드</strong>가 <strong>매개 변수</strong>(으)로 설정된 경우 소스 색상을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>대상 색상 모드:</strong></td>
    <td>대상 색상의 소스를 선택합니다.<br><ul><li><strong>매개 변수</strong>: 매개 변수를 사용하여 대상 색을 설정합니다.</li><li><strong>입력</strong>: 이미지 입력으로 대상 색상을 설정합니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>대상 색상:</strong></td>
    <td><strong>대상 색상 모드</strong>가 <strong>매개 변수</strong>(으)로 설정된 경우 대상 색상을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>사용자 정의 색상 변형:</strong></td>
    <td>사용자 정의 색조, 크로마, 루마 변형 컨트롤을 토글합니다.</td>
  </tr>
  <tr>
    <td><strong>색조:</strong></td>
    <td>결과에 적용된 색조 변형을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>크로마:</strong></td>
    <td>결과에 적용된 크로마 변형을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>루마:</strong></td>
    <td>결과에 적용되는 루마 변화를 조정합니다.</td>
  </tr>
</table>