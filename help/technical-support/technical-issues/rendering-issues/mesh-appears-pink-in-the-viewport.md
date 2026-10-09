---
breadcrumb-title: ""
description: Substance 3D Painter 뷰포트에서 핑크 메쉬 모양을 수정하여 적절한 재질 렌더링을 복원하는 방법을 알아봅니다.
title: 뷰포트에서 메쉬가 분홍색으로 표시됩니다
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 0%
---

# 뷰포트에서 메쉬가 분홍색으로 표시됩니다

![](../../../assets/pink-mesh.jpg){width="400px"}

**로그 창**&#x200B;에서 언급한 대로 **셰이더**&#x200B;를 그리는 데 사용된 **셰이더**&#x200B;가 더 이상 컴파일되지 않기 때문에&#x200B;**분홍**&#x200B;이 뷰포트에 표시될 수 있습니다. 최신 버전의 셰이더 API을 지원하지 않는 오래된 셰이더가 원인일 수 있습니다.

해결 방법은 다음과 같습니다.

* **기본 셰이더**&#x200B;의 경우: [셰이더 업데이트](../../../interface/shader-settings/updating-a-shader.md) 페이지의 단계별 절차를 따르십시오.
* **사용자 지정 셰이더**&#x200B;의 경우: 로그 창과 [셰이더 API](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/custom-shader-api-89686018.html) 페이지의 오류 메시지를 확인하십시오.
