---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/features/post-processing/glare.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 눈부심 후처리 효과를 사용하여 밝은 영역에 렌즈 플레어 및 블룸 효과를 추가하는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Features > Post Processing > Glare
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 눈부심
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# 눈부심

![](../../assets/glare-example.jpg)![](../../assets/glare.png)

매개 변수에 대한 설명 :

| 설정 | 설명 |
| --- | --- |
| **광도** | 이는 눈부심 효과의 전체 밝기입니다. 이 값을 0.0으로 설정하면 효과가 완전히 비활성화됩니다.  실제 값은 최대 약 16.0까지 약 0.5 ~ 4.0의 범위에서 발생합니다. |
| **임계값** | 임계값보다 밝은 픽셀만 추출하여 눈부심을 생성합니다.  자연스러워 보이는 결과의 경우 0.0에서 1.0 사이의 값이 권장됩니다. |
| **다시 매핑** **요소** | 1.0 이외의 값을 지정하면 추출된 고휘도 성분이 더 비선형적으로 확장(또는 압축)됩니다. 1.0보다 높은 값을 전달하면 밝은 픽셀의 눈부심이 더 강해집니다.  다른 효과에 영향을 주지 않고 분리된 상태에서 눈부심의 광도 매핑을 조정하려면 이 옵션을 사용합니다. 밝은 패스 이후의 광도는 부드러운 곡선에서 증가하며, 광도 값 1.0은 **다시 매핑 요소**&#x200B;에 접근하고, 1.0보다 큰 값은 접근합니다(**다시 매핑** **요소** ^2). |
| **모양** | 모양은 눈부심의 모양을 정의하며 다양한 모델을 사용할 수 있습니다 .<ul data-preserve-html="true"><li data-preserve-html="true"><strong>개화</strong> : 개화 효과만 있습니다.</li><li data-preserve-html="true"><strong>렌즈 플레어:</strong> 흐림/고스트(렌즈 플레어)/잔상.</li><li data-preserve-html="true"><strong>표준:</strong> 모든 기본 요소의 균형이 잘 잡힌 형식입니다.</li><li data-preserve-html="true"><strong>저렴한 렌즈:</strong> 날카로운 고스팅과 저렴한 렌즈의 다른 표현. </li><li data-preserve-html="true"><strong>후 이미지:</strong> 잔상이 매우 강한 문자를 입력합니다. </li><li data-preserve-html="true"><strong>필터 크로스 스크린:</strong> 크로스 모양의 별 필터 생성기가 연결된 렌즈.</li><li data-preserve-html="true"><strong>필터 크로스 스크린 스펙트럼</strong>: 강한 스펙트럼이 부착된 크로스 모양의 별 필터 생성기가 있는 렌즈.</li><li data-preserve-html="true"><strong>필터 Snow 십자</strong> : 6방향 별 필터 생성기가 연결된 렌즈입니다.</li><li data-preserve-html="true"><strong>필터 Snow 크로스 스펙트럼</strong> : 6개 방향의 강한 스펙트럼을 가진 별 필터 생성기가 부착된 렌즈.</li><li data-preserve-html="true"><strong>Filter Sunny Cross</strong> : 8방향 별 필터 생성기가 있는 렌즈</li><li data-preserve-html="true"><strong>필터 Sunny Cross Spectrum</strong> : 8개 방향의 강한 스펙트럼을 가진 별 필터 생성기가 있는 렌즈.</li><li data-preserve-html="true"><strong>수평 줄무늬</strong> : 이 렌즈 플레어 유형은 강한 수평 별 줄무늬를 생성합니다.</li><li data-preserve-html="true"><strong>세로 줄무늬</strong> : 세로 방향으로 별줄이 강하게 나타나는 문자입니다. CCD 디지털 카메라 등에 대한 얼룩.</li></ul> |

## 모양 예

![](../../assets/bloom-examples-bloom.jpg)![](../../assets/bloom-examples-standard.jpg)![](../../assets/bloom-examples-cross.jpg)![](../../assets/bloom-examples-snow.jpg)![](../../assets/bloom-examples-sunny.jpg)![](../../assets/bloom-examples-streak.jpg)
