---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/features/iray-renderer/iray-settings.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 Ray 렌더러 설정을 구성하여 렌더링 품질과 성능을 제어하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Features > Iray Renderer > Iray Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Iray 설정
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---


# Iray 설정

![](../../assets/iray-settings.png)

Iray 설정은 IRay 뷰포트의 렌더링, 실행 기간 및 품질을 제어합니다.

## Iray 정보

창의 상단 섹션에는 Iray의 상태가 다른 정보와 함께 표시됩니다.

| *설정* | *설명* |
| --- | --- |
| **상태** | 상태는 Ray 가 작동하는 방식을 나타냅니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong>렌더링</strong>(Iray에서 이미지를 계산하는 중)</li><li data-preserve-html="true"><strong>일시 중지됨</strong>(Iray 계산이 중지되었지만 완료되지 않음)</li><li data-preserve-html="true"><strong>완료</strong>(Ray 계산이 완료되었거나 설정 값에 도달함)</li></ul> |
| **해상도** | Iray 이미지의 해상도입니다(기본적으로 뷰포트 크기에 따라 다름). |
| **장면 크기** | 장면/3D 메쉬의 테두리 상자 크기입니다. 단위는 없지만 센티미터 단위로 추정된다. |
| **반복** | Iray가 설정에 정의된 최대값을 초과하여 수행한 계산 패스의 수입니다. |
| **렌더링 시간** | 렌더링하는 동안 경과된 시간으로 설정에 정의된 최대 시간을 초과합니다. |

>[!NOTE]
>
> 반복 수는 렌더링의 최종 품질을 정의합니다. 반복 수가 많을수록 품질이 좋습니다.\
> 그러나 반복은 시간이 걸릴 수 있으므로 최대 시간을 정의할 수 있습니다. 반복은 샘플 수로 정의됩니다.

## 설정

설정이 수정자가 되면 Iray는 렌더링 계산을 시작할 것입니다.\
전용 버튼 을 사용하면 Iray 를 일시 중지하여 이러한 비헤이비어를 방지할 수 있습니다.

![](../../assets/pause-2.png)

| *설정* | *설명* |
| --- | --- |
| **최소 샘플** | 픽셀로 수행되는 샘플의 최소 양 |
| **최대 샘플** | 픽셀 단위로 수행되는 최대 샘플 양 |
| **최대 시간** | Iray에서 계산을 수행할 수 있는 최대 시간입니다.  오른쪽의 드롭다운을 사용하여 단위(초, 분 또는 시간)를 설정할 수 있습니다. |
| **부식성 Sampler 사용** | 이 옵션을 사용하면 보다 고급 조명 반사(빛 무늬)를 계산할 수 있습니다. |
| **Firefly 필터 사용** | 이 옵션을 사용하면 가끔 발생할 수 있는 고립되고 매우 밝은 픽셀을 제거할 수 있습니다. |
| **뷰포트 확인 재정의** | 이 설정을 사용하면 현재 뷰포트 크기를 사용하는 대신 렌더링에 대한 사용자 정의 크기를 정의할 수 있습니다. 아래의 **폭** 및 **Height** 설정을 사용하여 픽셀 단위로 정의할 수 있습니다. |
| **렌더링 저장** | 현재 렌더링(완료되지 않은 경우에도)을 파일로 내보내는 작업. |
| **공유** | 현재 렌더링을 [ArtStation](https://www.artstation.com/)에 공유/내보낼 수 있습니다. |
