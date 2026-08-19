---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/pipeline-and-integration/resource-management/excluding-resources-in-a-resource-path.html"
breadcrumb-title: ''
description: 더욱 개선된 셸프 구성을 위해 Substance 3D Painter에서 리소스 경로에서 특정 리소스를 제외하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Excluding resources in a resource path
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 리소스 경로에서 리소스 제외
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---


# 리소스 경로에서 리소스 제외

이 페이지에서는 [에셋](../../interface/assets/assets.md) 창의 크롤링 프로세스 중에 무시되는 리소스와 폴더를 지정하도록 무시 파일을 설정하는 방법에 대해 설명합니다. 원치 않는 리소스가 표시되지 않도록 할 수 있습니다.

>[!NOTE]
>
> 이 기능은 버전 7.2.3부터 사용할 수 있습니다.

## 무시 파일 만들기

자원을 숨길 자원 폴더의 위치로 이동합니다. 그런 다음 다음과 같이 이름이 지정된 파일을 만듭니다.

```
.ignore_assets_pt
```


>[!NOTE]
>
> 파일 이름은 점으로 시작해야 합니다.

만든 모양은 다음과 같아야 합니다.

![](../../assets/ignore-file-location.png)

## 예

다음 파일 콘텐츠는 기본 라이브러리 폴더가 아닌 모든 리소스 및 폴더를 버립니다.

```
## exclude all

* 

 

## re-include library directories

!alphas 

!colorluts 

!effects 

!emitters 

!environments 

!export-presets 

!generators 

!materials 

!presets 

!procedurals 

!receivers 

!shaders 

!smart-masks 

!smart-materials 

!templates 

!textures
```


## 규칙 및 지침

다음 표에서는 무시 파일에 적용되는 일반 규칙을 보여 줍니다.

>[!NOTE]
>
> 무시 파일의 패턴 일치는 운영 체제 동작과 관계없이 대/소문자를 구분합니다.

| 규칙 | 설명 | 예 |
| --- | --- | --- |
| **빈 줄** | 일치하지 않는 빈 줄입니다. 가독성을 위한 구분 기호로 사용할 수 있습니다. |  |
| **디렉터리 구분 기호** | 슬래시는 디렉터리 구분 기호로 사용됩니다. 구분 기호는 검색 패턴의 시작, 중간 또는 끝에 나타날 수 있습니다.패턴의 시작 또는 중간(또는 둘 다)에 구분 기호가 있는 경우 패턴은 무시 파일 자체의 디렉토리 레벨을 기준으로 합니다. 그렇지 않으면 패턴이 무시 파일 레벨 아래의 모든 레벨에서도 일치할 수 있습니다. 패턴 끝에 구분 기호가 있는 경우 무시됩니다. 패턴은 파일과 디렉토리 둘 다와 일치합니다. | `folder/filename.extension   folder/sub-folder` |
| **주석 줄** | 숫자 기호(또는 해시)로 시작하는 줄은 주석 역할을 합니다. | `# This is a comment` |
| **별표** | 별표는 슬래시를 제외한 모든 항목과 일치합니다. | `# Match anything starting with Alpha   alpha*   # Match any file with given extension   *.jpg` |
| **문자 범위** | 폴더 및 파일 이름과 일치하도록 대괄호 사이에 문자 범위를 지정할 수 있습니다.<ul data-preserve-html="true"> <li data-preserve-html="true"><b>[abc]</b>: 지정된 목록의 문자 하나와 일치</li> <li data-preserve-html="true"><b>[a-c]</b>: 지정된 범위에서 한 문자와 일치합니다.</li> <li data-preserve-html="true"><b>[ !abc]</b>: 지정된 목록에 없는 하나의 문자와 일치</li> <li data-preserve-html="true"><b>[ !a-c]</b>: 지정된 범위에 없는 문자 하나와 일치</li> </ul>범위 및 목록은 <b>[0-9]</b> 형식의 숫자일 수도 있습니다. | `# Exclude any UDIM image in PNG   *_[0-9][0-9][0-9][0-9].png` |
| **이스케이프 문자** | 그렇지 않으면 무시되거나 규칙으로 사용되는 리터럴 문자를 나타냅니다. | `# This is a comment   [#]This/Is/A/Path` |
| **후행 공백** | 후행 공백은 이스케이프되지 않는 한 무시됩니다. | `# Match a subfolder with trailing space   folder/subfolder[ ]` |
| **느낌표 접두사** | 느낌표를 사용하여 패턴을 미리 수정하면 패턴을 부정할 수 있습니다.이전 패턴으로 제외된 일치하는 파일이 다시 포함됩니다. 해당 파일의 상위 디렉터리가 제외된 경우 파일을 다시 포함할 수 없습니다. 크롤링은 성능 상의 이유로 제외된 디렉터리를 나열하지 않으므로 포함된 파일의 패턴은 정의된 위치에 관계없이 영향을 주지 않습니다. | `# Re-include specific file   !my_file_name.png` |
