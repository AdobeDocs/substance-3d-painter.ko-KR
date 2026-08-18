---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/scripting-and-development/api-reference/shader-api/changelog-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter 셰이더 API의 변경 로그를 검토하여 업데이트, 새로운 기능 및 시간 경과에 따른 변경 사항을 추적합니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Changelog - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 변경 로그 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 3%

---


# 변경 로그 - 셰이더 API

## 변경 로그

## 2018.3.2

* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md): 샘플링 함수에서는 단순 밉맵 레벨 대신 텍스처 파생 함수를 사용합니다. 비등방성 샘플링 지원을 위한 요구 사항입니다. 샘플링 함수 서명은 수정되지 않습니다.
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md): 텍스처 파생 효과를 사용하기 위해 *getParallaxOffset* 함수 시그니처가 변경되었습니다.

## 2018.3.0

* 비등방성 Specular 하이라이트를 시각화하는 데 도움이 되는 새 [lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md) 라이브러리를 추가합니다
* 밉맵 가용성을 고려하여 채널 샘플링을 지원하는 새 [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md) 라이브러리를 추가합니다.
* 이 안전한 샘플링을 처리하기 위해 셰이더 라이브러리 인터페이스를 업데이트합니다.
* **사용 중단**: vec2 텍스처 좌표 및 텍스처 샘플러에 기반한 이전 기능은 더 이상 사용되지 않습니다(새 서명 사용).
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md): *applyParallaxOffset* 함수를 추가하여 시차 오클루전 효과 사용을 단순화합니다.
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md): 파랑 노이즈 난수 값 생성기와 임시 대체를 추가합니다.
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md): 값 해석 및 샘플링 도우미를 모두 사용하도록 모든 채널 샘플링 도우미 분할

## 2018.2.0

* **표면 셰이더 API 변경**: *음영* 함수 시그니처가 변경되었습니다. [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md)을(를) 참조하십시오.
* *shadeShadow* 함수는 더 이상 사용되지 않으며 사용자 지정 표면 셰이더에서 안전하게 제거할 수 있습니다
* 하위 표면 분산 지원 추가는 자세한 내용은 [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md) 및 [lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md)을 참조하십시오
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md): *pbrComputeBRDF* 함수가 제거되었습니다. 지금 라이브러리를 사용하는 방법을 알아보려면 [pbr-metal-rough.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md) 예를 참조하십시오.
* 새 엔진 매개 변수가 추가되었습니다. *텍스처\_파랑\_노이즈*, *종횡비\_비율*, *camera\_vp\_matrix\_inverse*, *환경\_노출*, *환경\_회전*, *포비*, *메인\_조명* 및 *화면\_크기*. 자세한 내용은 [all-engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md)을 참조하세요
* 사용자 지정 셰이더 매개 변수에 대한 도구 설명을 제공하려면 *설명* 메타데이터를 추가합니다.

## 2017.4.2

* 문서 샘플에서 누락된 셰이더를 수정합니다(픽셀화된 셰더 및 툰 셰더).
* 고해상도를 위한 디더링 수정
  * [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md): **bayerMatrix8()** >4k에 대해 유효한 값을 반환합니다.

## 2017.4.1

* pbr 코팅 셰이더 수정
  * [lib-vector.glsl](libraries-shader-api/lib-vectors-shader-api.md): **tangentSpaceToWorldSpace()** 및 **worldSpaceToTangentSpace()** 출력이 이제 정규화되었습니다.

## 2017.4.0

* 특정 메시에 대한 2D 보기의 Specular 반사가 잘못됨

## 2017.3.1

* 디더링 비용

## 2017.2.0

* Substance Designer 및 베이커 동작에 맞게 보간된 tbn 정규화 제거
* [뷰포트] 해머슬리 테이블을 피보나치 나선으로 바꾸기

## 2.6.0

* 셰이더의 혼합 및 컬링 모드 수정
* 디더링을 재작업합니다. 이제 선형으로 렌더링을 구성한 경우 색상 프로필 뒤에 적용하겠습니다

## 2.5.0

