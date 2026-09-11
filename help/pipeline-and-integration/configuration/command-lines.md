---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/pipeline-and-integration/configuration/command-lines.html"
breadcrumb-title: ''
description: 자동화, 스크립팅 및 파이프라인 통합을 위해 Substance 3D Painter에서 명령줄 인수를 사용하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Configuration > Command lines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 명령줄
user-guide-description: ''
user-guide-title: ''
source-git-commit: 22871eab2f25d09bd82f1292d8b3e5f8c4f1c2cf
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 3%

---


# 명령줄

이 페이지에는 프로젝트를 만들거나 열기 위해 응용 프로그램을 실행할 때 사용할 수 있는 여러 명령줄이 나열되어 있습니다.\
이러한 명령줄은 다음과 같이 사용할 수 있습니다.

```
"Adobe Substance 3D Painter.exe" --command [option] 
```


## 명령 목록

| Command | 설명 |
| --- | --- |
| **—도움말** **-?** **-h** | 사용할 수 있는 명령줄과 명령줄을 사용하는 방법에 대한 정보를 표시합니다. |
| **—버전** **-v** | Substance 3D Painter의 현재 버전을 표시합니다. |
| **—메시** | 프로젝트에 로드할 메시.예: `// Create a new project with a specific mesh   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj"       // Update a mesh inside an existing project   "Adobe Substance 3D Painter.exe" --mesh "E:/MymeshFolder/MyMesh.obj" "E:/MyMeshFolder/Project.spp"` |
| **—mesh-map** | 메쉬(AO, 표준, 곡률)와 연결된 베이킹된 맵 여러 번 지정할 수 있습니다. 이름 지정 : TextureSetName\_AdditionalMapSlot<ul data-preserve-html="true"> <li data-preserve-html="true">앰비언트 오클루전 = <strong> <em> ambient_오클루전 </em> </strong></li> <li data-preserve-html="true">곡률 = <strong> <em> 곡률 </em> </strong></li> <li data-preserve-html="true">표준 = <strong> <em> normal_base </em> </strong></li> <li data-preserve-html="true">월드 공간 표준 = <strong> <em> world_space_normals </em> </strong></li> <li data-preserve-html="true">위치 = <strong> <em> 위치 </em> </strong></li> <li data-preserve-html="true">Thickness = <strong> <em> Thickness </em> </strong></li> <li data-preserve-html="true">ID = <em> <strong> id </strong> </em></li> </ul>예: `"Adobe Substance 3D Painter.exe" --mesh "E:/MyMeshFolder/MyMesh.obj" --mesh-map " E:/MyMeshFolder/DefaultMaterial_ambient_occlusion.png"` |
| **—split-by-udim** | UDIM 타일별로 텍스처 세트를 만듭니다. |
| **—export-path** | 프로젝트의 출력을 내보낼 기본 내보내기 경로입니다. |
| **—vram-budget** | Substance 3D Painter 엔진에서 정의한 비디오 메모리(VRAM) 예산을 재정의합니다. &quot;양&quot;은 메가바이트 단위입니다.    예: `// Set the VRam budget to 2GB   "Adobe Substance 3D Painter.exe" --vram-budget 2048` |
| **—disable-version-checking** | 시작할 때 새 버전의 응용 프로그램을 사용할 수 있는지 확인하지 않음 |
| **—enable-remote-scripting** | 응용 프로그램 외부에서 스크립팅 명령을 실행할 수 있습니다. 자세한 내용은 [스크립팅을 사용한 원격 제어](../../scripting-and-development/scripts-and-plugins/remote-control-with-scripting.md)를 참조하세요. |
