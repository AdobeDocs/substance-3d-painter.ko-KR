---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/installation-and-preferences/automated-installation.html"
breadcrumb-title: ''
description: 기업 배포 및 파이프라인 통합 워크플로를 위해 Substance 3D Painter 설치를 자동화하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Installation and preferences > Automated installation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 자동 설치
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---


# 자동 설치

Substance 3D 독립 실행형 설치 관리자를 사용하는 경우 애플리케이션을 자동 모드로 설치하여 보다 쉽게 배포할 수 있습니다.

**InnoSetup**&#x200B;을(를) 사용하여 설치 관리자를 생성하는 중입니다. 설치 관리자에 사용할 수 있는 전체 매개 변수 집합은 [여기서 사용 가능](http://www.jrsoftware.org/ishelp/index.php?topic=setupcmdline)입니다.

## 명령줄을 통해 자동 모드로 설치

자동 설치를 수행하는 데 사용할 플래그는 **/SILENT**&#x200B;입니다. **/NCRC** 플래그는 프로세스 속도를 높이기 위해 패키지의 CRC(확인)를 건너뛰는 데도 사용할 수 있습니다.

예:

```
SubstancePainter_Installer.exe /NCRC /SILENT /DIR="C:InstallationFolder"
```


>[!NOTE]
>
> 설치 경로는 별도의 폴더에 단일 백슬래시 문자를 사용해야 합니다. 그렇지 않으면 설치 관리자가 경로를 인식하지 못합니다.
