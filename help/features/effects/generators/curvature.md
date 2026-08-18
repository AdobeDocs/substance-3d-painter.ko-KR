---
title: 곡선
description: Substance 3D Painter 곡률 제너레이터를 사용하는 방법에 대해 알아봅니다.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 4%

---


# 곡선

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_curvature.webp" alt=""/><br><strong>인:</strong> 마스크, 생성기, 회색 음영, 혼합</td>
    <td style="border: 0;" valign="top"><strong>설명</strong><br>곡률 생성기는 구워진 곡률 맵을 기반으로 마스크를 만듭니다. 텍스처 또는 미세한 세부 사항을 마스크에 혼합하는 옵션도 있습니다.<br><br>곡률 생성기는 단색(흑백) 텍스처를 출력합니다. 결과적으로 레이어에 직접 적용하지 않고 마스크를 생성하는 데 유용합니다.<br><br>구워진 위치 맵은 입력으로 필요합니다. <a href="../../../baking/baking.md">여기서 굽는 방법에 대해 자세히 알아보세요</a>.</td>
  </tr>
</table>

## 입력

| 입력 이름 | 설명 |
| --- | --- |
| **텍스처** 색상 | 사용자 정의 텍스처 또는 고정점을 사용합니다. |
| **마이크로 표준** 색상 | 사용자 정의 표준 텍스처 또는 고정점을 사용합니다. |
| **마이크로 Height** 색상 | 사용자 정의 텍스처 또는 고정점을 사용합니다. |
| **곡률** 회색 음영 | 구워진 곡률 맵을 사용합니다. |
| **월드 스페이스 표준** 색상 | 구워진 World Space Normals 지도를 사용합니다. |
| **위치 그라디언트** 색상 | 구워진 위치 맵을 사용합니다. |

## 매개변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| **전역 반전** | 모든 효과가 결합된 후 최종 결과를 반전합니다. |
| **전역 흐림 효과** | 모든 효과가 결합된 후 최종 마스크를 균일하게 부드럽게 합니다. |
| **전역 균형** | 명도 조정처럼 모든 효과를 검정 또는 흰색 사이에서 결합한 후 최종 마스크의 균형을 이동합니다. |
| **전역 대비** | 모든 효과가 결합된 후 최종 마스크의 대비를 조정합니다. |
| **텍스처 사용** | 사용자 정의 텍스처 맵 사용을 설정하거나 해제합니다. |
| **마이크로 세부 사항 사용** | 사용자 정의 마이크로 세부 사항 맵 사용을 켜거나 끕니다. |

### 곡선

<table>
  <tr>
    <th>매개 변수 이름</th>
    <th>설명</th>
  </tr>
  <tr>
    <td><strong>반전</strong></td>
    <td>생성된 곡률 맵을 반전합니다.</td>
  </tr>
  <tr>
    <td><strong>모드</strong></td>
    <td>곡률 모드를 설정합니다. <br><ul><li><strong>가장자리</strong>: 가장자리(볼록 영역)를 마스크합니다.</li><li><strong>공동</strong>: 공동(오목 영역)을 마스킹합니다.</li><li><strong>이중</strong>: 오목 및 볼록 영역을 마스크합니다.</li><li><strong>처리되지 않음</strong>: 표준 곡률 마스크입니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>선명함</strong></td>
    <td>선명한 곡률 세부 사항의 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>벌금</strong></td>
    <td>미세 곡률 세부 사항의 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>부드럽게</strong></td>
    <td>부드러운 곡률 세부 사항의 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>중간</strong></td>
    <td>중간 곡률 세부 사항의 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>크게</strong></td>
    <td>큰 곡률 세부 사항의 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>큼</strong></td>
    <td>큰 곡률 세부 사항의 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>거대하</strong></td>
    <td>큰 곡률 세부 사항의 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>대비</strong></td>
    <td>곡률의 대비/감소를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>밝기</strong></td>
    <td>곡률의 광도를 조정합니다.</td>
  </tr>
</table>

### 텍스처

<table>
  <tr>
    <th>매개 변수 이름</th>
    <th>설명</th>
  </tr>
  <tr>
    <td><strong>텍스처 불투명도</strong></td>
    <td>사용자 정의 텍스처의 가시성을 제어합니다.</td>
  </tr>
  <tr>
    <td><strong>반전</strong></td>
    <td>사용자 정의 텍스처만 반전합니다.</td>
  </tr>
  <tr>
    <td><strong>회색 음영 전환</strong></td>
    <td>색상 입력을 흑백으로 변환하는 데 사용할 방법을 선택합니다. </td>
  </tr>
  <tr>
    <td><strong>혼합 모드</strong></td>
    <td>사용자 정의 텍스처의 혼합 모드를 설정합니다.</td>
  </tr>
  <tr>
    <td><strong>비율</strong></td>
    <td>사용자 정의 텍스처의 크기를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>대비</strong></td>
    <td>사용자 정의 텍스처의 대비/감소를 설정합니다.</td>
  </tr>
  <tr>
    <td><strong>밝기</strong></td>
    <td>사용자 정의 텍스처의 광도를 설정합니다.</td>
  </tr>
  <tr>
    <td><strong>삼평면</strong></td>
    <td>삼각 평면(Triplanar)을 사용하면 텍스처가 UV에만 의존하지 않고 세 방향(X, Y, Z 축)에서 투영됩니다. <br><ul><li>삼각형을 사용하지 않으면 텍스처가 UV 레이아웃을 따릅니다.</li><li>삼면체를 사용하면 텍스처가 여러 각도에서 투영되어 혼합됩니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>삼평면 대비</strong></td>
    <td>트리평면 매핑을 사용하여 텍스처를 투영할 때 얼마나 부드럽게 혼합할지 조정합니다. 각 방향의 투영 간 혼합의 부드러움을 조정합니다.</td>
  </tr>
</table>

### 마이크로 세부 사항

<table>
  <tr>
    <th>매개 변수 이름</th>
    <th>설명</th>
  </tr>
  <tr>
    <td><strong>마이크로 Height</strong></td>
    <td>사용자 정의 Micro Height 맵 사용을 켜거나 끕니다.</td>
  </tr>
  <tr>
    <td><strong>미량 정상</strong></td>
    <td>사용자 정의 Micro Normal 맵 사용을 켜거나 끕니다.</td>
  </tr>
  <tr>
    <td><strong>곡률 유형</strong></td>
    <td>곡률 유형을 설정합니다. <br><ul><li><strong>표준</strong>: 일반적으로 매우 선명한 결과를 만들지만 더 넓은 세부 사항은 부족할 수 있습니다.</li><li><strong>Sobel</strong>: Sobel 필터를 사용하여 표준 맵을 평가하기 때문에 표준과 유사한 결과를 얻지만 약간 더 흐립니다.</li><li><strong>매끄럽게</strong>: 정보를 누적하기 위해 다양한 수준의 흐림 효과(예: 밉맵)를 생성합니다. 이 옵션을 선택하면 일반적으로 곡선이 더 매끄러워지지만 세부 묘사가 손실될 수 있습니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>곡률 강도</strong></td>
    <td><strong>표준 </strong> 및 <strong>소벨 </strong>곡률 모드에서 곡률 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>Height 세부 정보 강도</strong></td>
    <td>마이크로 Height 세부 사항의 강도를 조정합니다.</td>
  </tr>
</table>
