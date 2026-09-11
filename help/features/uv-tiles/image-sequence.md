---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/features/uv-tiles/image-sequence.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 UV 타일과 함께 이미지 시퀀스를 사용하여 애니메이션 텍스처 워크플로우에 사용하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Features > UV Tiles > Image Sequence
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 이미지 시퀀스
user-guide-description: ''
user-guide-title: ''
source-git-commit: 8b892d2d6c9d0f1a3b5d9d3ab9b180a7c2770a83
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# 이미지 시퀀스

이미지 시퀀스는 셸프에서 단일 리소스로 그룹화된 이미지 컬렉션입니다. 이미지는 파일 이름의 특정 패턴을 기준으로 그룹화됩니다.

## 이미지를 시퀀스로 가져오는 방법

이미지 파일을 가져올 때 파일 이름이 특정 패턴과 일치하면 자동으로 시퀀스로 가져옵니다. 가져온 파일 옆에 추가 이미지가 있는 경우 이 이미지도 고려됩니다. 그러므로 시퀀스에서 모든 파일을 수동으로 가져올 필요는 없으며 첫 번째 파일을 선택하면 됩니다.

파일 이름 일치 예:

다음 파일 이름은 파일 이름의 마지막 부분이 UDIM 번호 1032를 가리키고 있음을 인식할 수 있으므로 이미지 시퀀스를 성공적으로 가져옵니다.

* file\_22.1032.jpg
* file\_22-223.1032.jpg
* file\_22-223-1032.jpg
* file\_22-223\_1032.jpg

다음 파일 이름은 올바르게 구성되지 않아 이미지 시퀀스로 가져올 수 없습니다.

* file\_22-2232032.jpg
* file\_22-223PM2032.jpg
* file\_22-223-0032.jpg
* file\_22-223\_Rec2020.jpg

파일 이름 일치는 다음 정규식을 기반으로 합니다.

```
 ^(.+?)[\.\-\_](?
```


## 이미지 시퀀스를 사용하는 방법

이미지 시퀀스는 다른 리소스처럼 인터페이스의 임의 리소스 슬롯에 로드될 수 있습니다. 그러나 경우에 따라 설정을 추가로 사용해야 제대로 사용할 수 있습니다.

[레이어 채우기](../../painting/fill-projections/fill-projections.md)(및 채우기 효과)에서 투영 모드가 **채우기(UV 타일에 따라 일치)**&#x200B;으로 설정되어 있는지 확인하여 시퀀스의 각 이미지가 [텍스처 세트]의 오른쪽 [UV 타일](uv-tiles.md)에 할당되었는지 확인하십시오.
