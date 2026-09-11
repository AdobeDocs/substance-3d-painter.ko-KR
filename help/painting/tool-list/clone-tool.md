---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/tool-list/clone-tool.html"
breadcrumb-title: ''
description: Substance 3D Painter의 복제 툴을 사용하면 텍스처 디테일을 한 영역에서 다른 영역으로 복사할 수 있어 텍스처 페인팅이 원활해집니다.
helpx_creative_field: ""
helpx_description: Painter > Painting > Tool list > Clone Tool
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 복제 도구
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 1%

---


# 복제 도구

Substance 3D Painter 2에 도입된 복제 도구는 [페인트 도구](https://support.allegorithmic.com/documentation/display/SPDOC/Paint+brush) 와 동일한 유형의 매개 변수를 공유합니다. 이름에서 알 수 있듯이 [복제] 도구를 사용하면 특정 레이어 또는 전체 레이어 스택의 내용을 한 지점에서 다른 지점으로 복제할 수 있습니다.

![](../../assets/clone-01.gif)

## 사용

[복제] 도구를 사용하는 가장 간단한 방법은 페인팅 레이어의 내용에 사용하는 것입니다.

다음 두 단계로 수행할 수 있습니다.

* 모델에 마우스를 놓고 &quot;**V**&quot; 키를 눌러 원본 위치를 선택합니다.
* 그런 다음 복제된 영역이 나타날 위치에 마우스를 놓고 페인팅을 시작합니다.

&quot;**V**&quot;을(를) 다시 누르면 언제든지 원본을 업데이트할 수 있습니다.

![](../../assets/2018-06-12-18-11-59.png)

기본적으로 복제 도구를 사용하여 페인트할 때는 브러시를 놓은 후에 소스 위치가 그 뒤를 따라 해당 위치를 업데이트합니다. &quot;**복제 원본 동작**&quot;에 사용된 단추를 사용하지 않도록 설정하면 원본은 &quot;**V**&quot;을 누를 때 정의된 위치로 되돌아갑니다. 이는 동일한 소스 영역을 사용하여 여러 번 페인트할 때 유용할 수 있습니다.

복제 도구를 사용하는 더 스마트한 방법은 페인팅 레이어를 만들고 모든 채널의 혼합 모드를 &quot;통과&quot;로 설정하는 것입니다. 이렇게 하면 &quot;복제 레이어&quot; 아래에 있는 모든 레이어에서 비파괴적인 방식으로 정보를 복제할 수 있습니다. 아래 레이어는 그대로 유지되며, 나중에 적용한 모든 수정 사항은 복제 레이어에서 고려됩니다.

![](../../assets/clone-02.gif)
