---
helpx_url: 'https://helpx.adobe.com/substance-3d-painter/interface/project-configuration.html'
breadcrumb-title: ''
description: Substance 3D Painter에서 프로젝트 설정을 구성하여 텍스처 해상도, 채널 및 프로젝트 속성을 설정하는 방법을 알아봅니다.
helpx_creative_field: ''
helpx_description: Painter > Interface > Project configuration
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 프로젝트 구성
user-guide-description: ''
user-guide-title: ''
source-git-commit: 3e4ef9bd5897f042b01d6c0819ec06cc21ba208a
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 3%

---


# 프로젝트 구성

![](../assets/project-configuration-full.png)

프로젝트 구성 창에는 프로젝트 설정을 수정할 수 있는 컨트롤이 있습니다. 프로젝트 설정은 일반적으로 새 프로젝트를 만들 때 설정되지만, 프로젝트 후반부에서 이러한 설정을 변경해야 하는 경우도 있습니다.

## 3D 메시

3D 메시 또는 메시 파일이 변경된 경우 다른 프로젝트 데이터를 유지하면서 메시를 다시 가져올 수 있습니다. **메시 다시 가져오기**&#x200B;를 확인하고 올바른 파일을 가져오고 있는지 확인하십시오.

메쉬를 다시 가져오는 기능은 다음과 같은 경우에 유용합니다.

* 3D 모델 토폴로지 업데이트
* UV 업데이트
* [텍스처 집합](texture-set/texture-set.md) 추가 또는 제거

| **매개 변수** | **설명** |
| --- | --- |
| **3D 메시** | 3D 모델 파일의 경로를 나타냅니다. **선택 단추**&#x200B;를 사용하여 프로젝트의 원본 파일을 변경하십시오. |
| **메시 다시 가져오기** | 활성화되면 인터페이스 하단에 있는 확인(OK)을 클릭하면 메시 파일을 다시 가져옵니다. 선택(Select) 버튼을 사용하여 원본 메시 파일과 다른 메시 파일을 지정하면 이 매개변수가 자동으로 선택됩니다. |

>[!NOTE]
>
> 프로젝트 메시를 다시 가져올 때 질감 ID가 변경되거나 이름이 바뀐 경우 프로젝트의 이전 질감 세트를 비활성화하여 누락된 텍스처 모양이 될 수 있습니다. **텍스처 집합 목록**&#x200B;의 [재할당 창](texture-set/texture-set-reassignment.md)으로 이 문제를 해결할 수 있습니다.

## 프로젝트 설정

이 섹션에서는 프로젝트와 관련된 몇 가지 설정을 제어합니다.

<table>
  <tr>
    <th><em>설정</em></th>
    <th><em>설명</em></th>
  </tr>
  <tr>
    <td><strong>노멀 맵 포맷</strong></td>
    <td>뷰포트에서 메시에 사용할 노멀 맵 형식을 정의합니다. 이 매개 변수는 뷰포트의 <a href="shader-settings/shader-settings.md">음영</a>과 <a href="../baking/baking.md">베이커</a>의 메시 맵에만 영향을 줍니다. 레이어 스택은 독립적입니다. 일반 응용 프로그램에 권장되는 값:<br><br><ul><li><strong>Unity</strong>: OpenGL</li><li><strong>Unreal 엔진</strong>: DirectX</li><li><strong>Maya</strong>: OpenGL</li><li><strong>3DS 최대</strong>: DirectX</li><li><strong>블렌더</strong>: OpenGL</li></ul></td>
  </tr>
  <tr>
    <td><strong>조각당 접선 공간 계산</strong></td>
    <td>음영 및 조명을 위해 뷰포트에서 표준 맵을 계산하고 표시하는 방법을 결정합니다. 이 옵션을 활성화하면 메쉬의 탄젠트 및 이항식이 정점이 아닌 픽셀 단위로 계산됩니다.<br>일반 응용 프로그램에 대한 권장 값:<br><br><ul><li><strong>Unity</strong>: 사용 안 함(HDRP를 사용하는 경우 사용)</li><li><strong>Unreal 엔진</strong>: 사용</li></ul></td>
  </tr>
</table>

>[!NOTE]
>
> 표준 형식이나 탄젠트 계산을 변경하려면 메쉬 맵을 다시 가져와서 뷰포트의 모양이 올바른지 확인해야 합니다.

### 파일 유형별 설정

