---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/mesh-flash-to-white-when-moving-camera.html"
breadcrumb-title: ''
description: 안정적인 렌더링을 위해 Substance 3D Painter 뷰포트에서 카메라를 이동할 때 메쉬가 흰색으로 깜박이는 문제를 해결하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Mesh flash to white when moving camera
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 카메라 이동 시 메시 플래시가 흰색으로 바뀜
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# 카메라 이동 시 메시 플래시가 흰색으로 바뀜

![](../../../assets/white-flash-svt-optim.gif){width="300px"}

이전 프로젝트가 뷰포트에서 카메라 주위로 이동하면 흰색/빈 텍스처로 생성된 흰색 플래시가 잠깐 표시될 수 있습니다. 이는 [SVT(Sparse Virtual Textures](https://substance3d.adobe.com/display/DRAFTPAINTER/Sparse+Virtual+Textures)) 시스템이 이전 셰이더가 사용하지 않는 특정 셰이더 구성에 의존하기 때문입니다.

흰색 플래시를 제거하려면 **프로젝트 셰이더**&#x200B;를 **업데이트**&#x200B;하면 됩니다.

* **기본 셰이더**&#x200B;의 경우: [셰이더 업데이트](../../../interface/shader-settings/updating-a-shader.md) 페이지의 단계별 절차를 따르십시오.
* **사용자 지정 셰이더**&#x200B;의 경우: 로그의 오류 메시지와 [셰이더 API](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html) 페이지를 확인하세요.
