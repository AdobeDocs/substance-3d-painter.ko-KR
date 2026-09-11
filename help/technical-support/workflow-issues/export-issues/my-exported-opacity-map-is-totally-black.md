---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/workflow-issues/export-issues/my-exported-opacity-map-is-totally-black.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 불투명도 맵을 수정하여 투명도를 적절하게 내보내는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Export Issues > My exported opacity map is totally black
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 내보낸 불투명도 맵이 완전히 검정색입니다.
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 0%

---


# 내보낸 불투명도 맵이 완전히 검정색입니다.

새 프로젝트를 만들 때 기본 색상은 텍스처가 아니라 셰이더에서 옵니다. 따라서 페인트를 지정하지 않은 모든 부품을 내보내면 해당 부품에 데이터가 없기 때문에 알파 값이 0으로 설정된 검정색이 됩니다.

이 문제를 해결하는 가장 쉬운 방법은 레이어 스택 하단에 채우기 레이어를 배치하는 것입니다. 이 경우 셰이더의 기본 색상과 동일한 기본 색상으로 모든 UV를 채웁니다.
