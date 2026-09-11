---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/scripting-and-development/api-reference/shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter의 셰이더 API 참조에 액세스하여 사용자 정의 셰이더를 만들고 렌더링 기능을 확장합니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---


# 셰이더 API

![](../../../assets/header-shader.jpg)

Substance Painter은 셰이더를 사용하여 실시간 뷰포트에서 재질을 렌더링합니다. 사용자 정의 셰이더를 작성하여 새 비헤이비어를 구현하거나 뷰포트를 다른 렌더러와 일치시킬 수 있습니다.

[Substance share](https://share.allegorithmic.com/libraries?by_category_type_id=6)에서 Substance Painter에 대한 추가 셰이더를 찾을 수 있습니다.

>[!NOTE]
>
> 셰이더 API은 **도움말 > 문서 > 셰이더 API** 메뉴로 이동하여 응용 프로그램에서 직접 사용할 수도 있습니다.

## 셰이더 참조

## 변경 로그

* [전체 변경 로그 파일](changelog-shader-api.md)

## 준비

Substance Painter에서 *GLSL*&#x200B;에 자신만의 셰이더를 쓸 수 있습니다. 조각 셰이더의 *부분*&#x200B;만 쓸 수 있습니다. 이 셰이더를 *표면 셰이더*&#x200B;라고도 합니다. 더 이상 걱정하지 말고 &quot;Hello world&quot; Substance Painter 표면 셰이더를 소개하겠습니다.

```
void shade(V2F inputs) { 

  diffuseShadingOutput(vec3(1.0, 0.0, 1.0)); 

}
```


이제 이 스니펫을 *.glsl* 파일에 저장하고 셸프의 셰이더 탭에 드롭하여 Substance Painter에 로드하면 이제 이 스니펫을 사용하고 메쉬에서 아름답고 균일한 분홍색을 볼 수 있습니다.

## 표면 셰이더

* [surface-shader.glsl](shaders-shader-api/surface-shader-shader-api.md)

## 엔진이 제공한 데이터(또는 내 채널에 액세스하는 방법)

Substance Painter에서 렌더링 엔진 매개 변수(문서의 텍스처, 추가 채널, 카메라 관련 데이터 등)에 액세스할 수 있습니다. 다음은 모든 엔진 제공 매개 변수의 전체 목록입니다.

* [all-engine-params.glsl](parameters-shader-api/all-engine-params-shader-api.md)

## 엔진 설정(또는 렌더링 상태를 지정하는 방법)

효과에 특정 렌더링 구성(컬링, 혼합, 샘플링 로크리티 등)을 사용하고자 하는 경우도 있습니다. 일부 렌더링 상태가 노출되며 셰이더에서 설정할 수 있습니다. 다음은 노출된 모든 렌더링 상태의 전체 목록입니다.

* [all-rendering-states-params.glsl](parameters-shader-api/all-rendering-states-params-shader-api.md)

## 사용자 정의 수정(또는 셰이더를 어떻게 수정합니까?)

셰이더에 사용자 정의 변경 사항이 있는 것이 일반적입니다. Substance Painter의 셰이더에서 이를 위해 사용자 정의 변경 사항을 지정하는 방법을 도입했습니다. 다음은 모든 사용자 정의 셰이더 tweaks 유형의 전체 목록입니다.

* [all-custom-params.glsl](parameters-shader-api/all-custom-params-shader-api.md)

## 포함된 라이브러리

모든 셰이더에서 비대화형 코드를 많이 작성하지 않기 위해, 작지만 실용적인 유용한 기능 라이브러리를 만들었습니다. **지금은 편집하거나 직접 만들 수 없습니다.**

* [lib-alpha.glsl](libraries-shader-api/lib-alpha-shader-api.md) : 불투명도 관련 도우미를 포함합니다.
* [lib-bayer.glsl](libraries-shader-api/lib-bayer-shader-api.md) : bayer 행렬 도우미 포함
* [lib-defines.glsl](libraries-shader-api/lib-defines-shader-api.md) : 유용한 수학 상수를 포함합니다.
* [lib-방출.glsl](libraries-shader-api/lib-emissive-shader-api.md) : 방출 속성 도우미 포함
* [lib-env.glsl](libraries-shader-api/lib-env-shader-api.md) : 환경 맵 관련 도우미 포함
* [lib-normal.glsl](libraries-shader-api/lib-normal-shader-api.md) : 노멀 맵 관련 도우미(및 Height 맵이 생성한 노멀 맵)를 포함합니다.
* [lib-pbr.glsl](libraries-shader-api/lib-pbr-shader-api.md) : 물리적 기반의 렌더링 도우미를 포함합니다.
* [lib-pbr-aniso.glsl](libraries-shader-api/lib-pbr-aniso-shader-api.md) : 비등방성 물리적 기반 렌더링 도우미 포함
* [lib-pom.glsl](libraries-shader-api/lib-pom-shader-api.md) : 시차 오클루전 매핑 도우미 포함
* [lib-random.glsl](libraries-shader-api/lib-random-shader-api.md) : 임의 유틸리티(낮은 불일치 시퀀스)를 포함합니다.
* [lib-sampler.glsl](libraries-shader-api/lib-sampler-shader-api.md) : 채널 getters 도우미를 포함합니다.
* [lib-sparse.glsl](libraries-shader-api/lib-sparse-shader-api.md) : 안전한 스파스 텍스처 샘플링 도우미를 포함합니다.
* [lib-sss.glsl](libraries-shader-api/lib-sss-shader-api.md) : 서브서피스 스캐터링 도우미 포함
* [lib-utils.glsl](libraries-shader-api/lib-utils-shader-api.md) : 색상 유틸리티 함수(sRGB 변환, 톤 매핑)가 포함되어 있습니다.
* [lib-vectors.glsl](libraries-shader-api/lib-vectors-shader-api.md) : 공통 벡터 도우미 포함

## 메타데이터

불필요한 정보를 추가로 선언하여 렌더링 시스템에 힌트를 줄 수 있습니다. 구문은 다음과 같습니다.

```
//: metadata { 

//:   "key1":"value1", 

//:   "key2":"value2" 

//: }
```


지원되는 키는 다음과 같습니다.

* **custom-ui**: 표준 셰이더 매개 변수 사용자 인터페이스를 QML 모듈로 작성된 사용자 지정 보기로 바꿉니다(스크립팅 설명서 참조). 경로는 절대 경로이거나 셸프 *사용자 지정 ui* 폴더 중 하나에 상대적일 수 있습니다.
* **mdl**: 셰이더와 함께 사용할 Ray mdl 재질을 정의합니다. 경로 구문은 다음과 같습니다. *mdl::folder1::folder2::mdl\_filename::material\_name*. 여기서 *folder1::folder2::mdl\_filename*&#x200B;은(는) mdl 파일에 대한 셸프 *mdl* 폴더 중 하나의 내부 경로이고 *::material\_name*&#x200B;은(는) 이 mdl 파일 내에 선언된 재질의 이름입니다. (예: &quot;mdl&quot; : &quot;mdl::alg::materials::physically\_metallic\_roughness::physically\_metallic\_roughness&quot;)

## 셰이더 예시 (예, 마지막으로!)

실제 셰이더처럼 보이는 것을 맛보기 위해 복잡성을 증가시켜 정렬한 몇 가지 샘플 셰이더가 있습니다.

* [pixelated.glsl](shaders-shader-api/pixelated-shader-api.md) : 픽셀화 셰이더
* [toon.glsl](shaders-shader-api/toon-shader-api.md) : toon 셰이더
* [pbr-metal-rough.glsl](shaders-shader-api/pbr-metal-rough-shader-api.md) : Substance Painter에 포함된 기본 PBR 셰이더

## 동적 재질 레이어

동적 재질 레이어는 셰이더 내에서 재질이 함께 혼합되어 Substance Painter의 블렌딩 마스크를 사용자가 동적으로 편집할 수 있게 하는 특정 작업 과정입니다. 이 워크플로우를 활성화하려면 두 가지 새로운 기능이 있습니다.

* 셰이더 정의에서 편집 가능한 스택 선언: [layering\_declare\_stacks.glsl](parameters-shader-api/layering-declare-stacks-shader-api.md)
* 셰이더 매개 변수로 재질 바인딩: [레이어링\_bind\_materials.glsl](parameters-shader-api/layering-bind-materials-shader-api.md)