* 뷰포트에 LUT(색상 프로파일)에 대한 지원 추가(sRGB 변환 옵션)
* 셰이더에서 불투명도에 디더링 추가
* PBR 셰이더에 시차 오클루전 매핑 추가
* 기본 셰이더 UI에서 사용자 정의 매개 변수를 숨기는 방법 추가
* 레이어 셰이더 설명서에서 채널 태그 목록에 링크 추가
* &#39;channel\_ao&#39; 태그를 &#39;channel\_ambientocclusion&#39;으로 바꿉니다.
* [뷰포트] 일부 표준 맵에는 가공물로 나타나는 고정된 값이 있습니다
* 셰이더스 문서에서 사용 가능한 채널 수정
* 사용자 지정 셰이더 UI 정의 허용
* 재질 레이어 셰이더에 표준 사용자 정의 셰이더 UI 추가
* 이제 사용자 정의 UI 파일이 (mdl과 같은) 셸프의 셰더/사용자 정의 UI 폴더에 대해 상대적으로 검색됩니다.
* 기본 셰이더에서 Specular level 채널 사용
* Vec3 셰이더 매개 변수 예제 수정
* Painter을 OpenGL 코어 프로필로 업그레이드

## 2.4.0

* 내보낸 맵과 뷰포트에 표시된 맵을 결합한 표준 맵의 차이를 수정합니다

## 2.2.0

* 비문서 텍스처의 일반 재질에 비결합 텍스처에 대한 지원 추가
* 사용자 정의 셰이더 슬라이더 설명서 업데이트
* 슬라이더의 단계 정밀도 정의 허용
* 동적 재질 레이어 설명서

## 2.1.1

* lib-utils에 &#39;RGB2Gray&#39; 함수 추가

## 2.1.0

* 셰이더 매개 변수 및 재질/마스크에 대한 그룹 정의 허용
* 설명서에 누락된 채널 추가(&#39;ao&#39;, &#39;diffuse&#39;, &#39;specularlevel&#39;)

## 2.0.4

* 알파 값이 낮은 일반 풀기 함수가 올바르지 않음
* 사용자 지정 셰이더에서 메시 꼭지점 색상을 읽을 수 있도록 허용
* [뷰포트] 일부 컴퓨터에서 확장된 환경 맵

## 2.0.0

* 전용 채널별로 일반/AO 추가 맵을 재정의하도록 허용
* Sobel 메서드를 사용하도록 Height2Normal 함수 변경
* 셰이더당 mdl 정의 가능성 추가
* 선반에 새 mdl 폴더 추가
* 확산 및 Specular level 채널 사전 설정 추가
* 톤 매핑에 대한 설명서 업데이트
* 직교 모드에서 반사 수정
* 엔브맵의 특정 위치에 나타나는 흰색 수직 결함을 수정했습니다.
* 텍스처 매개 변수에 대해 &#39;default\_color&#39;를 정의할 수 있습니다.

## 1.7.0

* 외부 텍스처(선반에서) 샘플링 가능

## 1.6.0

* 감마/톤 매핑 함수를 표시하여 재정의할 수 있습니다.
* 여러 텍스트 표시

## 1.5.0

* 셰이더 오류 보고서에 줄 번호 및 파일 이름 추가

## 1.4.1

* sRGB 변환은 모두 sRGB 표준을 따릅니다. 단, 근사치가 가까운 셰이더에서 변환이 수행됩니다
* Height 채널을 표준 맵으로 변환하면 잘못된 색상 공간으로 변환됩니다

## 1.4.0

* 앰비언트 오클루전 채널 추가
* 일반 버전에 새 워크플로우 추가
* 텍스처 관련 자동 매개 변수에 대한 &#39;or&#39; 식 구문 추가
* OSX에서 Intel gpu용 pbr 셰이더 수정

## 1.3.4

* 조각 셰이더에서 이항 보간 허용
* 믹트 탄젠트 공간 수정

## 1.3.3

* 네거티브 라이트 강도를 생성하는 구형 조화 수정
* 노출 계산은 Substance Designer(및 노출 슬라이더 수정)와 다릅니다.
* 그림자는 100% 금속 표면에 표시되지 않아야 합니다

## 1.3.0

* 그림자 기능 추가
* 불투명도 지원 추가(&#39;alpha\_test&#39; 및 &#39;alpha\_blend&#39;)

## 1.2.0

* 필요한 openGL 상태를 사용자 정의 셰이더로 설정하는 기능
* 반전된 비트각 수정
* 일반 채널에 대한 지원 추가

## 1.0

* 사용자 정의 셰이더에 대한 지원 추가
