---
title: 필터
description: Substance 3D Painter에서 필터 효과를 사용하여 이미지 처리 필터 및 텍스처 조정을 적용하는 방법에 대해 알아봅니다.
source-git-commit: 4b8afda243f2969b036efe14588f201177ee3139
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 3%
---

# 필터

필터 효과는 레이어 또는 레이어의 내용을 마스킹하는 물질입니다. 패스스루 혼합 모드에서는 레이어에서 레이어 스택 결과를 수정할 수 있습니다. 따라서 패스스루 혼합 모드에서는 레이어에 필터를 사용하여 레이어 스택 전체를 수정할 수 있습니다.

## 필터를 적용하려면 어떻게 해야 합니까?

필터 유형에 따라 레이어의 콘텐츠 또는 마스크에 필터 효과를 만들어야 합니다. 필터를 적용하는 방법에는 두 가지가 있습니다.

* 수동 방식은 필터를 설정하기 위해 여러 단계가 필요하지만, 프로세스의 각 단계에 대한 직접 제어를 제공합니다.
* 드래그하여 놓기 방식을 사용하면 필터를 빠르게 추가하고 모든 채널에서 혼합 모드를 통과하도록 자동으로 설정할 수 있습니다.

### 수동으로 필터 추가

다음 예제에서는 흐림 효과 필터가 레이어 콘텐츠에 적용되지만 마스크에 필터를 적용하는 데 더 일반적으로 사용됩니다.

**1. 필터 효과 추가**

먼저 레이어의 콘텐츠 또는 레이어 마스크를 선택한 다음 **효과 단추**&#x200B;를 클릭하거나 마우스 오른쪽 단추를 클릭하여 컨텍스트 메뉴를 엽니다. 목록에서 &quot; **필터 추가**&quot; 옵션을 선택합니다.

![](../../assets/filters/filter-add-manually.gif)

**2. 속성 창에서 필터 선택**

**속성 패널**&#x200B;에서 필터가 아직 선택되지 않았습니다. 필터 선택 단추를 클릭하여 미니 쉘프를 열고 원하는 필터를 선택합니다. 여기서 **흐림 효과 필터**&#x200B;를 선택합니다.
![](../../assets/filters/filter-select.gif)

>[!NOTE]
>
> 필터를 수동으로 적용하는 경우 필터가 그 아래에 있는 레이어의 내용에 영향을 주도록 하려면 통과 혼합 모드를 사용해야 할 수도 있습니다.

## 셸프에서 필터 드래그 앤 드롭

이 방법은 전체 Layerstack에 적용해야 하는 필터를 위해서만 제공됩니다. 모든 채널 [혼합 모드](../../interface/layer-stack/blending-modes.md)가 자동으로 설정됩니다. 마스크에 필터를 적용하는 데는 작동하지 않습니다.

**1. 셸프의 필터 영역 열기**

셸프에서 왼쪽의 &quot;필터&quot; 섹션을 클릭합니다.

![](../../assets/shelf-filters.gif)

**2. 필터**&#x200B;을(를) 끌어서 놓습니다.

선반에 사용할 필터를 선택합니다. 레이어 스택에 끌어다 놓아 올바른 위치에 배치해야 합니다(예: 원치 않는 그룹에 떨어뜨리지 마십시오).

![](../../assets/filter-dragdrop.gif)

위의 예시에서 드롭된 필터에는 [패스스루 혼합] 모드가 이미 있습니다. 문서의 모든 채널에 적용됩니다.

## Painter에 새 필터 추가

Painter으로 가져올 새 필터가 있는 경우 표준 리소스를 추가하는 것처럼 추가할 수 있습니다. SBSAR 파일을 **에셋 패널**&#x200B;로 드래그하여 놓으면 새 필터 가져오기를 관리할 수 있습니다.

## 나만의 필터 만들기

모든 필터는 Substance으로, Substance 3D Designer으로 만들 수 있습니다. Substance 3D Designer은 빠르게 시작할 수 있도록 Substance 3D Painter 템플릿을 제공합니다.

자세한 내용은 이 페이지([사용자 지정 효과 만들기](../../content/creating-custom-effects/creating-custom-effects.md))를 참조하십시오.

## Painter의 기본 필터

### 표준

