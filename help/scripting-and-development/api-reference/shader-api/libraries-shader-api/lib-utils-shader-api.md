---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-utils-shader-api.html"
breadcrumb-title: ''
description: Substance 3D Painter에 대한 Lib Utils 셰이더 API 참조에 액세스하여 사용자 정의 셰이더 개발에서 유틸리티 함수를 사용합니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Utils - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib 유틸리티 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 1%

---


# Lib 유틸리티 - 셰이더 API

## 알레고리학 유틸리티 함수

## 톤 매핑

다음은 셰이더에서 사용할 수 있는 톤 매핑의 예입니다. Painter은 Yebis가 적용한 옵션 매핑을 제외한 톤 매핑을 적용하지 않습니다. 셰이더에서 톤 매핑을 수행하기로 결정한 경우 Yebis 톤 매핑 앞에 적용됩니다.

sigma와 n 매개 변수를 기반으로 S-커브 톤 매핑을 수행합니다.

```
vec3 tonemapSCurve(vec3 value, float sigma, float n) 

{ 

  vec3 pow_value = pow(value, vec3(n)); 

  return pow_value / (pow_value + pow(sigma, n)); 

}
```


## sRGB 변환

Painter에서 사용되는 변환입니다. 사용자 정의 셰이더에 다음 선을 넣어 뷰포트에서 자동 선형 -> sRGB 변환을 재정의할 수 있습니다.

*#define DISABLE\_FRAMEBUFFER\_SRGB\_CONVERSION*

사용자 정의 변환을 수행합니다.

sRGB에서 선형 색상 변환으로 스칼라 버전입니다.

```
float sRGB2linear(float x) 

{ 

  return x <= 0.04045 ? 

    x * 0.0773993808 : // 1.0/12.92 

    pow((x + 0.055) / 1.055, 2.4); 

}
```


sRGB에서 선형 색상 변환으로 RGB 버전.

```
vec3 sRGB2linear(vec3 rgb) 

{ 

  return vec3( 

    sRGB2linear(rgb.r), 

    sRGB2linear(rgb.g), 

    sRGB2linear(rgb.b)); 

}
```


sRGB에서 선형 색상 변환으로 RGB + Alpha 버전.

```
vec4 sRGB2linear(vec4 rgba) 

{ 

  return vec4(sRGB2linear(rgba.rgb), rgba.a); 

}
```


선형-sRGB 색상 변환. 스칼라 버전입니다.

```
float linear2sRGB(float x) 

{ 

  return x <= 0.0031308 ? 

      12.92 * x : 

      1.055 * pow(x, 0.41666) - 0.055; 

}
```


선형-sRGB 색상 변환. RGB 버전.

```
vec3 linear2sRGB(vec3 rgb) 

{ 

  return vec3( 

      linear2sRGB(rgb.r), 

      linear2sRGB(rgb.g), 

      linear2sRGB(rgb.b)); 

}
```


선형-sRGB 색상 변환. RGB + Alpha 버전.

```
vec4 linear2sRGB(vec4 rgba) 

{ 

  return vec4(linear2sRGB(rgba.rgb), rgba.a); 

}
```


선형-sRGB 색상 변환(선택 사항) 스칼라 버전입니다.

```
//: param auto conversion_linear_to_srgb 

uniform bool convert_to_srgb_opt; 

float linear2sRGBOpt(float x) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(x) : x; 

}
```


선형-sRGB 색상 변환(선택 사항) RGB 버전.

```
vec3 linear2sRGBOpt(vec3 rgb) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgb) : rgb; 

}
```


선형-sRGB 색상 변환(선택 사항) RGB + Alpha 버전.

```
vec4 linear2sRGBOpt(vec4 rgba) 

{ 

  return convert_to_srgb_opt ? linear2sRGB(rgba) : rgba; 

}
```


색상 변환. 스칼라 버전입니다.

```
uniform int output_conversion_method; 

float convertOutput(float x) 

{ 

 if (output_conversion_method == 0) return x; 

 else if (output_conversion_method == 1) return linear2sRGB(x); 

 else return sRGB2linear(x); 

}
```


색상 변환. RGB 버전.

```
vec3 convertOutput(vec3 rgb) 

{ 

 if (output_conversion_method == 0) return rgb; 

 else if (output_conversion_method == 1) return linear2sRGB(rgb); 

 else return sRGB2linear(rgb); 

}
```


색상 변환. RGB + Alpha 버전.

```
vec4 convertOutput(vec4 rgba) 

{ 

 if (output_conversion_method == 0) return rgba; 

 else if (output_conversion_method == 1) return linear2sRGB(rgba); 

 else return sRGB2linear(rgba); 

}
```


## 디더링

음영에 디더링을 추가하는 몇 가지 도우미입니다.

디더링 모드에 8x8 Bayer 행렬 사용

```
import lib-bayer.glsl 

 

float getDitherThreshold(uvec2 coords) 

{ 

  return bayerMatrix8(coords); 

} 

 

 

vec4 RGB2Gray(vec4 rgba) 

{ 

  float gray = 0.299 * rgba.r + 0.587 * rgba.g + 0.114 * rgba.b; 

  return vec4(vec3(gray), rgba.a); 

}
```


광택이 있는 금속 표면에서 AO 및 그림자 제거(거울에 가까움)

```
float specularOcclusionCorrection(float diffuseOcclusion, float metallic, float roughness) 

{ 

  return mix(diffuseOcclusion, 1.0, metallic * (1.0 - roughness) * (1.0 - roughness)); 

} 

 
```
