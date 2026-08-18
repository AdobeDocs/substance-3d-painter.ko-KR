---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/pipeline-and-integration/resource-management/adding-saved-searches-manually.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 저장된 검색을 수동으로 추가하여 자주 사용하는 리소스 필터에 빠르게 액세스하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding saved searches manually
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 수동으로 저장된 검색 추가
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 2%

---


# 수동으로 저장된 검색 추가

구성 파일을 편집하여 에셋 검색 쿼리(또는 저장된 검색)를 정의할 수 있습니다. 이 페이지에서는 방법을 설명합니다.

## 구성 파일의 위치

사용자 지정 저장 쿼리를 추가하려면 [사용자 문서] 폴더로 이동하여 **Shelf.ini** 파일을 엽니다.

<table data-preserve-html="true" style="width: 100.0%;"> <colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup> <tbody> <tr> <th>플랫폼</th> <th>버전</th> <th>경로</th> </tr> <tr> <td rowspan="2"><strong>Windows</strong></td> <td><strong>7.2</strong> 이상</td> <td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">레거시</td> <td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Mac</strong></td> <td colspan="1"><strong>7.2</strong> 이상</td> <td colspan="1">/Users/사용자 이름/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">레거시</td> <td colspan="1">/Users/사용자 이름/Documents/Allegorithmic/Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>리눅스</strong></td> <td colspan="1"><strong>7.2</strong> 이상</td> <td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td>레거시</td> <td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td> </tr> </tbody> </table>

## 예

다음은 구성 파일에 넣을 수 있는 콘텐츠의 예입니다.

```
[filters] 

size=4 

1name=Grunge 

1query="u:basematerial=,smartmaterial=,smartmask=,texture=,procedural=,brush=,alpha= grunge" 

2name=Procedural 

2query="u:procedural=" 

3name=Environment 

3query="u:environment=" 

4name=Default Filters 

4query="p:/allegorithmic/^ u:filters="
```


다음은 구문 작동 방식입니다.

* **크기**: 응용 프로그램에서 읽고 로드해야 하는 사용자 지정 사전 설정 수를 결정합니다.
* **숫자**: 줄 시작 부분에서 현재 사전 설정을 정의합니다(예: **1/**).
* **쿼리**: (숫자 뒤)는 사용되는 실제 검색어를 정의합니다. 이 예제에서는 사용에 **u:**, 경로에 **p:** 또는 검색어에 문자열을 사용합니다. 쿼리 콘텐츠는 따옴표로 묶어야 합니다. 사용할 수 있는 용어에 대해 알아보려면 [이 페이지를 확인하세요](../../interface/assets/advanced-search-queries.md).
* **이름**: 사전 설정의 이름입니다.
