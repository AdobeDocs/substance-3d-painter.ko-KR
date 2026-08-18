---
title: 자동 스티처
description: Substance 3D Painter의 Auto Stitcher 제네레이터 사용 방법을 알아봅니다.
source-git-commit: b095b9b437f75bbb3a3b85ee84a6850026c3bf98
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 1%

---


# 자동 스티처

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../../assets/generators/icon_auto_stitcher.png" alt=""/><br><strong>내부:</strong> 스티치, 스티치</td>
    <td style="border: 0;" valign="top"><strong>설명</strong><br>자동 스티처 생성기는 절차적으로 생성된 경로를 따라 스티칭 효과를 자동으로 생성합니다. 이러한 패스는 UV 이음새, 곡률 또는 사용자 정의 입력 맵을 기반으로 생성할 수 있습니다.<br><br>자동 스티처 생성기는 단색(흑백) 텍스처를 출력합니다. 따라서 마스크를 생성하여 스티칭 효과를 적용하는 데 유용합니다.<br><br>곡률 마스크 모드를 사용하려면 구겨진 곡률 맵이 필요합니다. <a href="../../../baking/baking.md">여기서 굽는 방법에 대해 자세히 알아보세요</a>.</td>
  </tr>
</table>

## 입력

<table>
  <tr>
    <th>입력 이름</th>
    <th>설명</th>
  </tr>
  <tr>
    <td><strong>곡률</strong> 회색 음영</td>
    <td>스티칭 경로를 생성하는 방법을 선택합니다.<br><ul><li><strong>UV 마스크</strong>는 UV 솔기를 따라 패스를 생성합니다.</li><li><strong>곡률 </strong>은(는) 선명한 가장자리 근처에 패스를 생성합니다.</li><li><strong>사용자 지정 입력</strong>을 사용하면 맵을 사용하여 경로를 생성할 위치를 제어할 수 있습니다.<br><strong>사용자 지정 입력</strong>을 사용하면 고대비 영역에서 패스가 생성됩니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>사용자 지정 입력</strong> 회색 음영</td>
    <td>사용자 정의 텍스처 또는 고정점을 사용합니다.</td>
  </tr>
</table>

## 매개변수

<table>
  <tr>
    <th>매개 변수 이름</th>
    <th>설명</th>
  </tr>
  <tr>
    <td><strong>마스크 모드</strong></td>
    <td>마스크 모드를 선택합니다.<br><ul><li>UV 마스크: UV 섬을 기반으로 마스크합니다.</li><li>곡률: 곡률 맵을 기반으로 마스크를 만듭니다.</li><li>사용자 정의 입력: 사용자 정의 입력 텍스처를 기반으로 마스크를 만듭니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>패스 Smoothness</strong></td>
    <td>스티치가 적용된 패스를 부드럽게 합니다.</td>
  </tr>
  <tr>
    <td><strong>패스 위치</strong></td>
    <td>패스 위치를 오프셋합니다.</td>
  </tr>
  <tr>
    <td><strong>스티치 크기</strong></td>
    <td>스티치의 비율을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>스티치 폭</strong></td>
    <td>스티치의 폭을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>스티치 길이</strong></td>
    <td>스티치의 길이를 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>스티치 원형률</strong></td>
    <td>스티치의 원형률을 조정합니다.</td>
  </tr>
  <tr>
    <td><strong>지터</strong></td>
    <td>스티치 흐름 방향에서 지터를 조정합니다.</td>
  </tr>
</table>

## 예

<table>
  <tr>
    <td><img src="../../../assets/generators/examples/auto-stitcher/custom-input2.png" alt=""/></td>
    <td>이 예제에서는 사용자 정의 입력으로 스티칭 패스를 만드는 방법을 보여 줍니다. <br><ul><li>흑백 기본 색상은 자동 스티처 생성기에 대한 사용자 정의 입력으로 사용 중인 노이즈 텍스처를 표시합니다.</li><li>Autostitcher 생성기는 빨간색 레이어를 마스킹하고 빨간색 스티칭된 경로는 보이게 합니다.</li><li>빨간색 스티칭된 패스는 사용자 정의 입력 노이즈 텍스처의 충분히 큰 검은색 또는 흰색 영역에 맞습니다. 빨간색 스티칭은 흰색에서 검은색으로, 검은색에서 흰색으로 바뀌지 않습니다.</li></ul><br>아래 이미지는 이 예제를 만드는 데 사용된 간단한 레이어 설정을 보여줍니다.<br><br><img src="../../../assets/generators/examples/auto-stitcher/custom-input-layer-stack.png" alt=""/></td>
  </tr>
</table>
