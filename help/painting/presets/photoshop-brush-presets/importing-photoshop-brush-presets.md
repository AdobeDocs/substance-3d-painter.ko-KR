---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/painting/presets/photoshop-brush-presets-abr/importing-photoshop-brush-presets.html"
breadcrumb-title: ''
description: Photoshop 브러시 사전 설정(ABR 파일)을 Substance 3D Painter으로 가져와 브러시 라이브러리를 확장하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Photoshop Brush Presets (ABR) > Importing Photoshop Brush Presets
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Photoshop 브러시 사전 설정 가져오기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---


# Photoshop 브러시 사전 설정 가져오기

이 페이지에서는 ABR 파일을 Substance 3D Painter으로 가져오는 방법을 단계별로 설명합니다.

1. <b>리소스 가져오기 창을 엽니다.</b>

   자원 임포트 창은 다음 세 가지 방법으로 열 수 있습니다.

   * ABR 파일을 에셋 패널로 드래그하여 놓습니다.
   * 기본 메뉴에서 <b>파일 > 리소스 가져오기 </b>을(를) 사용합니다.
   * [에셋] 패널에서 <b>+ </b>버튼을 사용합니다.
1. <b>리소스 가져오기 창에 ABR 파일을 추가합니다.</b>

   ABR 파일을 에셋 창으로 드래그 앤 드롭하여 가져오기 창을 열지 않은 경우 기본적으로 비어 있습니다.

   ABR 파일을 추가하려면 다음 중 하나를 수행합니다.

   * ABR 파일을 창으로 **끌어 놓기**.
   * **리소스 추가** 단추를 클릭하여 ABR 파일을 선택하고 로드합니다.

   >[!NOTE]
   >
   > ![](../../../assets/shelf-import-error.png)
   > 
   > ABR 파일에 문제가 있는 경우 경고 아이콘이 파일 옆에 나타날 수 있습니다. 예:
   > 
   > * 호환되는 사전 설정이 없습니다. 자세한 내용은 [Photoshop 브러시 매개 변수 호환성](photoshop-brush-parameters-compatibility.md) 목록을 참조하십시오.
   > * 파일을 읽을 수 없습니다(예: 파일이 손상됨).
1. <b>ABR 파일을 가져오는 방법을 선택하세요.</b>

   자원 가져오기 창의 하단에서 ABR 파일을 로드할 위치를 선택합니다.

   * <b> 프로젝트</b>: ABR 파일이 현재 열려 있는 프로젝트로 로드됩니다. 브러쉬는 현재 프로젝트가 열려 있고 프로젝트 파일에 첨부된 경우에만 사용할 수 있습니다.
   * <b> 세션</b>: ABR 파일이 메모리에 로드됩니다. 브러시 사전 설정은 애플리케이션을 닫을 때까지 사용할 수 있습니다.
   * <b> 라이브러리</b>: ABR 파일이 디스크의 셸프에 복사됩니다. 브러시 사전 설정은 Painter을 열 때마다 모든 프로젝트에서 사용할 수 있습니다.

   ![](../../../assets/import-location.png)
1. <b>선반에서 브러시 사전 설정에 액세스합니다.</b>

   ![](../../../assets/shelf-demo.png)

   브러시 사전 설정을 가져오는 데 문제가 없으면 [에셋](../../../interface/assets/assets.md) 창에 표시됩니다.

   >[!NOTE]
   >
   > 브러시 사전 설정이 비트맵을 기반으로 하는 경우 사용하는 이미지는 브러시 사전 설정과 같은 이름으로 [선반]의 Alpha 섹션에서도 사용할 수 있습니다.