* [흐리게](filters/standard/blur.md)
* [흐림 방향](filters/standard/blur-directional.md)
* [흐림 경사](filters/standard/blur-slope.md)
* [클램프](filters/standard/clamp.md)
* [색상 균형](filters/standard/color-balance.md)
* [색상 보정](filters/standard/color-correct.md)
* [대비 광도](filters/standard/contrast-luminosity.md)
* [그림자](filters/standard/drop-shadow.md)
* [영역 색상 채우기](filters/standard/fill-area-color.md)
* [영역 마스크 채우기](filters/standard/fill-area-mask.md)
* [FXAA (앤티 앨리어스)](filters/standard/fxaa-anti-aliasing.md)
* [광선](filters/standard/glow.md)
* [그래디언트](filters/standard/gradient.md)
* [동적 그레이디언트](filters/standard/gradient-dynamic.md)
* [회색 음영 전환](filters/standard/grayscale-conversion.md)
* [하이패스](filters/standard/highpass.md)
* [막대 그래프 스캔](filters/standard/histogram-scan.md)
* [히스토그램 이동](filters/standard/histogram-shift.md)
* [HSL 가시 범위](filters/standard/hsl-perceptive.md)
* [반전](filters/standard/invert.md)
* [대칭](filters/standard/mirror.md)
* [픽셀화](filters/standard/pixelate.md)
* [포스터화](filters/standard/posterize.md)
* [선명하게](filters/standard/sharpen.md)
* [Smoothstep](filters/standard/smoothstep.md)
* [임계값](filters/standard/threshold.md)
* [변환](filters/standard/transform.md)
* [뒤틀기](filters/standard/warp.md)

### 완료

* [MatFinish 브러시 적용 선형](filters/finishes/matfinish-brushed-linear.md)
* [MatFinish 아연 도금](filters/finishes/matfinish-galvanized.md)
* [매트피니시 그레인](filters/finishes/matfinish-grainy.md)
* [매트피니쉬연삭](filters/finishes/matfinish-grinded.md)
* [MatFinish Hammered](filters/finishes/matfinish-hammered.md)
* [MatFinish 천공 원](filters/finishes/matfinish-perforated-circles.md)
* [MatFinish 파우더 코팅](filters/finishes/matfinish-powder-coated.md)
* [매트 피니시](filters/finishes/matfinish-raw.md)
* [매트 피니시 러프](filters/finishes/matfinish-rough.md)

### MatFx

* [MatFX Comic Book](filters/matfx/matfx-comic-book.md)
* [MatFX 세부 정보 Edge Wear](filters/matfx/matfx-detail-edge-wear.md)
* [MatFX Edge Damage](filters/matfx/matfx-edge-damages.md)
* [MatFX HBAO](filters/matfx/matfx-hbao.md)
* [MatFX 오일 페인트](filters/matfx/matfx-oil-paint.md)
* [MatFX 필링 페인트](filters/matfx/matfx-peeling-paint.md)
* [MatFX 녹 풍화](filters/matfx/matfx-rust-weathering.md)
* [MatFX 차단 라인](filters/matfx/matfx-shut-line.md)
* [MatFX Watercolor](filters/matfx/matfx-watercolor.md)
* [MatFX 물방울](filters/matfx/matfx-water-drops.md)

### 조명

* [베이크된 조명 환경](filters/lighting/baked-lighting-environment.md)
* [스타일이 적용된 구운 조명](filters/lighting/baked-lighting-stylized.md)

### 고급

* [비등방성 구와하라](filters/advanced/anisotropic-kuwahara.md)
* [경사](filters/advanced/bevel.md)
* [베벨 매끄럽게](filters/advanced/bevel-smooth.md)
* [색상 일치](filters/advanced/color-match.md)
* [방향 거리](filters/advanced/directional-distance.md)
* [그레이디언트 곡선](filters/advanced/gradient-curve.md)
* [Height 조정](filters/advanced/height-adjustments.md)
* [Height을 표준으로](filters/advanced/height-to-normal.md)
* [마스크 윤곽선](filters/advanced/mask-outline.md)
* [PBR 유효성 검사](filters/advanced/pbr-validate.md)
* [정량화](filters/advanced/quantize.md)
* [스타일화](filters/advanced/stylization.md)
* [3회 평면 고급](filters/advanced/tri-planar-advanced-filter.md)
