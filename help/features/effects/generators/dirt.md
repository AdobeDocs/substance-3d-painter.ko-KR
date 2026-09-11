---
title: 흙
description: Substance 3D Painter의 Dirt 생성기 사용 방법을 알아봅니다.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 1%

---


# 흙

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_dirt.webp" alt=""/><br><strong>인:</strong> 마스크, 생성기</td>
    <td style="border: 0;" valign="top"><strong>설명</strong><br>Dirt 생성기는 곡률, 앰비언트 오클루전을 기반으로 틈새, 가장자리 및 평평한 표면에 Dirt 및 그런지의 사실적인 축적을 추가합니다. 또한 필요에 따라 [마이크로 Height] 및 [마이크로 노멀 맵]을 사용하여 더 많은 세부 사항을 추가할 수 있습니다.<br><br>Dirt 생성기는 흑백 텍스처를 출력합니다. 따라서 마스크를 생성하여 Dirt 또는 그런지 세부 정보를 모델에 추가하는 데 유용합니다.<br><br>구겨진 위치, 곡률, 앰비언트 오클루전 및 세계 공간 표준 맵이 이미지 입력으로 필요합니다. <a href="../../../baking/baking.md">여기서 굽는 방법에 대해 자세히 알아보세요</a>.</td>
  </tr>
</table>

>[!NOTE]
>
> Dirt 생성기는 메시에 Dirt을 빠르게 추가할 수 있는 강력한 도구입니다. 최상의 결과를 얻으려면 환경 및 에셋 내역을 항상 고려하여 Dirt 적용 방식을 제어할 수 있도록 추가 마스크를 사용하는 것이 좋습니다.

## 입력

| 입력 이름 | 설명 |
| --- | --- |
| **곡률** 회색 음영 | 구워진 곡률 맵을 사용합니다. |
| **앰비언트 오클루전** 회색 음영 | 구운 앰비언트 오클루전 맵을 사용합니다. |
| **월드 스페이스 표준** 색상 | 구워진 World Space Normals 지도를 사용합니다. |
| **위치** 색상 | 구워진 위치 맵을 사용합니다. |
| **사용자 지정 그런지** 회색 음영 | 사용자 정의 텍스처 또는 고정점을 사용합니다. |
| **마이크로 표준** 색상 | 사용자 정의 표준 텍스처 또는 고정점을 사용합니다. |
| **마이크로 Height** 색상 | 사용자 정의 텍스처 또는 고정점을 사용합니다. |

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
    <td><strong>반전</strong></td>
    <td>Dirt 마스크를 반전합니다.</td>
  </tr>
  <tr>
    <td><strong>Dirt 수준</strong></td>
    <td>Dirt 효과의 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>Dirt 대비</strong></td>
    <td>Dirt 효과의 대비를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>삼각 평면 사용</strong></td>
    <td>삼각 평면(Triplanar)을 활성화하면 UV에만 의존하지 않고 세 방향(X, Y, Z 축)에서 텍스처가 투영됩니다. <br><ul><li>트리평면이 활성화되지 않은 경우 텍스처는 UV 레이아웃을 따릅니다.</li><li>삼각 평면을 활성화하면 텍스처가 여러 각도에서 투영되고 혼합됩니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>삼평면 혼합 대비</strong></td>
    <td>삼면형 매핑을 사용하여 텍스처를 투영할 때 혼합하는 매끄러운 정도를 조정합니다. 각 방향의 투영 간 혼합의 부드러움을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>그런지 양</strong></td>
    <td>그런지 세부 사항의 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>그런지 비율</strong></td>
    <td>그런지 세부 사항의 크기를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>사용자 정의 그런지 사용</strong></td>
    <td>사용자 정의 그런지 맵 사용을 켜거나 끕니다.</td>
  </tr>
  <tr>
    <td><strong>가장자리 마스크</strong></td>
    <td>곡률 맵을 기반으로 가장자리의 마스크를 조정합니다.</td>
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
    <td>사용자 정의 마이크로 높이 맵 사용을 켜거나 끕니다.</td>
  </tr>
  <tr>
    <td><strong>미량 정상</strong></td>
    <td>사용자 정의 Micro 노멀 맵 사용을 켜거나 끕니다.</td>
  </tr>
  <tr>
    <td><strong>곡률 유형</strong></td>
    <td>곡률 유형을 설정합니다. <br><ul><li><strong>표준</strong>: 일반적으로 매우 선명한 결과를 만들지만 더 넓은 세부 사항은 부족할 수 있습니다.</li><li><strong>Sobel</strong>: 표준과 비교했을 때 비슷한 결과를 만들지만 Sobel 필터를 사용하여 노멀 맵을 평가하기 때문에 약간 더 흐립니다.</li><li><strong>매끄럽게</strong>: 정보를 누적하기 위해 다양한 수준의 흐림 효과(예: 밉맵)를 생성합니다. 이 옵션을 선택하면 일반적으로 곡선이 더 매끄러워지지만 세부 묘사가 손실될 수 있습니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>곡률 강도</strong></td>
    <td>표준 및 소벨 곡률 모드에서 곡률 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>Height 세부 정보 강도</strong></td>
    <td>마이크로 Height 세부 사항의 양을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>AO 반경</strong></td>
    <td>미세한 세부 사항에서 앰비언트 오클루전의 반경(범위)을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>AO 깊이</strong></td>
    <td>미세한 세부 사항에서 앰비언트 오클루전의 깊이(강도)를 조정합니다.</td>
  </tr>
</table>
