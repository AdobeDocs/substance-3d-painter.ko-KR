---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/technical-support/workflow-issues/project-issues/a-project-has-been-processed-as-a-text-file-and-is-now-corrupted.html"
breadcrumb-title: ''
description: 텍스트 파일로 처리된 손상된 Substance 3D Painter 프로젝트 파일을 복구하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Workflow Issues > Project Issues > Corrupted project file
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 프로젝트 파일 손상됨
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---


# 프로젝트가 텍스트 파일로 처리되어 현재 손상되었습니다.

프로젝트를 로드할 때 다음 오류가 표시될 수 있습니다.

```
[Hdf5Archive] Archive 'project.spp' appears to have been processed as a text file and is irremediably corrupted. 

[Project management] The selected project 'project.spp' isn't valid!
```


이 오류는 프로젝트가 Substance 3D Painter 외부에서 수정되었으며 **제대로 다시 읽을 수 없음** 을 의미합니다.\
일반적으로 이 문제는 **Perforce** 같은 버전 관리 소프트웨어가 Substance 3D Painter 프로젝트 **을(를) 이진 파일** 대신 텍스트 파일로 처리할 때 발생합니다. 유일한 해결 방법은 새 규칙/예외를 버전 관리 소프트웨어에 추가하여 **spp 파일을 이진 파일** 로 강제로 처리하는 것입니다. **Perforce**&#x200B;에 대한 자세한 내용은 전용 설명서 <https://www.perforce.com/perforce/r16.1/manuals/cmdref/p4_typemap.html>을(를) 참조하십시오.
