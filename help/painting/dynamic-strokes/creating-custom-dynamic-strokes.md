---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/dynamic-strokes/creating-custom-dynamic-strokes.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 사용자 정의 역동적인 획을 만들어 독특한 브러시 획 비헤이비어 및 효과를 디자인하는 방법을 살펴봅니다.
helpx_creative_field: ""
helpx_description: Painter > Painting > Dynamic strokes > Creating Custom Dynamic Strokes
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 사용자 정의 역동적인 획 만들기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# 사용자 정의 역동적인 획 만들기

사용자 정의 역동적인 획을 만들기 위해 다음 두 가지 옵션을 사용할 수 있습니다.

* 기존 Substance 리소스를 사용하여 새 브러시/도구 사전 설정 만들기
* 처음부터 새 Substance 리소스를 만듭니다([Substance 3D Designer](https://substance3d.adobe.com/display/SDDOC/Substance+Designer) 필요).

또한 오류를 방지하기 위해 사용자 지정 Substance 파일을 만들기 전에 [동적 선 성능](dynamic-stroke-performances.md)을 읽는 것이 좋습니다.

## 기존 리소스 재사용

처음부터 새 역동적인 획을 만드는 것은 어려울 수 있습니다. 기존 리소스를 사용하여 조정하고 새 사전 설정으로 저장하면 시작점으로 충분합니다.

셸프에서 필요에 맞는 호환 가능한 리소스를 찾은 다음 [사전 설정](../presets/presets.md)에 대한 페이지를 확인하세요.

## 역동적인 획에 대한 사용자 정의 Substance 파일 만들기

다음은 Substance 그래프의 역동적인 획에 대해 지원되는 매개 변수 목록입니다.

| 변수 식별자 | 설명 |
| --- | --- |
| <b>임의화</b> | Substance 파일이 [임의화]를 노출한 상태로 요리되는 경우 동적 선 기능을 사용하여 제어할 수 있습니다. |
| <b>stampIndex</b> | 브러시 획을 페인트할 때 Substance 3D Painter에서 <b>Integer1</b>을(를) 제공합니다. 최소값과 최대값은 영향을 주지 않으므로 Substance 3D Painter은 해당 값을 무시합니다. |
| <b>stampCycleCount</b> | <b>Integer1</b> Painter은 매개 변수 기본값, 최소값 및 최대값을 읽어서 스탬프 사이클 수 매개 변수를 표시합니다. 이 매개 변수는 만들 고유한 Substance 변형의 수를 제어합니다. |
| <b>$time</b> | <b>Float1</b>은(는) 경과된 페인팅 시간(스트로크당)을 기준으로 브러시 스트로크를 페인팅할 때 Substance 3D Painter에서 공급됩니다. 이 속성은 많은 Substance 변형을 생성할 수 있으므로 성능에 영향을 줄 수 있습니다. |
| <b>선 간격</b> | <b>float1</b> 칠해진 전체 선에 대한 현재 간격 값입니다. |
| <b>strokeSize</b> | <b>float1</b> 칠해진 전체 선의 현재 크기 값입니다. |
| <b>stampStrokePosition</b> | <b>integer1</b> 선의 시작/시작을 지정하는 데 사용됩니다. 끝 값은 수동 페인팅이 아닌 패스 선에서만 사용할 수 있습니다. 가능한 값:<ul data-preserve-html="true"> <li data-preserve-html="true">0 = 중간</li> <li data-preserve-html="true">1 = 시작</li> <li data-preserve-html="true">2 = 끝</li> </ul>isstrokepositionactive 사용자 태그를 사용하여 비활성화할 수 있습니다. |
| <b>distanceAlongCurve</b> | <b>float1</b> 지정된 스탬프에서 패스를 따라 이동한 현재 거리입니다. 이 속성은 많은 Substance 변형을 생성할 수 있으므로 성능에 영향을 줄 수 있습니다. <b>iscurvedistanceactive</b> 사용자 태그로 사용하지 않도록 설정할 수 있습니다. |
| <b>distanceMaxCurve</b> | <b>float1</b> 패스 도구를 사용하여 만든 패스의 총 길이입니다. <b>iscurvedistanceactive</b> 사용자 태그로 사용하지 않도록 설정할 수 있습니다. |
| <b>pathCorner</b> | <b>integer1</b> 리본에서 사용 중인 모퉁이 유형을 나타냅니다. 가능한 값:<ul data-preserve-html="true"> <li data-preserve-html="true">0 = 모서리 없음</li> <li data-preserve-html="true">1 = 왼쪽 모서리</li> <li data-preserve-html="true">2 = 오른쪽 모서리</li> </ul> |
| <b>pathCornerAngle</b> | 리본 경로 모서리의 <b>부동</b> 각도(반경 단위)입니다. 정확한 각도 값을 기반으로 모퉁이의 모양을 보정하거나 조정하는 데 사용할 수 있습니다. |
| <b>patchLengthOnCurve</b> | 리본 경로에서 섹션(패치)의 <b>부동</b> 크기입니다. <b>distanceAlongCurve</b> 및 <b>distanceMaxCurve</b>과 함께 사용하면 예를 들어 패치의 크기를 표준화할 수 있습니다. |
