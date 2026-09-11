---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/pipeline-and-integration/configuration/environment-variables.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 환경 변수를 사용하여 응용 프로그램 동작 및 파이프라인 통합을 구성하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Environment variables
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 환경 변수
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 3%

---


# 환경 변수

이 페이지에는 애플리케이션의 기본 동작을 재정의하는 데 사용할 수 있는 환경 변수가 나열됩니다.

| 변수 | 설명 | 버전 |
| --- | --- | --- |
| **SUBSTANCE\_PAINTER\_라이선스** | 값: 라이선스 파일 자체에 대한 직접 경로입니다.라이센스 파일의 기본 위치를 재정의할 수 있습니다. 예 : 라이선스 파일이 **H:/allegorithmic/licenses/substance\_painter.key**&#x200B;에 있는 경우 변수 데이터는 **&quot;H:/allegorithmic/licenses/substance\_painter.key&quot;**&#x200B;이어야 합니다.  **참고:** 3.x(2017.x) 이전 버전에는 SUBSTANCE\_PAINTER\_2\_LICENSE을 대신 사용하십시오. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALLEGO\_LICENSE\_IDLE\_DELAY** | 값: 7200다중 사용자 구성의 경우 라이선스 시트를 릴리스하기 전에 시간을 초 단위로 지정합니다. 기본값은 2시간(7200s)입니다. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_SKIP\_CHECK\_FOR\_UPDATES** | 값 : 0 또는 1 (1 = 업데이트 확인 비활성화)응용 프로그램을 시작할 때 업데이트 확인을 건너뛸 수 있습니다. 새로운 기능 패널을 비활성화합니다. | <ol data-preserve-html="true"><li data-preserve-html="true">2.2</li></ol> |
| **SUBSTANCE\_PAINTER\_SVT\_HARDWARE\_ACCELERATION** | 값: 0 또는 1 (1 = 활성화됨)GPU에서 스파스 기능을 사용합니다. GPU 또는 운영 체제에서 지원되지 않는 경우 설정이 무시됩니다. 호환되는 하드웨어 구성의 경우 설명서를 참조하십시오. [스파스 가상 텍스처](../../features/sparse-virtual-textures.md)이 변수는 [설정](../../interface/settings/settings.md) 창에서 사용할 수 있는 매개 변수를 재정의합니다. | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_TEMP\_LOCATION** | 값: 폴더에 대한 직접 경로Substance Painter이 임시 파일(SVT 캐시 포함)을 쓸 위치를 정의합니다. 이 변수는 [설정](../../interface/settings/settings.md) 창에서 사용할 수 있는 매개 변수를 재정의합니다. | <ol data-preserve-html="true"><li data-preserve-html="true">3</li></ol> |
| **SUBSTANCE\_PAINTER\_PREVIEWS\_MEMORY\_BUDGET** | 값: 500자산 창에서 응용 프로그램이 임시 저장소 미리 보기를 로드하고 저장하는 데 사용할 수 있는 메모리(Ram)를 정의합니다. 예산 한도에 도달하면 이전 미리 보기가 언로드됩니다. 이 값은 에셋 창의 미리 보기 표시만 제어합니다.이 값은 MB로 정의됩니다. 기본값은 500MB입니다. | <ol data-preserve-html="true"><li data-preserve-html="true">2</li></ol> |
| **SUBSTANCE\_PAINTER\_PLUGINS\_PATH** | 추가 Python 플러그인의 위치 | 6.1 |
| **PYTHONPATH** | 애플리케이션의 Python 통합에 따라 로드할 추가 Python 모듈입니다. 자세한 내용은 [외부 Python 모듈 로드](https://helpx.adobe.com/kr/substance-3d/unlisted/documentation/spdoc/loading-external-python-modules-205363420.html)를 참조하세요. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **OCIO** | OpenColorIO에서 [색상 관리](../../features/color-management/color-management.md) 설정을 구동하는 데 사용되는 **config.ocio** 파일의 경로입니다.  **참고:** 이 환경 변수는 **PAINTER\_ACE\_CONFIG** 변수보다 우선 순위가 높습니다. | <ol data-preserve-html="true"><li data-preserve-html="true">4</li></ol> |
| **PAINTER\_ACE\_CONFIG** | Adobe ACE으로 [색상 관리](../../features/color-management/color-management.md) 설정을 구동하는 데 사용되는 json 파일의 경로입니다. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_DISABLE\_SPECIFIC\_FEATURES** | 애플리케이션 내에서 다음과 같은 여러 기능을 비활성화합니다.<ul data-preserve-html="true"><li data-preserve-html="true">외부 리소스 링크(도움말, 웹 페이지, 샘플 등)</li><li data-preserve-html="true">업데이트 확인 비활성화</li><li data-preserve-html="true">사용 현황 통계 전송 비활성화</li><li data-preserve-html="true">substance share으로 내보내기 사용 안 함</li><li data-preserve-html="true">시작 및 새로운 기능 패널 비활성화</li></ul> | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **ALG\_PAINTER\_DEBUG\_FPS** | 뷰포트에 의해 렌더링되는 초당 프레임 수에 대한 카운터를 뷰포트 내에 표시합니다. | <ol data-preserve-html="true"><li data-preserve-html="true">1</li></ol> |
| **SUBSTANCE\_PAINTER\_VRAM\_BUDGET** | Painter에서 사용할 수 있는 GPU 메모리 양을 지정합니다. 글로벌 예산을 MB 단위로 정의합니다. 예를 들어 4GB 제한을 정의하려면 4000 값을 사용합니다.명령줄 인수를 사용하여 동일한 작업을 수행할 수도 있습니다. [명령줄](command-lines.md)을 참조하십시오. | <ol data-preserve-html="true"><li data-preserve-html="true">2.1</li></ol> |
