---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/features/post-processing/tone-mapping.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 톤 매핑 후처리를 사용하여 뷰포트에서 노출 및 색 보정을 조정하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Tone Mapping
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 톤 매핑
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---


# 톤 매핑

![](../../assets/tone-mapping.png)

톤 매핑 매개 변수를 사용하면 색상을 화면에 표시되도록 비율을 조정하는 방법을 제어할 수 있습니다. 이러한 설정은 현재 화면에서 표시할 수 있는 범위를 초과할 수 있는 광범위한 값 때문에 색상을 재분포하는 데 유용할 수 있습니다.

>[!NOTE]
>
> Substance 3D Painter에서는 **HDR**(High Dynamic Range) 색상(선형 감마 공간)을 출력하지만 대부분의 화면에서는 **LDR**(낮은 동적 범위) 색상만 시각화할 수 있습니다. HDR 범위를 LDR 범위에 매핑하려면 변환을 수행해야 합니다. 이것이 톤 매핑의 원리입니다.

| *설정* | *설명* |
| --- | --- |
| **노출** | 눈부심 효과가 적용되거나 톤 매핑이 발생하기 전에 HDR 공간 렌더링 결과의 크기를 조정합니다. |
| **감마** | 감마 교정의 감마 값입니다. |
| **함수** | HDR 범위를 LDR 범위에 매핑하는 데 사용할 함수입니다.  사용 가능한 기능은 다음과 같습니다.<ul data-preserve-html="true"><li data-preserve-html="true"><strong> 자동 </strong> : 톤 맵 함수가 자동으로 선택됩니다. 기본값은 <strong> Sensitometric </strong> 입니다. </li><li data-preserve-html="true"><strong> 선형 </strong> : 이 유형의 경우에만 출력 색상이 0에서 1로 클램프되지 않습니다. 이는 효과를 적용한 후 애플리케이션 측의 HDR 공간에서 일부 효과를 구현할 때 최적입니다. <br/>선형 매핑을 최종 화면 출력으로 사용하면 높은 광도 구성 요소가 완전히 손실되고 밝은 영역이 날아가기 때문에 사용할 특별한 이유가 없으면 이 방법을 사용하지 않는 것이 좋습니다.</li><li data-preserve-html="true"><strong> LinearSat </strong> : 출력 색상이 고정되어 있다는 점을 제외하면 <strong> Linear </strong> 과(와) 거의 동일합니다. 또한 눈부심 합성이 <strong> 선형 </strong> 보다 조금 더 매끄럽습니다.</li><li data-preserve-html="true"><strong> Sensitometric </strong> : HDR 공간에서 장면 렌더링을 수행할 때 기본 함수입니다.</li><li data-preserve-html="true"><strong> Reinhard </strong> : <strong> Sensitometric </strong> 보다 더 점진적으로 매핑하고 대비가 약간 낮습니다. 이에 의해, 고휘도 성분의 해상도가 높아져, 밝은 부분의 휘도 편차를 보다 강하게 재현시킬 수 있다.</li><li data-preserve-html="true"><strong> ReinhardLum </strong> : 광도를 참조로 하여 <strong> Reinhard </strong> 톤 맵을 구현하고 원래 채도(선명도: RGB 비율)를 유지하기 위한 유형입니다. 광도 정보만 LDR 공간에 매핑하고 원래 채도를 재현합니다. 톤 매핑 후에도 HDR 공간의 채도가 유지됩니다.</li><li data-preserve-html="true"><strong> 로그 </strong> : 이로 인해 <strong> 라인하드 </strong> 보다 더 점진적으로 매핑되고 대비가 낮습니다. 이는 고휘도 성분의 해상도가 높아지고, 밝은 부분의 휘도 편차를 가장 강하게 재현시키는 원인이 된다.</li><li data-preserve-html="true"><strong> LogLum </strong> : 광도를 참조로 하여 로그 공간의 톤 맵을 구현하고 원래 채도를 유지하기 위한 유형입니다(선명도: RGB 비율). 이는 광도 정보만을 로그 공간에 매핑한 다음 원래 채도를 재현합니다. 톤 매핑 후에도 HDR 공간의 채도가 유지됩니다.</li></ul> |
| **매핑 요소** | 이는 톤 매핑 프로세스의 최종 LDR 공간에 매핑되는 HDR 공간의 광도(밝기)에 대한 최대 레벨을 제어합니다. 지정된 HDR 공간 광도보다 밝은 색상은 LDR 공간에 표시할 수 없으므로 밝은 영역이 날아갑니다. 즉, 이 값은 LDR 공간의 최대 광도 값(1.0)에 매핑되는 HDR 공간의 광도(노출 비율 조정 후)입니다. HDR 렌더링 모드에서 이 값이 낮을수록 대비가 높아지고 밝은 영역이 날아갈 가능성이 커집니다. 반대로 값을 높게 지정하면 대비가 낮아지고 밝은 영역이 날아갈 가능성이 줄어듭니다. LDR 렌더링 모드에서 효과를 적용하기 위해 HDR 공간에 다시 매핑하는 경우 광도 범위가 **매핑 요소**&#x200B;에 지정된 값까지 확장됩니다. 반대로 **매핑 요소** 광도는 톤 매핑 중 최대 LDR 광도에 매핑됩니다.즉, 효과 적용에 대해 LDR 렌더링 결과에 적용되는 동적 범위 비율 조정 요소를 지정합니다. 이 값을 높은 값으로 설정하면 효과에서 밝은 영역이 강조됩니다.  **참고:** HDR 렌더링 모드에서 **함수**&#x200B;가 **선형** , **선형 채도** 또는 **센시토메트릭** 중 하나로 설정된 경우 이 설정은 영향을 주지 않습니다(무시됨). |
