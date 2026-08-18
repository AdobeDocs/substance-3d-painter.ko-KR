---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/shelf-issues/font-import.html"
breadcrumb-title: ''
description: 글꼴 리소스를 성공적으로 가져오고 사용하기 위해 Substance 3D Painter에서 글꼴 파일 가져오기 문제를 해결하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 글꼴 파일을 가져올 수 없음
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# 글꼴 파일을 가져올 수 없음

[텍스트 리소스](../../../painting/text-resource.md)가 도입되면 시작 시 글꼴 파일이 자동으로 수집됩니다. 글꼴 파일을 수동으로 가져올 수도 있습니다.

이러한 경우 몇 가지 오류 메시지가 나타날 수 있습니다.

* Painter 인터페이스로 파일을 드래그 앤 드롭하는 경우.
* Painter이 디스크에서 글꼴을 검색하는 경우(라이브러리 크롤링).

## 문제 해결 방법

<b>손상된 파일</b>에 대한 오류 메시지가 나타나면 대체 버전을 찾아 Painter에서 로드할 수 있습니다. <b>.ttf</b> 및 <b>.otf</b> 형식만 지원됩니다.

<b>라이선싱 문제</b>에 대한 오류 메시지가 발생하면 해당 글꼴은 Painter과 호환되지 않아 가져올 수 없습니다.

### 메시지 개요

|  |  |
| --- | --- |
| <b>오류 메시지</b> | <b>설명</b> |
| &quot;LIBRARYNAME&quot; 라이브러리에 FONTNAME, FONTNAME, FONTNAME,...의 4개 글꼴 파일에 영향을 미치는 문제가 있습니다. | 이 메시지는 Painter 내에서 가져올 수 없는 확인된 글꼴 파일 이름의 짧은 목록을 수집합니다. 이러한 파일은 무시되며 에셋 창에 표시되지 않습니다. |
| 글꼴 문제가 발견되었습니다. 자세한 내용은 https://...를 참조하십시오. | 글꼴에서 문제를 발견했음을 나타내는 일반 메시지입니다. |
| 라이선싱 제한으로 인해 FONTNAME을 가져올 수 없습니다. 자세한 내용은 https://...를 참조하십시오. | Painter은 글꼴을 사용하려면 해당 프로젝트 파일에 글꼴을 포함할 수 있어야 합니다. 허용하지 않는 글꼴(메타데이터에 지정됨)은 가져올 수 없습니다. |
| 파일이 손상되었거나 지원되지 않는 유형이므로 FONTNAME을 가져올 수 없습니다. 자세한 내용은 https://...를 참조하십시오. | Painter에서 제공된 글꼴 파일을 읽을 수 없습니다. |
