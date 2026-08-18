---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/interface/assets/advanced-search-queries.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 고급 검색 쿼리를 만들어 복잡한 검색 조건을 사용하여 특정 에셋을 찾는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Interface > Assets > Advanced search queries
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 고급 검색 쿼리
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# 고급 검색 쿼리

고급 검색 쿼리를 사용하면 복합 검색을 구성하여 [저장된 검색](saved-searches.md)으로 다시 사용할 수 있습니다.

고급 쿼리는 검색 막대에서 사용할 수 있으며 다음을 포함할 수 있습니다.

1. **경로**: 폴더/폴더 구조로 검색 결과를 구체화할 수 있습니다.
1. **사용량** : 응용 프로그램에서 사용 가능한 사용량을 모두 나열합니다.
1. **텍스트 쿼리** : 다른 유형의 쿼리를 자유롭게 추가할 수 있도록 허용합니다(사용자 지정 키워드 등).

새 검색 쿼리를 정의할 때 여러 항목을 선택할 수 있습니다.

## 경로

경로 쿼리를 사용하면 경로를 기반으로 쿼리를 구체화할 수 있습니다. **경로별 필터** 패널에 사용 가능한 모든 라이브러리가 나열됩니다(편집 > 설정 > 라이브러리를 통해 직접 추가할 수 있음).\
경로 정의를 사용하여 사용자 정의 라이브러리 경로 또는 계층 구조의 특정 하위 폴더별로 필터링할 수 있습니다.

## 사용

사용량 은 리소스의 정의와 Substance 3D Painter에서 리소스를 사용하는 방법을 정의합니다. 일부는 리소스의 파일 유형에 의해 정의될 수 있습니다.\
예-

* **pbr.glsl**: 셰이더 파일 - 셰이더로만 사용할 수 있고 그 외에는 사용할 수 없습니다.
* **effect.sbsar**: Substance 파일 - 생성기, 필터 또는 재질일 수 있으므로 원래 그래프(Designer의 경우)에 용도가 설정되어 있지 않으면 가져올 때 Painter의 사용자가 이를 표시해야 합니다.

## 텍스트

텍스트 쿼리는 여러 유형의 필터링을 지원하며, 일부는 일반 인터페이스보다 더 향상되었습니다.\
올바른 키워드를 입력하여 활성화할 수 있습니다.

* **사용 가능한 검색 유형** :
  * &quot; **n:** &quot; : 이름
  * &quot; **s:** &quot; : shelf/library(&quot;session&quot; 및 &quot;project&quot; 포함)
  * &quot; **p:** &quot; : 경로
  * &quot; **u:** &quot; : 사용
* **이스케이프** : 이스케이프 처리해야 하는 문자 앞에 &quot; **\** &quot;을(를) 사용하거나 따옴표를 대신 사용할 수 있습니다. 예:
  * **a\ 이름\(공백 포함)**
  * **&quot;공백이 있는 이름&quot;**
* **특정 특성(또는 그룹)** : 특정 특성을 검색하려면 형식 지정자로 &#39;또는 그룹&#39;을 앞에 추가합니다. 예 :
  * **n:a,b,c,d** : 이름은 a 또는 b 또는 c 또는 d입니다.
* **검색 동작** :
  * 특정 사용을 필터링하려면 특정 **키워드**&#x200B;을(를) 검색에 추가합니다. 예: &quot; **이미지** 앰비언트&quot;
  * 여러 요청을 추가하려면 쉼표 &quot; **,** &quot;을(를) 사용하십시오(예: &quot;cobalt **,** gold&quot;(쉼표를 사용하는 경우, 검색에는 두 키워드와 동시에 일치하는 리소스만 표시됨).
  * 정확한 이름을 검색하려면 느낌표 &quot;!&quot;를 사용하십시오. 끝의 예: **di!**  (이 키워드는 **Dirt**&#x200B;을(를) 반환하지만 **drips**&#x200B;은(는) 반환하지 않습니다. 이 키워드는 유사 항목 일치를 사용하지 않도록 설정합니다.)
  * 검색에서 패턴을 제외하려면 하이픈 &quot; **-**&quot;을(를) 사용하십시오(예: **u:image n:-normal**, &quot;normal&quot;이 포함되지 않은 이미지를 반환함)
* **일치하는 함수(패턴 접미사) :**
  * **기본값** : 대략적인 일치(유사 항목)
  * **포함** : !
  * **regex** : #
  * **같음** : =
  * **다음으로 시작** : ^
  * **다음으로 종료** : &amp;
