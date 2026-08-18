---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/rendering-issues/broken-viewport-ubuntu.html"
breadcrumb-title: ''
description: 적절한 3D 렌더링을 위해 Substance 3D Painter의 Ubuntu에서 끊기거나 응답하지 않는 뷰포트 문제를 해결하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Viewport appears broken or unresponsive on Ubuntu
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 뷰포트가 Ubuntu에서 손상되었거나 응답하지 않음
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---


# 뷰포트가 Ubuntu에서 손상되었거나 응답하지 않음

버전 11.1부터 Steam의 Ubuntu에서 Painter을 실행할 때 뷰포트가 손상되거나 응답하지 않을 수 있습니다.

이는 적절한 GPU가 할당된 상태에서 시작하지 않는 Painter과 관련이 있습니다. 우분투에서 별도의 GPU 대신 통합 GPU를 선택하면 됩니다. Painter은 문제를 일으킬 수 있는 Steam을 통해 이 구성을 상속합니다.

다음과 같은 몇 가지 해결 방법이 있습니다.

1. 터미널에서 Steam을 실행합니다. 이렇게 하면 다른 컨텍스트가 강제로 적용되며 Steam 및 Painter이 올바른 GPU에서 실행되도록 해야 합니다.
1. Steam 바로 가기를 편집하여 <b>전용 그래픽 카드를 사용하여 실행</b> 설정을 비활성화합니다. 그런 다음 Steam을 정상적으로 실행하십시오.

자세한 내용은 [이 github 문제](https://github.com/ValveSoftware/steam-for-linux/issues/9940)를 참조하세요.
