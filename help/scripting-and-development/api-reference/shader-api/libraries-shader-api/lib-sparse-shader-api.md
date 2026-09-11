---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/api-reference/shader-api/libraries-shader-api/lib-sparse-shader-api.html"
breadcrumb-title: ''
description: 사용자 정의 셰이더에서 스파스 셰이더 API 샘플링을 사용하려면 Substance 3D Painter에 대한 Lib 스파스 텍스처 참조에 액세스하십시오.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > API Reference > Shader API > Libraries - Shader API > Lib Sparse - Shader API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Lib 스파스 - 셰이더 API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Lib 스파스 - 셰이더 API

## lib-sparse.glsl

이 파일은 스파스 텍스처 샘플링 정확도를 보장하기 위한 유용한 함수(ARB\_sparse\_texture)를 제공합니다. 비디오 메모리에 실제로 있는 텍스처의 일부만 샘플링할 수 있습니다.

**공용 함수:** *getSparseCoord* *getSparseCoordLod0* *textureSparseQueryLod* *textureSparse*

**공용 구조:** *SamplerSparse* *SparseCode*

*FEATURE\_SPARSE\_텍스처* 매크로는 스파스 가상 텍스처 확장이 활성화된 경우에만 정의됩니다.

활성화된 경우 추가 텍스처 조회 검사를 처리하여 텍스트가 누락된 경우 밉맵 피라미드를 위로 올라갈 수 있습니다.

```
## ifdef FEATURE_SPARSE_TEXTURE

//: param auto material_lod_check_needed 

uniform bool material_lod_check_needed = false; 

//: param auto material_lod_mask 

uniform usampler2D material_lod_mask; 

## endif // FEATURE_SPARSE_TEXTURE

//: param auto uvtile_reference_sampler 

uniform sampler2D uvtile_reference_sampler; 

//: param auto uvtile_size 

uniform vec2 uvtile_size; 

//: param auto uvtile_inverse_size 

uniform vec2 uvtile_inverse_size; 

//: param auto uvtile_lod_bias 

uniform float uvtile_lod_bias;
```


Sampler 및 스파스 텍스처 정보 구조

단일 자동 바인딩으로 모든 샘플러 관련 유니폼을 쿼리하는 데 사용됨

```
struct SamplerSparse { 

  sampler2D tex; 

  vec4 size; // width, height, 1/width, 1/height 

  bool is_set; // a boolean indicating whether the texture is in the texture set or not 

  uvec3 lod_mask_select; // masking operations description allowing to retrieve loaded mipmaps information 

};
```


스파스 샘플링 좌표

UV 좌표 및 재료 기반 희소 LoD 마스크 저장

```
struct SparseCoord { 

  vec2 tex_coord; 

  vec2 dfdx; 

  vec2 dfdy; 

  float lod; 

  uint material_lod_mask; 

}; 

 

 

## if defined(SHADER_FRAGMENT)
```


*textureSparse()* 샘플링 함수에 사용되는 빌드 텍스처 좌표 구조입니다(조각 셰이더에서 호출해야 함).

예: *SparseCoord uv1coord = getSparseCoord(inputs.multi\_tex\_coord[1]);*

```
SparseCoord getSparseCoord(vec2 tex_coord) { 

  SparseCoord res; 

  res.tex_coord = tex_coord; 

  res.dfdx = dFdx(tex_coord); 

  res.dfdy = dFdy(tex_coord); 

## ifdef FEATURE_SPARSE_TEXTURE

  res.material_lod_mask = material_lod_check_needed ? 

    textureLod(material_lod_mask,tex_coord,0.0).r : 

    0u; 

  res.lod = getLodFromReferenceSampler(tex_coord); 

## endif // FEATURE_SPARSE_TEXTURE

  return res; 

} 

## endif
```


*textureSparse()* 샘플링 함수에 사용되는 빌드 텍스처 좌표 구조 기본 수준 샘플링 버전(외부 조각 셰이더인 경우 사용 가능)

