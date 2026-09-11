---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/stability-issues/crash-with-low-virtual-memory.html"
breadcrumb-title: ''
description: 안정적인 애플리케이션 성능을 보장하기 위해 가상 메모리 부족으로 인해 발생하는 Substance 3D Painter 충돌을 해결하는 방법을 알아보십시오.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Stability Issues > Crash with low virtual memory
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 가상 메모리가 부족한 충돌
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# 가상 메모리가 부족한 충돌

**페이징** 파일(**스왑** 메모리/ **가상** 메모리)이 **너무 낮음** 값으로 설정된 경우 Substance 3D Painter이 불안정할 수 있습니다.\
운영 체제에서 이러한 설정을 처리하도록 하는 것이 좋습니다(일반적으로 기본적으로 이러한 경우). Substance 3D Painter이 제대로 작동하려면 가상 메모리 **최소**(**16GB**)가 필요합니다.

## Windows에서 가상 메모리 크기를 변경하는 방법은 무엇입니까?

>[!NOTE]
>
> Windows에서 가상 메모리 크기를 변경하려면 컴퓨터를 다시 시작해야 합니다.

다음 단계를 통해 가상 메모리 설정에 액세스합니다

1. **컴퓨터/이 PC** 아이콘을 마우스 오른쪽 단추로 클릭하고 **속성**&#x200B;을 선택합니다.
1. &quot;**고급 시스템 설정** 선택
1. **성능** 섹션의 **설정** 단추를 클릭합니다.
1. **고급** 탭을 클릭합니다.
1. **가상 메모리** 섹션에서 **변경**&#x200B;을 클릭합니다.

이제 다음 중 하나를 수행할 수 있습니다.

* **모든 드라이브에 대한 페이징 파일 크기 자동 관리** 확인란을 활성화합니다.

**또는**

* 가상 메모리 크기를 변경할 하드 드라이브를 선택하고 **시스템 관리 크기**&#x200B;를 선택한 다음 **설정** 단추를 클릭하십시오.

**자동:**

![](../../../assets/virtual-memory-default.png)

**수동:**

![](../../../assets/virtual-memory-settings.png)
