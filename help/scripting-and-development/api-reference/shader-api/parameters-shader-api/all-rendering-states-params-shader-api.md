---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/scripting-and-development/api-reference/shader-api/parameters-shader-api/all-rendering-states-params-shader-api.html"
breadcrumb-title: ''
description: 렌더링 상태 매개 변수를 제어하려면 Substance 3D Painter의 모든 렌더링 상태 매개 변수 셰이더 API 참조에 액세스하십시오.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Parameters - Shader API > All Rendering States Params - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 모든 렌더링 상태 매개 변수 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 2%

---


# 모든 렌더링 상태 매개 변수 - 셰이더 API

## 렌더링 상태 예

## 백페이스 컬링

뒷면 오려내기:

```
//: state cull_face on
```


앞면과 뒷면 그리기:

```
//: state cull_face off
```


## 혼합

혼합되지 않고 완전히 불투명한 개체:

```
//: state blend none
```


맨 뒤로 그리기 순서에 대한 표준 혼합 모드:

```
//: state blend over
```


앞뒤로 그리기 순서에 대한 표준 혼합 모드입니다. 색상에 알파가 미리 곱해졌다고 가정합니다.

```
//: state blend over_premult
```


추가 혼합 모드:

```
//: state blend add
```


곱하기 혼합 모드:

```
//: state blend multiply
```


## 셰이더 샘플링 지역

기본적으로 문서 채널은 페인팅 중에 렌더링 최적화를 위해 변환되지 않은 텍스처 좌표를 사용하여 샘플링됩니다.

아티팩트가 표시되는 경우 *nonlocal* 상태를 *on*(으)로 설정합니다.

```
//: state nonlocal on 

 
```