```
SparseCoord getSparseCoordLod0(vec2 tex_coord) { 

  SparseCoord res; 

  res.tex_coord = tex_coord; 

  res.dfdx = vec2(0.0); 

  res.dfdy = vec2(0.0); 

## ifdef FEATURE_SPARSE_TEXTURE

  res.material_lod_mask = material_lod_check_needed ? 

    textureLod(material_lod_mask,tex_coord,0.0).r : 

    0u; 

  res.lod = 0.0; 

## endif // FEATURE_SPARSE_TEXTURE

  return res; 

} 

 

## if defined(SHADER_FRAGMENT)
```


스파스 텍스처에서 샘플링하는 데 사용할 세부 수준을 계산합니다.

Climb up mipmap pyramid if texels is missing Lots LoD BEFORE LoD bias applied

```
float textureSparseQueryLod(SamplerSparse sampler, SparseCoord coord) { 

## ifdef FEATURE_SPARSE_TEXTURE

  float lodfix = coord.lod; 

  if (material_lod_check_needed) { 

    lodfix = getFixedSparseLod(getTextureLodMask(sampler.lod_mask_select, coord.material_lod_mask), lodfix); 

  } 

  return lodfix-uvtile_lod_bias; 

## else // FEATURE_SPARSE_TEXTURE

  return textureQueryLod(sampler.tex, coord.tex_coord).y-uvtile_lod_bias; 

## endif // FEATURE_SPARSE_TEXTURE

} 

## endif // SHADER_FRAGMENT
```


스파스 텍스처에서 샘플링하는 데 사용되는 파생 함수 계산

텍스트가 없는 경우 밉맵 피라미드 위로 올라가기

```
void textureSparseQueryGrad(out vec2 dfdx, out vec2 dfdy, SamplerSparse sampler, SparseCoord coord) { 

## ifdef FEATURE_SPARSE_TEXTURE

  if (material_lod_check_needed) { 

    float lodfix = getFixedSparseLod(getTextureLodMask(sampler.lod_mask_select, coord.material_lod_mask), coord.lod); 

    if (coord.lod!=lodfix) { 

      // Fix dfdx dfdy, take account offset, no more anisotropy 

      vec2 ddfix = exp2(lodfix-uvtile_lod_bias) * uvtile_inverse_size; 

      dfdx = vec2(ddfix.x,0.0); 

      dfdy = vec2(0.0,ddfix.y); 

      return; 

    } 

  } 

## endif // FEATURE_SPARSE_TEXTURE

  dfdx = coord.dfdx; 

  dfdy = coord.dfdy; 

}
```


스파스 텍스처에 대해 텍스처 조회를 수행합니다. 필요한 경우 밉맵 레벨 위로 이동합니다.

이 함수는 표준 *텍스처(sampler2D, vec2)*&#x200B;을(를) 대체하여 스파스 텍스처에서 텍셀을 검색합니다

```
vec4 textureSparse(SamplerSparse sampler, SparseCoord coord) { 

  vec2 dfdx,dfdy; 

  textureSparseQueryGrad(dfdx, dfdy, sampler, coord); 

  return textureGrad(sampler.tex, coord.tex_coord, dfdx, dfdy); 

}
```


지정된 텍스처에서 오프셋이 작은 최적화된 다중 텍스처 조회를 수행합니다

최대 N=4에 대해 이 도우미의 대체 버전을 제공하고 있습니다.

```
void textureSparseOffsets(SamplerSparse sampler, SparseCoord coord, vec2 offsets[N], out vec4 results[N]) { 

  vec2 dfdx,dfdy; 

  textureSparseQueryGrad(dfdx, dfdy, sampler, coord); 

  for(int i = 0; i < N; ++i) { 

    results[i] = textureGrad(sampler.tex, coord.tex_coord + offsets[i], dfdx, dfdy); 

  } 

} 

 
```
