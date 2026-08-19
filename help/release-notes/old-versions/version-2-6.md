---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/release-notes/old-versions/version-2-6.html"
breadcrumb-title: ''
description: Substance 3D Painter 버전 2.6의 릴리스 노트를 검토하여 새로운 기능, 개선 사항 및 버그 수정에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Painter > Release notes > Old versions > Version 2.6
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 버전 2.6
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 0%

---


# 버전 2.6

**Substance Painter 2.6**&#x200B;에서는 새 프로젝트를 만들거나 업데이트된 재질 이름으로 메시를 다시 가져올 필요 없이 Substance Painter 내에서 직접 텍스처 세트를 관리할 수 있는 방법을 제공하는 데 중점을 두었습니다. 또한 프로젝트에서 사용되는 리소스를 업데이트할 수 있는 방법을 제공하고자 했습니다. 과거에 많이 요청했던 내용이었습니다.

출시일: *27 2017년 4월*

## 주요 기능

### 새 샘플 프로젝트 &quot;Meet Mat&quot;

![](../../assets/meetmat-render.jpg)

이 새 샘플 프로젝트에서는 &quot;**Mat**&quot;이라는 이름의 반짝이고 사랑스러운 새 캐릭터를 제공합니다. 페인팅할 준비가 된 3개의 텍스처 세트가 포함되어 있습니다.\
**Meet Mat** 대회에 참가하여 멋진 경품을 획득하세요. <https://www.allegorithmic.com/contest/meet-mat-2017-substance-3d-painting-contest>

### 프로젝트의 리소스를 업데이트하는 기능이 포함된 새 스크립팅 API

![](../../assets/resources-updater-ui.jpg)

프로젝트의 **리소스를 다른 버전으로 바꾸기**&#x200B;할 수 있는 새 함수를 추가하도록 Substance Painter 스크립팅 API가 개선되었습니다. 이 새로운 기능을 시연하기 위해 스크립팅 API로 만든 새 **플러그인**&#x200B;이 추가되었으며 지정된 프로젝트에 포함된 모든 리소스를 검색할 수 있습니다. 빨간색으로 표시된 리소스는 &quot;오래된&quot; 리소스로 감지되며 자동으로 대체될 수 있습니다. 이 기능은 &quot;오래된&quot; 리소스에 한정되지 않으며 모든 에셋을 다른 것으로 대체할 수 있습니다. 이는 많은 새로운 가능성을 제공하며 Substance Painter이 **비파괴적 페인팅 도구**!인 방법을 더 많이 보여줍니다.

**플러그인**&#x200B;은(는) GitHub에서 사용할 수 있습니다. 잠재적인 개선 사항이 표시되면 언제든지 도움을 요청하십시오. <https://github.com/AllegorithmicSAS/painter-plugin-resources-updater>

![](../../assets/resource-update-demo.gif)

### 텍스처 세트의 이름을 바꾸고 재할당하는 새로운 기능

![](../../assets/texture-set-rename-description.png)

이제 Substance Painter 내부에 직접 설정된 텍스처의 이름을 변경할 수 있습니다. 텍스처 세트의 이름을 바꾸면 사용된 내보내기 사전 설정에 따라 디스크에서 내보내는 텍스처의 이름에 영향을 미칩니다.\
텍스처 세트의 이름을 바꾸려면 해당 이름을 두 번 클릭하여 수정하거나 마우스 오른쪽 버튼을 클릭하여 컨텍스트 메뉴를 엽니다. 사용자 정의 설명을 추가하여 텍스처 세트의 역할에 대한 자세한 정보를 제공할 수도 있습니다. 이 기능은 [UDIM 프로젝트](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/uv-tile-udim-legacy-144310352.html)에서 작업할 때 매우 유용합니다. &quot;**설정**&quot; 단추를 사용하여 설명이 목록에 표시되는 방법을 구성하십시오.

![](../../assets/reasign-texture-set.png)

이제 텍스처 세트를 다른 메시 재질에 재할당할 수 있습니다. 즉, 이전에 사용하지 않도록 설정되었던 텍스처 세트를 **복구**&#x200B;하거나(메시에 없기 때문에) **교체**&#x200B;할 수 있습니다. [텍스처 집합 목록] 창에서 새 &quot;**설정**&quot; 단추를 클릭하고 &quot;**텍스처 집합 다시 할당**&quot; 항목을 클릭하면 됩니다. [텍스처] 세트와 해당 세트가 [메시 재질]에 연결되는 방식을 관리하는 데 사용되는 새 창이 열립니다. 텍스처 집합 이름을 원하는 위치로 **끌어 놓기**&#x200B;하면 관리를 수행할 수 있습니다.

## 튜토리얼

새로운 주요 기능은 최신 비디오 튜토리얼에서 다룹니다.

## 릴리스 정보

### 2.6.2

(2017년 10월 20일 릴리스)

**추가됨 :**

* [텍스처 세트] 비활성화된 텍스처 세트 삭제 허용
* [Shelf] 여러 사용자가 동일한 Shelf 폴더 내에 쓸 수 있도록 허용합니다.
* [스크립팅] 플러그인 폴더를 다시 로드할 수 있음
* [스크립팅] 호환성을 보장하기 위해 플러그인 메타데이터에 필요한 최소 API 버전을 추가합니다
* [IRay] 이미지 내보내기 대화 상자 개선

**고정:**

