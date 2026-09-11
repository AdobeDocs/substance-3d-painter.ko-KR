---
title: Shrinkwrap 부풀리기
description: Substance 3D Painter의 Inflate Shrinkwrap 생성기를 사용하는 방법에 대해 알아봅니다.
source-git-commit: b7770a9497f0db047433aec32c31b57f8dc13ae7
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 3%

---


# Shrinkwrap 부풀리기

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_inflate_shrinkwrap.webp" alt=""/><br><strong>내부:</strong> 축소, 부풀리기, 생성기, 임의화</td>
    <td style="border: 0;" valign="top"><strong>설명</strong><br>Inflate Shrinkwrap은 얇은 재질의 생성기가 메쉬 표면에 나타나는 것과 비슷한 주름을 추가합니다.<br><br>Inflate Shrinkwrap 생성기는 단색(흑백) 텍스처를 출력합니다. 따라서 수축 효과를 만드는 마스크를 생성하는 데 유용합니다. 하지만 채우기 레이어에 직접 배치하여 Height과 일반 채널에 주름을 추가할 수도 있습니다.<br><br>이미지 입력에는 구워진 곡률 맵이 필요합니다. <a href="../../../baking/baking.md">여기서 굽는 방법에 대해 자세히 알아보세요</a>.</td>
  </tr>
</table>

## 입력

| 입력 이름 | 설명 |
| --- | --- |
| **곡률** 회색 음영 | 구워진 곡률 맵을 사용합니다. |

## 매개변수

<table>
  <tr>
    <th>매개 변수 이름</th>
    <th>설명</th>
  </tr>
  <tr>
    <td><strong>사전 설정</strong></td>
    <td>팽창된 사전 설정, 진공 당기기 사전 설정 및 타이트 사전 설정 간에 전환합니다.</td>
  </tr>
  <tr>
    <td><strong>시드</strong></td>
    <td>Dirt 텍스처 생성에 사용되는 시드 값을 설정합니다. <br><ul><li>[임의]를 클릭하여 다른 임의 시드로 전환합니다.</li><li>연필을 클릭하여 현재 시드 값을 보고 원하는 경우 특정 값을 입력합니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>부풀리기 또는 가는 줄 바꿈</strong></td>
    <td>[부풀리기] 모드와 [화면 감싸기] 모드 사이를 전환합니다.</td>
  </tr>
  <tr>
    <td><strong>이음새 강도</strong></td>
    <td>가장자리가 얼마나 두드러지는지 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>가장자리 상승 폭</strong></td>
    <td>부풀린 가장자리가 얼마나 부풀었는지 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>가장자리 상승 강도</strong></td>
    <td>융기된 가장자리 효과의 강도를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>주름 밀도</strong></td>
    <td>주름 수를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>주름 긴장</strong></td>
    <td>UV 테두리에서 주름이 서로 얼마나 조밀하게 당겨지는지 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>주름 범위</strong></td>
    <td>주름과 UV 테두리의 거리를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>주름 비율</strong></td>
    <td>주름의 크기를 조정합니다.</td>
  </tr>
</table>

### 기술 매개 변수

| 매개 변수 이름 | 설명 |
| --- | --- |
| **Height 범위** | Height 범위를 설정합니다. |
| **Height 위치** | Height을 검정(0) 또는 흰색(1) 방향으로 조정합니다. |
| **표면 크기(cm)** | 서피스의 물리적 크기를 설정합니다. |
| **표면 깊이(cm)** | 서피스의 물리적 깊이를 설정합니다. |
