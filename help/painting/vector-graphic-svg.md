---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/vector-graphic-svg.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 벡터 그래픽(SVG 및 AI 파일)을 사용하여 텍스처에 확장 가능한 벡터 아트워크를 추가하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 벡터 그래픽(SVG)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---


# 벡터 그래픽(.svg 및 .ai)

![매개 변수 목록 옆의 메시에 투영된 svg 파일을 보여 주는 이미지](../assets/svg_overview.png)

벡터 그래픽 파일(<b>.svg</b> 및 Illustrator <b>.ai</b> 모두)을 Painter 내에서 일반 이미지처럼 가져올 수 있습니다. 몇 가지 설정을 사용하여 그래픽의 모양을 조정하고 나머지 텍스처링에 더 잘 맞춥니다.

* SVG 파일에 대한 자세한 내용은 [이 페이지를 참조하세요](https://www.adobe.com/creativecloud/file-types/image/vector/svg-file.html).
* AI 파일에 대한 자세한 내용은 [이 페이지](https://www.adobe.com/ie/creativecloud/file-types/image/vector/ai-file.html)를 참조하세요.

SVG 및 AI 파일은 선택한 설정에 따라 [레이어 스택](../interface/layer-stack/layer-stack.md)에서 사용할 때 픽셀 이미지로 자동으로 변환됩니다. 비파괴 프로세스이며 해상도를 변경하거나 소스 파일을 업데이트하면 최종 결과도 업데이트됩니다.

## 속성

벡터 파일을 가져와 레이어 또는 도구 속성 내에 로드하면 다음과 같은 매개 변수 세트를 사용할 수 있습니다.

| 섹션 | 설정 | 설명 |
| --- | --- | --- |
| <b>대지</b> | <b>대지</b> | 파일에 포함된 대지를 선택합니다.  **참고:** 이 설정은 Illustrator(.ai) 파일에서만 사용할 수 있습니다. |
| <b>해상도</b> | 해결 방법 | 레이어 스택 내에서 텍스처링에 사용할 때 svg가 비트맵 이미지(픽셀)로 변환될 크기를 정의합니다.   가능한 값:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>자동</b>: 해상도는 현재 텍스처 세트(채우기 레이어/효과에서 사용 시) 또는 브러시 도구에서 사용 시 512픽셀의 해상도로 결정됩니다.<br/> </li> <li data-preserve-html="true"><b>에셋</b>: 해상도는 SVG 파일 자체 내에 정의된 픽셀 크기에 의해 결정됩니다.<br/> </li> <li data-preserve-html="true"><b>사용자 지정</b>: 해상도는 인터페이스의 바로 아래 해상도 설정에 의해 결정됩니다.</li> </ul>  <div><img alt="svg 해상도 설정" class="" data-preserve-html="true" id="root_content_flex_items_position_position-par_table_row-ad42696-column-7212622_image" src="../assets/svg_resolution_custom.png" title="svg 해상도 설정"/></div> |
|  |  |  |
| <b>자르기 영역</b> | 다음으로 자르기 | 렌더링된 영역으로 SVG 모양이 제한되는 방법을 정의합니다.   가능한 값:<ul data-preserve-html="true"> <li data-preserve-html="true"><b>에셋 경계</b>: 영역은 SVG 파일 내부에 정의된 경계로 정의됩니다.</li> <li data-preserve-html="true"><b>사용자 지정</b>: 영역은 바로 아래의 인터페이스 설정을 통해 명시적 값으로 정의됩니다.<br/> </li> </ul> |
|  | 정사각형 종횡비 | 자르기 영역이 <b>에셋 테두리</b>로 정의된 경우, 이 설정을 사용하면 SVG을 정사각형 이미지로 렌더링할 때 잘못된 스트레치가 발생하지 않고 원래 비율이 유지됩니다.   이 설정을 사용하면 일부 요소가 예기치 않게 표시될 수 있습니다. 이 문제를 방지하려면 이 설정을 비활성화하고 대신 채우기 레이어/효과 내에 있는 UV 설정을 수동으로 조정합니다. |
|  | 상단 왼쪽 하단 오른쪽 | 자르기가 [사용자 정의 영역]으로 설정된 경우 이러한 설정을 통해 왼쪽 위 및 오른쪽 아래 모퉁이를 지정하여 영역을 수동으로 정의할 수 있습니다. |
|  |  |  |
| <b>범위</b> | 범위 | 렌더링하기 전에 SVG 파일 내에 포함할 요소를 정의합니다.   기본값은 <b>문서</b>이며, 이는 SVG 파일의 모든 내용이 사용됨을 의미합니다. 포함할 요소를 조정하려면 <b>변경</b> 단추를 사용하십시오. |

### 범위 창

벡터 그래픽의 범위를 편집할 때는(위의 설정 참조) 최종 렌더링된 이미지에서 포함하거나 제외할 항목을 지정하기 위해 선택할 요소 목록이 창에 나타납니다.

<b>축소판 표시</b> 확인란을 사용하여 각 요소의 이미지를 표시합니다.

![](../assets/v10_ai_thumbs.jpg)