* [엔진] 해상도 변경 시 획이 사라지는 문제(4K>2K)
* [Bakers] 이름으로 일치가 활성화된 상태에서 ID 맵 굽기가 실패했습니다.
* [베이커] 오류 메시지가 충분히 명시적이지 않음
* [3D 보기] 접선 공간이 베이커와 동기화되지 않습니다.
* [도구] 손가락 도구를 사용할 때 검은색 가공물
* [Shader] 비 PBR 셰이더가 더 이상 작동하지 않습니다.
* [Shader] &quot;pbr-coated&quot;가 끊어졌습니다.
* [Shader] &quot;pbr-coated&quot; 셰이더의 코팅 거칠기는 더 이상 영향을 주지 않습니다.
* [Shader] 사양 광택 셰이더가 Iray 및 SD와 일치하지 않습니다.
* [Shelf] 이름은 같지만 확장명이 다른 두 파일을 로드할 때 충돌이 발생합니다
* [Shelf] 선반에서 더 이상 사전 설정을 편집할 수 없음
* [Shelf] 셸프에 가져온 에셋에 대해 사용자 정의 미리 보기를 설정할 수 없습니다.
* 캐시에서 로드된 리소스는 사용을 잃게 됩니다.
* 템플릿을 만들기 전에 프로젝트를 저장하면 쓰기 권한 오류가 반환됩니다.
* 파일 이름에 마침표가 두 개 포함된 경우 잘못된 프로젝트 저장
* 여러 개의 점(.)이 있는 파일 가져오기 파일 이름에 문제가 있음

### 2.6.1

(2017년 5월 12일 릴리스)

**추가됨 :**

* [TextureSet] 메시 재질을 Nothing으로 다시 할당하지 않음

**고정:**

* 베이킹된 맵을 교체한 후 TextureSet을 전환할 때 충돌 발생
* 레이어의 혼합 모드를 변경한 후 &quot;실행 취소 및 재실행&quot;을 수행할 때 충돌 발생
* big ID 맵에서 &quot;색상 선택&quot; 효과를 사용할 때 충돌 또는 멈춤
* [내보내기] 이름을 바꾼 텍스처 세트가 내보내기 창에서 알파벳순으로 정렬되지 않습니다
* [TextureSet] 기본 이름으로 재설정하면 단일성이 확인되지 않음
* [TextureSet] 프로젝트를 다시 연 후 이름이 바뀐 텍스처 세트가 비활성화됩니다.
* [Shelf] 기본 템플릿 콘텐츠가 누락됨
* [Shelf] 정사각형이 아닌 텍스처는 정사각형으로 표시됩니다
* [Shader] 텍스처 세트를 비활성화하면 연관된 셰이더가 제거됩니다.
* [스크립팅] alg.baking.setTextureSetBakingParameters()가 더 이상 작동하지 않음
* [스크립팅] 웹소켓 튜토리얼의 오타
* [스크립팅] AlgWidgets의 다양한 문제
* [Log] 경우에 따라 사용 가능한 가상 메모리가 잘못 검색됩니다.

### 2.6.0

(2017년 4월 27일 릴리스)

**추가됨** :

* 새 샘플 프로젝트 &quot;Meet Mat&quot; 추가
* [플러그인] 새로운 &quot;Resources Updater&quot; 플러그인
* [TextureSet] 텍스처 세트의 이름을 바꾸고 설명을 추가할 수 있습니다.
* [TextureSet] 재료 재할당 허용
* [TextureSet] 텍스처 세트 목록 창에 설정 버튼을 추가합니다.
* [TextureSet] 목록 맨 아래에 &quot;사용 안 함&quot; 텍스처 세트를 표시합니다.
* [Substance] 현재 텍스처 설정 해상도에서 추가 맵을 사용하여 성능을 향상시킵니다.
* [스크립팅] 프로젝트에 사용된 리소스(재료, 생성기 등)를 업데이트할 수 있습니다.
* [스크립팅] 선반을 추가/제거하는 방법 추가
* [스크립팅] 프로젝트의 리소스에서 정보를 쿼리할 수 있습니다.
* [스크립팅] 사용 가능한 셸 목록 검색 허용
* [스크립팅] AlgWidget 축소판 자습서 개선
* [내보내기] 파일 형식 지원을 기반으로 비트 심도 비활성화/활성화
* [Log] 콘솔에서 인쇄할 플러그인 이름 추가
* [Log] 숨겨진 텍스처 세트에 대한 오류 제거
* 샘플에 대한 새 아이콘 및 텍스트로 &quot;시작 화면&quot; 업데이트

**고정** :

* 특정 프로젝트에서 메시를 업데이트할 때 충돌 발생
* [뷰포트] 대칭 평면 내부 색상이 더 이상 표시되지 않습니다.
* [뷰포트] 단독 보기를 사용할 때 일부 후처리 효과가 활성화됨
* [음영] &quot;위\_premult&quot; 혼합이 제대로 작동하지 않음
* [Shaders] 기본 셰이더를 사용하는 알파 테스트에 대한 경고
* [Shelf] Substance의 태그 구문 분석이 잘못되었습니다.
* [Shelf] MatFX 녹 풍화 기능이 제대로 작동하지 않음
* [Shelf] 기본적으로 잘못된 채널에서 HSL 필터가 활성화됩니다
* [Shelf] 기본적으로 [Height/표준] 채널에서 선명 효과가 활성화됩니다
* [내보내기] Vray 내보내기 사전 설정이 OpenGL 표준 맵을 사용하지 않음
* [도구] 복제/손가락 도구의 부정확성 문제 가공물 만들기
