---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/assets/navigation.html"
breadcrumb-title: ''
description: Substance 3D Painter의 에셋 패널로 이동하여 리소스 라이브러리를 효율적으로 검색하고 액세스하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Interface > Assets > Navigation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 탐색
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 1%

---


# 탐색

에셋 창에는 탐색 경로, 검색 필드 및 에셋 유형 아이콘과 같은 여러 가지 탐색 방법이 있습니다. 모든 내비게이션 유형은 상호 종속적이므로 이러한 검색을 결합하여 사용자의 장점을 활용할 수 있습니다.\
예를 들어 에셋 유형 아이콘에서 재질을 선택했지만 경로 기록을 사용하여 스마트 마스크 폴더로 이동한 경우 [에셋] 패널에 결과가 표시되지 않습니다. 재질을 표시하려면 모든 라이브러리로 돌아가고 스마트 마스크를 찾으려면 재질을 선택 해제해야 합니다.

## 탐색 경로

탐색 경로를 사용하면 라이브러리를 빠르게 탐색할 수 있습니다. 화살표를 클릭하면 자산이 디스크에 저장되는 방법이 표시되며 표시된 위치를 선택할 수 있습니다. 회색으로 표시된 경우 해당 폴더에 선택한 유형의 에셋이 없지만 해당 위치로 이동할 수 있습니다.

![](../../assets/00-05-breadcrumbs.jpg)

## 검색 필드

검색 필드는 형식화된 쿼리가 포함된 리소스를 필터링하는 데 사용할 수 있습니다. 참고: 리소스 제목뿐만 아니라 리소스 위치 및 리소스 내에 포함된 모든 태그를 검색합니다.\
입력된 검색은 키워드보다 더 고급일 수도 있습니다. [고급 검색 쿼리](advanced-search-queries.md)를 참조하세요.

![](../../assets/00-05-searchfield.jpg)

## 에셋 유형

>[!NOTE]
>
> 클릭할 때 **Ctrl**&#x200B;을(를) 유지하여 에셋 유형 아이콘을 다중 선택할 수 있습니다.

기본 선택은 재질이지만, 다른 자산 유형 아이콘을 클릭하면 다른 유형의 리소스가 표시됩니다.

![](../../assets/00-05-assettypeicons.jpg)

| 에셋 유형 | 설명 |
| --- | --- |
| 재질 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r1-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1-1.png"/></div> | *기본 재질*(으)로 가져온 .sbsar과 채우기 레이어에서 만든 재질을 포함합니다(사전 설정 만들기에 대한 자세한 내용은 [여기](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/creating-and-saving-a-preset-180191514.html)에서 확인할 수 있습니다). 이 재질은 채우기 레이어에서 사용할 수 있으며 메쉬 또는 텍스처 집합의 전체 표면에 적용됩니다. |
| 스마트 재질 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r2-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-7.png"/></div> | 폴더 내에 저장된 여러 레이어로 구성된 보다 복잡한 재질을 포함합니다(스마트 재질은 직접 만들 수 있는 사전 설정이기도 합니다).기본 재질과 마찬가지로 스마트 재질은 메시/텍스처 세트 전체에 적용되지만 곡률, 오클루전 또는 기타 표면 세부 사항과 같은 메시의 개별 정보도 고려합니다. 이러한 표면 세부 사항을 얻고 스마트 재질을 올바르게 사용하려면 먼저 메쉬를 [구워](../../baking/baking.md)해야 합니다. |
| 스마트 마스크 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r3-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-2.png"/></div> | 다중 레이어 효과 및/또는 생성기를 사용하는 보다 복잡한 마스크를 포함합니다. 스마트 마스크 사전 설정을 직접 [만들기](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html)할 수 있습니다.스마트 재질과 마찬가지로 스마트 마스크도 올바르게 작동하려면 메시에서 구운 정보가 필요합니다. |
| 필터 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r4-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-3.png"/></div> | *filter*(으)로 가져온 .sbsar 파일을 포함합니다.필터는 이미 있는 텍스처를 특정 방식으로 변형하는 효과입니다. 일부 필터는 흑백 정보에서만 작동하고, 일부는 재료 입력에서만 작동하므로, 마스크에 일부 필터를 사용할 수 없습니다. |
| 브러시 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r5-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-4.png"/></div> | 브러쉬, 파티클 및 도구를 포함합니다. 이는 모두 Painter에서 [생성](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html)할 수 있는 사전 설정입니다.**브러시**&#x200B;는 알파를 사용하는 기본 흑백 사전 설정입니다. 브러시를 사용하여 일부 또는 모든 채널이나 마스크에서 페인트할 수 있습니다.**파티클**&#x200B;에는 브러시와 같은 특성이 있지만 메시와의 물리적 상호 작용을 시뮬레이션하는 추가 매개 변수 집합도 있습니다. 그들은 엎지름, 물방울, 비 또는 물리적 시뮬레이션이 필요한 다른 어떤 것의 효과를 낼 수 있다.**도구**&#x200B;에는 브러시 및/또는 입자 비헤이비어가 포함될 수 있지만, 이 사전 설정은 재질 채널 정보에도 저장됩니다. |
| 알파 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r6-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-5.png"/></div> | 다양한 알파와 보다 정교한 효과로 [만들기](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/managing-assets-217187091.html)할 수 있는 여러 브러시 메이커(Photoshop 같은, 역동적인 획, 페인트 롤러)를 포함합니다.Alpha은 검정 부분이 사용될 때 투명하게 표시되는 회색 음영 이미지입니다. |
| 텍스처 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r7-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-6.png"/></div> | 그런지, 절차, 베이킹된 맵, 단단한 표면 표준 및 LUT를 포함합니다.**그런지**&#x200B;는 흥미로운 노이즈와 텍스처가 있는 회색 음영 이미지입니다. 마스크를 통하거나 채널에 직접 연결하여 메쉬 표면에 변형을 추가하는 데 사용할 수 있습니다.**절차**&#x200B;는 또한 노이즈나 일반 패턴으로 구성된 회색 음영 텍스처입니다. 그러나 일부 정적 그런지와 달리 프로시저는 반복 없이 크기를 조절할 수 있고 무작위 시드를 통해 무한 변동을 가질 수 있는 동적 비트맵입니다.**베이킹된 맵**&#x200B;은 메시에서 추출한 표면 및 모양 정보를 나타냅니다. 굽기에 대한 자세한 내용은 여기를 참조하십시오.**단단한 표면 표준**&#x200B;은 표준 채널을 사용하여 메시에 직접 스탬프할 수 있는 세부 정보입니다.**LUT**(조회 테이블)은 디스플레이 설정에서 뷰포트의 색상 프로필 동작을 시뮬레이션하는 데 사용할 수 있는 색상 프로필 텍스처입니다. [여기](../../features/post-processing/color-profile.md)에서 색상 프로필에 대해 자세히 알아볼 수 있습니다. |
| 환경 맵 <div><img class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_dx_table_row-r8-column-c0_dynamic_grid_items_grid-cell_position-par_image" src="../../assets/00-05-assettypes-1.jpg"/></div> | *환경*(가장 일반적으로 .hdr 또는 .exr)으로 가져온 이미지를 포함합니다.환경 맵은 조명 설정을 자동으로 생성하는 배경 이미지입니다. 환경 맵을 뷰포트로 직접 드래그하거나 디스플레이 설정을 통해 환경 맵을 사용할 수 있습니다. |
