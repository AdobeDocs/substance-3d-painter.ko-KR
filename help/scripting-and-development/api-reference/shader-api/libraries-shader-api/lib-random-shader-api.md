---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-random-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter에 대한 Lib Random 셰이더 API 참조에 액세스하여 사용자 정의 셰이더 개발에서 임의 값을 생성합니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Random - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 임의 라이브러리 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---


# 임의 라이브러리 - 셰이더 API

## lib-random.glsl

**공용 함수:** *getBlueNoiseThreshold* *getBlueNoiseThresholdTemporal* *fibonacci1D* *fibonacci2D* *fibonacci2DDitheredTemporal*

라이브러리에서 가져오기

```
import lib-defines.glsl
```


스칼라 값을 포함하는 2D 파랑 노이즈 텍스처

```
//: param auto texture_blue_noise 

uniform sampler2D texture_blue_noise;
```


파란색 노이즈 텍스처 해상도

```
const ivec2 texture_blue_noise_size = ivec2(256);
```


현재 프레임 임의 시드

```
//: param auto random_seed 

uniform int alg_random_seed;
```


픽셀 좌표를 기준으로 균일한 난수 값을 가져옵니다.

```
float getBlueNoiseThreshold() 

{ 

  return texture(texture_blue_noise, gl_FragCoord.xy / vec2(texture_blue_noise_size)).x + 0.5 / 65536.0; 

}
```


픽셀 좌표 및 프레임 ID를 기반으로 균일한 난수 값을 가져옵니다.

```
float getBlueNoiseThresholdTemporal() 

{ 

  return fract(getBlueNoiseThreshold() + M_GOLDEN_RATIO * alg_random_seed); 

}
```


피보나치 시퀀스에서 i *번째* 번호를 반환합니다.

```
float fibonacci1D(int i) 

{ 

  return fract((float(i) + 1.0) * M_GOLDEN_RATIO); 

}
```


피보나치 시퀀스에서 i *번째* 커플을 반환합니다. nbSample은 균일한 분포를 얻기 위해 필요하다.

```
vec2 fibonacci2D(int i, int nbSamples) 

{ 

  return vec2( 

    (float(i)+0.5) / float(nbSamples), 

    fibonacci1D(i) 

  ); 

}
```


피보나치 시퀀스에서 i *번째* 커플을 반환합니다. nbSample은 균일한 분포를 얻기 위해 필요하다. 이 버전에는 프레임 단위 및 픽셀 단위 의사 랜덤 회전이 적용되어 있습니다.

```
vec2 fibonacci2DDitheredTemporal(int i, int nbSamples) 

{ 

  vec2 s = fibonacci2D(i, nbSamples); 

  s.x += getBlueNoiseThresholdTemporal(); 

  return s; 

} 

 
```
