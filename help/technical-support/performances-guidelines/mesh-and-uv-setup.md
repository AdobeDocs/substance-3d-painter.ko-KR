---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/performances-guidelines/mesh-and-uv-setup.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 성능 및 텍스처 품질을 최적화하기 위해 메시 및 UV 설정에 대한 모범 사례를 알아보십시오.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Performances guidelines > Mesh and UV setup
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 메쉬 및 UV 설정
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# 메쉬 및 UV 설정

Painter용 메쉬를 준비하는 데 몇 분 정도 소요되면 텍스처링 프로세스를 더 빠르고 쉽게 수행할 수 있습니다.

+++높은 폴리카운트 모델
Painter에서 처리할 수 있는 polycount에 대한 특정 벤치마크는 없습니다. 이는 컴퓨터 사양, 텍스처 세트 할당 및 레이어 스택 속성에 따라 크게 다르지만 레이어 스택 최적화를 고려할 경우 1,000만 개 미만의 polys는 잘 처리해야 합니다.

+++

+++낮은 폴리카운트 모델
너무 낮은 폴리 같은 것이 있다. 텍스처 엔진에서는 다각형을 사용하여 브러쉬 선을 계산하기 위해 렌더링할 메시 부분을 알기 때문입니다. 폴리카운트가 매우 낮은 메시는 GPU를 불필요하게 오버워크할 수 있는 작은 브러시 획에도 완전히 다시 렌더링할 수 있습니다.

예를 들어 하나의 4중 평면을 텍스처링하는 경우 정보가 더 많은 정점에 분산되므로 특히 획이 많은 손으로 페인팅할 때는 메쉬를 세분화하는 것이 좋습니다.

+++

+++여러 텍스처 세트에서 텍스처 나누기
더 복잡한 재질 할당이 있는 더 큰 메시를 여러 [텍스처 세트]로 분할하는 것이 좋습니다. 텍스처 세트를 사용하면 해상도 및 셰이더 속성과 같은 텍스처 세트별로 다른 설정을 할당할 수 있습니다. 예를 들어, 메시 중 일부에서만 반투명도나 SSS를 사용하는 경우 해당 부분에 다른 텍스처 세트 및 다른 셰이더 인스턴스를 할당하는 것이 가장 좋습니다. 이렇게 하면 훨씬 복잡한 속성을 사용하지 않는 곳에서 계산할 필요가 없습니다.

+++

+++UV 섬을 가깝게 유지
3D 공간에서 이웃인 UV 섬을 가깝게 유지하세요. 이는 UDIM 레이아웃과 클래식 UV 공간 레이아웃 모두에 적용됩니다. 페인트 선이나 텍스처링을 공유한 경우에는 반대쪽 끝에 있는 경우보다 UV 공간의 같은 영역에 모여 있을 때 더 쉽게 계산할 수 있습니다.

텍스처 엔진은 텍스처를 더 작은 청크로 분할하여 계산 속도를 높여 작동합니다. 즉, 각 획이 모든 획으로 전체 텍스처를 업데이트하지 않고 변경해야 하는 청크만 업데이트합니다. 인접한 UV 섬을 서로 가깝게 유지함으로써, 단일 스트로크에 의해 영향을 받을 청크의 수를 최소화한다.

+++

+++오브젝트가 너무 많으면 안 됩니다
성능은 8000개 미만의 하위 개체가 있는 메시를 가져올 때 편안해야 합니다. 이 한도를 초과하면 뷰포트 및 페인팅 성능에 영향을 줄 수 있습니다. 이 제한에 도달하면 개체를 함께 병합하여 렌더링 오버헤드를 줄이는 것이 좋습니다.

+++
