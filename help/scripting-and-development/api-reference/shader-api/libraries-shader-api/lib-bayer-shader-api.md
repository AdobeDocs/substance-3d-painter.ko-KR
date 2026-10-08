---
breadcrumb-title: ""
description: Substance 3D Painter용 Lib Bayer 셰이더 API 참조에 액세스하여 사용자 정의 셰이더에서 Bayer 디더링 패턴을 만들 수 있습니다.
title: Lib Bayer - 셰이더 API
user-guide-description: ""
user-guide-title: ""
source-git-commit: 6b6d52207ca1d043aaa1b2b14145b6b49d4c1942
workflow-type: tm+mt
source-wordcount: '32'
ht-degree: 0%
---

# Lib Bayer - 셰이더 API

## lib-bayer.glsl

**공용 함수:** *bayerMatrix8*

```
float bayerMatrix8(uvec2 coords) { 

  return (float(bayer(coords.x, coords.y)) + 0.5) / 64.0; 

} 

 
```
