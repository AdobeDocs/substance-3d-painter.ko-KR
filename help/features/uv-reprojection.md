---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/uv-reprojection.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 UV 재투영을 사용하여 다른 UV 레이아웃 간에 텍스처를 전송하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Features > UV Reprojection
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: UV 재투영
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# UV 재투영

UV 재투영은 텍스처 해상도를 변경하거나 새 메쉬를 가져올 때 발생하는 자동 프로세스입니다.\
[프로젝트 구성](https://substance3d.adobe.com/display/draftpainter/project%20configuration) 창을 통해 문서에 새 메시를 로드하면 모든 작업이 해당 새 메시에 다시 투영됩니다. 토폴로지가 변경되었는지(유사한 경우) 또는 UV가 변경되었는지 여부는 중요하지 않습니다. 재투영은 모든 레이어와 브러시 획을 다시 계산해서 작업하기 때문에 시간이 조금 걸릴 수 있습니다(특히 텍스처 해상도가 높은 경우).

2D 보기로 페인팅

2D 보기에서 만든 모든 획은 UV 공간에서 수행되므로 다시 가져온 후 메쉬의 UV가 크게 변하는 경우 적절하게 재투영할 수 있는 방법이 없습니다. 프로젝트 재투영 방지를 만드는 가장 좋은 방법은 3D 보기 대신 ID 맵과 다른 유형의 선택 및 페인팅에 의한 마스크에 의존하는 것입니다.

## 재투영은 어떻게 작동합니까?

Substance 3D Painter은 데이터를 월드 공간에서 3D로 저장하여 모든 것을 비파괴적으로 유지합니다. 즉, 메시를 다시 가져올 때 Substance 3D Painter은 다시 가져오기 전에 메시가 있던 위치를 페인트하려고 하지만 일부 조각이 어디로 이동했을 수 있는지 알 수 없습니다.

또한 Substance 3D Painter에서 메시를 가져올 때는 경계 상자를 계산하여 공간을 등록하고 도구(페인트 브러시, 파티클 등)의 상대 비율을 정의합니다. 이 테두리 상자는 모든 축에서 1단위 너비입니다. 새 메시를 가져올 때 &quot;선 유지&quot;를 선택 해제하면 테두리 상자가 새 메시로 다시 표준화됩니다. 따라서 메쉬의 크기가 크게 변경되면 선이 이동할 수 있습니다. 그러나 &quot;선 유지&quot;를 선택하는 경우 브러시 선을 올바르게 다시 투영하기 위해 원래 테두리 상자의 크기를 새 테두리 상자로 조절합니다.

>[!WARNING]
>
> 3D 메쉬의 단위를 변경하면 UV 재투영이 작동하지 않을 수 있습니다. 토폴로지가 변경되지 않았더라도 이전 메쉬와 새 메쉬는 크기가 크게 다른 것으로 해석될 수 있습니다. 수정이 어려울 수 있으므로 장치 설정을 변경하지 않는 것이 좋습니다.
