---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/shaders-shader-api/pixelated-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter의 [픽셀화된 셰이더 API] 참조에 액세스하여 사용자 정의 픽셀화된 렌더링 효과를 만듭니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Shaders - Shader API > Pixelated - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 픽셀화 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---


# 픽셀화 - 셰이더 API

## 기본 픽셀화 셰이더

라이브러리에서 가져옵니다.

```
import lib-sampler.glsl
```


우리는 전체 빛의 위치를 정의한다

```
const vec3 light_pos = vec3(10.0, 10.0, 10.0);
```


자동 매개 변수 세계 눈 위치를 **camera\_pos**&#x200B;에 **바인딩**&#x200B;합니다.

```
//: param auto world_eye_position 

uniform vec3 camera_pos;
```


**문서의 채널**&#x200B;기본 색상&#x200B;**을(를) 균일한** basecolor\_tex **에 바인딩**&#x200B;합니다.

```
//: param auto channel_basecolor 

uniform SamplerSparse basecolor_tex;
```


이 셰이더에 대한 새 사용자 정의 트윅을 기본값과 함께 정의합니다. 이 옵션은 그림자가 표시되면 윤곽선의 Thickness을 조정하는 데 사용됩니다.

```
//: param custom { 

//:  "default": 0.4, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Unlit outline thickness" 

//: } 

uniform float unlit_outline_thickness;
```


이 셰이더에 대한 새 사용자 정의 트윅을 기본값과 함께 정의합니다. 이 클립은 불이 켜져 있을 때 외곽선의 Thickness을 조정하는 데 사용됩니다.

```
//: param custom { 

//:   "default": 0.1, 

//:   "min": 0.0, 

//:   "max": 1.0, 

//:   "label": "Lit outline thickness" 

//: } 

uniform float lit_outline_thickness;
```


셰이더의 진입점입니다.

```
void shade(V2F inputs) 

{
```


우리는 몇 가지 유용한 값을 계산한다.

```
  vec3 V = normalize(camera_pos - inputs.position); 

  vec3 N = normalize(inputs.normal); 

  vec3 L = normalize(light_pos - inputs.position); 

  float NdV = dot(N, V); 

  float NdL = max(0.0, dot(N, L));
```


**우선 순위**&#x200B;는 **윤곽선 검색**&#x200B;을 수행하는 것입니다. 윤곽선 조건에 도달하면 검은색으로 종료합니다.

```
  if (NdV < mix(unlit_outline_thickness, lit_outline_thickness, NdL)) { 

    return; 

  } 

 

  vec3 baseColor = getBaseColor(basecolor_tex, inputs.sparse_coord);
```


기본 색상 광도를 기반으로 마스크 크기에 일부 지터 도입

```
  float maskRadiusJitter = pow(dot(baseColor, vec3(0.3333)), 0.1);
```


조각의 화면 공간 위치를 기반으로 마스크 값을 계산합니다. 그러면 격자와 같은 패턴이 만들어집니다.

```
  float mask = pow(1.0 - length(fract(gl_FragCoord.xy / 7.0) - vec2(0.5)), maskRadiusJitter * 5.0) * 5.0;
```


여기서 우리는 베이스 색상을 샘플링하고 간단한 확산 감쇠를 적용한다

```
  vec3 color = baseColor * NdL; 

 

  diffuseShadingOutput(mask * color); 

} 

 
```
