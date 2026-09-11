---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/resource-management/preferences-and-content-migration.html"
breadcrumb-title: ''
description: 업그레이드하거나 새 시스템으로 이동할 때 Substance 3D Painter의 환경 설정 및 콘텐츠를 마이그레이션하는 방법에 대해 알아보십시오.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Preferences and content migration
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 환경 설정 및 콘텐츠 마이그레이션
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---


# 환경 설정 및 콘텐츠 마이그레이션

이 페이지에서는 환경 설정 및 Shelf/Assets에서 데이터를 마이그레이션하여 새 버전에 사용하는 방법에 대해 설명합니다.

버전 7.2 릴리스 후에는 애플리케이션의 여러 버전(Substance 3D 독립 실행형, Steam 및 Creative Cloud 데스크탑)에서 공통으로 사용할 수 있도록 환경 설정 및 셸프 위치가 변경되었습니다. 이 변경으로 인해 이제 이전 환경 설정 및 사용자 지정 리소스 **이(가) 기본적으로 무시됨**&#x200B;이(가) 됩니다(**손실되지 않음**). **Shelf**&#x200B;의 이름이 **에셋**(으)로 바뀌었으므로 마이그레이션에 아래에 설명된 몇 가지 단계가 포함됩니다.

## 재고 및 자산 자원 마이그레이션

기본 사용자의 리소스 위치가 변경되어 이제 Documents 폴더에 저장된 모든 콘텐츠가 새 버전의 애플리케이션에서 무시됩니다. 이 내용을 복원하려면 파일을 한 위치에서 다른 위치로 이동하기만 하면 됩니다.

### 콘텐츠를 찾을 수 있는 장소

쉘프 또는 에셋 경로는 다음 위치에서 찾을 수 있습니다.

<table data-preserve-html="true" style="width: 100.0%;"><colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup><tbody><tr><th>플랫폼</th><th>버전</th><th>경로</th></tr><tr><td rowspan="2"><strong>Windows</strong></td><td><strong>7.2</strong> 이상</td><td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td></tr><tr><td colspan="1">레거시</td><td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td></tr><tr><td rowspan="2"><strong>Mac</strong></td><td colspan="1"><strong>7.2</strong> 이상</td><td colspan="1">/Users/사용자 이름/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td colspan="1">레거시</td><td colspan="1">/Users/사용자 이름/Documents/Allegorithmic/Substance Painter</td></tr><tr><td rowspan="2"><strong>리눅스</strong></td><td colspan="1"><strong>7.2</strong> 이상</td><td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td></tr><tr><td>레거시</td><td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td></tr></tbody></table>

### Shelf 콘텐츠를 마이그레이션하는 방법

이전 Shelf 콘텐츠는 디스크에 있는 파일이므로 마이그레이션하는 것은 이러한 파일을 적절한 위치에 배치하는 것입니다.

1. 애플리케이션 닫기
1. 이전 Shelf 폴더로 이동
1. 하위 폴더(알파, 절차, 자료 등) 복사 또는 잘라내기
1. 새 에셋 폴더로 이동
1. 이전에 복사한 하위 폴더를 Assets 폴더 내에 붙여넣으십시오. 붙여넣으라는 메시지가 표시되면 덮어씁니다.

이제 애플리케이션을 다시 시작하고 에셋 창에 콘텐츠가 표시됩니다.

>[!NOTE]
>
> 리소스의 상위 폴더뿐만 아니라 하위 폴더도 복사해야 합니다. 상위 폴더의 이름이 **shelf**&#x200B;에서 **에셋**(으)로 바뀌었으므로 상위 폴더만 복사하면 응용 프로그램에 리소스가 표시되지 않습니다.

### 선반 사전 설정을 마이그레이션하는 방법

셸프 사전 설정은 구성 파일 내에 저장됩니다. 이러한 사전 설정을 마이그레이션하려면:

1. 애플리케이션 닫기
1. 이전 Shelf 폴더로 이동
1. Shelf.ini 파일 복사 또는 잘라내기
1. 새 에셋 폴더로 이동
1. 파일을 붙여넣고 기존 파일을 덮어씁니다.

이제 애플리케이션을 다시 시작하면 저장된 검색이 전용 섹션 또는 에셋 창에 표시됩니다.

## 환경 설정 마이그레이션

인터페이스에서 애플리케이션 설정을 수동으로 다시 조정하는 것이 좋습니다. 이는 호환성 문제를 야기하지 않고 정보를 마이그레이션하는 가장 안전한 방법입니다.

그렇지 않으면 다음 페이지를 확인하여 환경 설정의 위치를 알아보십시오. [환경 설정 및 응용 프로그램 데이터 위치](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/application-preferences-location-147095594.html).
