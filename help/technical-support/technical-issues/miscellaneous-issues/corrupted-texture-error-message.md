---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/technical-issues/miscellaneous-issues/corrupted-texture-error-message.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 텍스처 기능을 복원하기 위해 손상된 텍스처 오류 메시지를 수정하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Miscellaneous Issues > Corrupted texture error message
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 손상된 텍스처 오류 메시지
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# 손상된 텍스처 오류 메시지

프로젝트의 텍스처가 손상되면 저장 프로세스 중에 오류가 발생하여 프로젝트가 완전히 손상되고 복구할 수 없는 상태가 될 수 있습니다. 그러나 이 문제는 수동으로 해결할 수 있습니다.\
프로젝트를 열 때 손상된 리소스가 로그에 표시되는데, 로그 창에서는 다음과 유사한 오류 메시지가 표시됩니다.

![](../../../assets/corrupt1.png)

## 손상된 리소스 참조 수정

### 1 - 리소스 찾기

오류가 표시되는 첫 번째 단계에서는 문제가 있는 리소스를 찾고 식별합니다.\
대부분의 경우 범인은 **메시 맵**(구운 텍스처)에서 비롯됩니다. 이를 확인하는 빠른 방법은 레이어 스택의 마스크 생성기를 확인하는 것입니다.

손상된 리소스는 다음과 같습니다.

![](../../../assets/corrupt2.png)

>[!NOTE]
>
> 이는 리소스가 단순히 누락되었음을 의미할 수도 있습니다.\
> 확인하려면 슬롯을 지우고 베이크에 수동으로 다시 영향을 미칩니다. 빨간색 십자 썸네일이 여기에 계속 있으면 리소스가 손상되었음을 의미합니다.

### 2 - 리소스 교체

손상된 리소스를 바꾸려면 먼저 해당 리소스에 대한 모든 참조를 제거해야 합니다. 전류가 상대적으로 작으면, 이것은 수동으로 행해질 수 있다.\
그러나 프로젝트가 여러 텍스처 집합 또는 여러 레이어에 걸쳐 있는 경우 [리소스 업데이트 프로그램](../../../features/plugins/resources-updater.md)을 사용하면 손상된 리소스를 찾아서 일시적으로 다른 리소스로 바꿀 수 있습니다.

>[!NOTE]
>
> * 구운 텍스처의 경우에는 [텍스처 설정](../../../interface/texture-set/texture-set-settings.md) 창에서 메시 맵 슬롯도 지우는 것을 잊지 마십시오.
> * 표준 맵과 같이 텍스처 설정 에서만 사용되는 베이크도 손상될 수 있습니다. 오류가 지속되는 경우 이러한 오류도 제거해 보십시오.

### 3 - 정리

손상된 리소스에 대한 모든 참조가 사라지면 기본 메뉴(**파일** > **정리**)에서 프로젝트 정리를 수행합니다.\
이렇게 하면 현재 사용되지 않는 손상된 모든 리소스가 프로젝트에서 제거됩니다. 선반에서 프로젝트 탭으로 이동하여 문제가 있는 리소스가 모두 사라졌는지 확인할 수 있습니다.

### 4 - 저장

정리 후에 프로젝트 를 저장해 봅니다.

* 오류 없이 저장하면 이제 프로젝트가 손상되지 않습니다(이제 메시 맵을 다시 굽고 리소스를 다시 가져올 수 있음).
* 오류가 남아 있으면 프로젝트에 손상된 리소스에 대한 참조가 남아 있음을 의미합니다.
