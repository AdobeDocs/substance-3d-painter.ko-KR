---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/technical-support/project-resources.html"
breadcrumb-title: ''
description: Substance 3D Painter의 프로젝트 리소스 및 기술 문서에 액세스하여 워크플로우와 문제 해결을 개선합니다.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 프로젝트 리소스
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# 프로젝트 리소스 및 설정

프로젝트 리소스를 관리하면 Painter에서 프로젝트 성능에 좋은 기반을 마련할 수 있습니다.

+++축소 베이킹된 맵
일부 베이킹된 맵이 2k 또는 4k 해상도가 아니어도 됩니다. 배치를 2k에서 굽는 것을 망설이지 말고 더 낮은 해상도에서 다시 굽아서 시각적 차이가 있는지 확인하십시오.

+++

+++가져온 비트맵 관리
가져온 이미지는 성능에 큰 영향을 줄 수 있으므로 가져온 이미지에 주의해야 합니다. 텍스처 세트가 2k로 설정되어 있고 더 높은 해상도로 내보내지지 않는 경우 8k 이미지를 사용해도 긍정적인 영향을 주지 않으며, 텍스처 세트의 해상도이므로 품질이 2k로 제한됩니다.

포맷도 중요합니다. EXR, HDR 및 PNG도 JPG보다 훨씬 무겁고, 일부 이미지에는 EXR의 품질 수준(예: 기본 색상 대 Height 세부 정보)이 필요하지 않을 수 있습니다.

+++

+++셰이더 설정 조정
Ultra으로 Specular 품질을 사용하면 더 정확한 결과를 얻을 수 있지만, 설정은 비용이 많이 듭니다. 셰이더에서 한 번에 많은 효과를 활성화할수록 계산이 더 많이 수행됩니다. 가능한 경우 별도의 셰이더를 사용하여 복합 재질을 다른 텍스처 집합으로 분할합니다. 변위 가 활성화된 경우 쪽맞춤 매개변수에 주의해야 합니다.

+++

+++파일 옵션 조정
<b>파일 > 저장 > 파일 저장 및 축소</b> 사용 <b>불필요한 데이터를 플러시하려면 </b>크기를 조정하고, <b>사용하지 않는 리소스 제거</b>를 사용하여 프로젝트 내 어디에서도 사용되지 않는 프로젝트로 가져온 파일을 제거합니다.

+++