USD 메시 포맷을 선택하면 다른 파일 유형별 설정을 사용할 수 있습니다.

![](../assets/image2023-1-30-11-16-6.png){width="473px"}

<table>
  <tr>
    <th><em>매개변수</em></th>
    <th><em>설명</em></th>
  </tr>
  <tr>
    <td><strong>범위 및 변형</strong></td>
    <td>USD 파일의 특정 부분을 선택합니다. 기본적으로 'Root'로 설정됩니다. 즉, 전체 USD 파일이 Painter 프로젝트에서 사용됩니다. <strong>변경...</strong>은(는) USD의 내용을 표시하는 새 창을 엽니다. 변형이 검색되면 프로젝트로 로드할 특정 변형을 선택할 수 있습니다.<br><br>참고:<br><ul><li>선택한 모델링 변형만 영향을 받습니다.</li><li>변형 내에 중첩된 변형은 현재 검색되지 않습니다.</li></ul></td>
  </tr>
  <tr>
    <td><strong>서브디비전 수준</strong></td>
    <td>세분화가 있는 형상에 적용됩니다. Painter에서 텍스처링용 메쉬를 얼마나 세분화할 것인지를 지정합니다. USD 파일 내에서 하위 구분이 명시적으로 '없음'으로 설정된 경우 이 설정은 회색으로 표시됩니다. UV 풀기 후 세분화가 적용되어 메쉬의 UV 모양이 바뀌지 않습니다.</td>
  </tr>
  <tr>
    <td><strong>프레임</strong></td>
    <td>애니메이션이 감지된 USD에 적용됩니다. Painter 프로젝트로 로드할 프레임을 선택합니다. 선택한 USD 파일에 애니메이션이 없는 경우 이 설정은 회색으로 표시됩니다.</td>
  </tr>
</table>

## UV 타일 설정

이 섹션에는 프로젝트에서 UDIM 사용을 전환할 수 있는 컨트롤이 있습니다. 프로젝트를 만든 후에는 이 설정을 변경할 수 없지만 여기에서 프로젝트 설정을 볼 수 있습니다. 자세한 내용은 [UV 타일 설명서](../features/uv-tiles/uv-tiles.md)를 참조하십시오.

## 가져오기 설정

이러한 설정은 선택한 메시를 가져오는 방법을 제어합니다.

| *설정* | *설명* |
| --- | --- |
| **카메라 가져오기** | 이 옵션을 활성화하면 메시 파일에 있는 카메라도 가져와 3D 뷰포트에서 사용할 수 있습니다. |
| **메시에서 선 위치 유지** | 이 설정은 새 3D 메시를 가져온 후 브러시 획을 다시 계산하는 방법을 제어합니다. 대부분의 경우 이 설정을 활성화된 상태로 유지하는 것이 좋습니다. 자세한 내용은 [UV 재투영](../features/uv-reprojection.md) 설명서를 참조하십시오. |
| **자동 언랩** | 자동 UV 풀기. 옵션 버튼을 클릭하여 프로세스를 구성합니다. 자세한 내용은 [자동 UV 감싸기 해제 설명서](../features/automatic-uv-unwrapping.md)를 참조하십시오. |

### 물리적 크기 설정

가져온 메시의 [물리적 크기](../features/physical-size.md)을(를) 조정합니다.

| *설정* | *설명* |
| --- | --- |
| **메시 파일의 내부 단위 비율 사용** | 물리적으로 정확한 측정으로 메쉬를 만든 경우 Painter에서 동일한 물리적 크기를 유지하려면 이 옵션을 선택한 상태로 둡니다. |
| **사용자 지정 단위 크기** | 물리적 크기를 염두에 두고 메쉬를 만들지 않은 경우 이 옵션을 사용하여 메쉬의 크기를 사용자 정의합니다. 이 값을 결정하려면 원하는 물리적 크기와 가져온 메시 단위의 크기를 알아야 합니다. |
| **재질을 할당할 때 채우기 레이어 비율을 물리적 크기로 전환** | 이 옵션을 활성화하면 물리적 크기 속성이 있는 재질을 할당할 때 칠 레이어 및 효과는 비율 조정 방법을 자동으로 물리적 크기으로 전환합니다. |

### 색상 관리 설정

이 섹션에서는 색상을 변환하는 방법에 대한 설정을 제어합니다. 자세한 내용은 [색상 관리](../features/color-management/color-management.md) 설명서를 참조하세요.
