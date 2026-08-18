---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/scripting-and-development/scripts-and-plugins/creating-a-javascript-plugin.html"
breadcrumb-title: ''
description: Substance 3D Painter용 JavaScript 플러그인을 만들어 기능을 확장하고 사용자 정의 작업 과정을 자동화하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > Scripts and plugins > Creating a Javascript plugin
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Javascript 플러그인 만들기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 1%

---


# Javascript 플러그인 만들기

이 단계별 안내서에서는 프로젝트에서 현재 선택한 레이어의 마스크를 내보낼 수 있는 간단한 플러그인을 만드는 방법에 대해 설명합니다.

이 안내서의 플러그인의 목표는 프로젝트 내에 있는 현재 텍스처 세트의 모든 채널을 개별 텍스처로 내보내는 것입니다.

## 1 - 플러그인 폴더로 이동

새 Javascript 플러그인을 추가하려면 Substance 3D Painter의 플러그인 폴더에 폴더를 만들어야 합니다.

**플러그인** 폴더에 액세스하려면 다음으로 이동하십시오.

<table data-preserve-html="true" style="width: 100.0%;"> <colgroup> <col style="width: 15.0%;"/> <col style="width: 15.0%;"/> <col style="width: 70.0%;"/> </colgroup> <tbody> <tr> <th>플랫폼</th> <th>버전</th> <th>경로</th> </tr> <tr> <td rowspan="2"><strong>Windows</strong></td> <td><strong>7.2</strong> 이상</td> <td colspan="1">C:\Users\username\Documents\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">레거시</td> <td colspan="1">C:\Users\username\Documents\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>Mac</strong></td> <td colspan="1"><strong>7.2</strong> 이상</td> <td colspan="1">/Users/사용자 이름/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td colspan="1">레거시</td> <td colspan="1">/Users/사용자 이름/Documents/Allegorithmic/Substance Painter</td> </tr> <tr> <td rowspan="2"><strong>리눅스</strong></td> <td colspan="1"><strong>7.2</strong> 이상</td> <td colspan="1">/home/username/Documents/Adobe/Adobe Substance 3D Painter</td> </tr> <tr> <td>레거시</td> <td colspan="1">/home/username/Documents/Allegorithmic/Substance Painter</td> </tr> </tbody> </table>

### 2 - 플러그인 폴더 생성

플러그인 이름은 상위 폴더의 이름을 기반으로 합니다.

이 예제에서는 플러그인 폴더 내에 **export-textures**&#x200B;이라는 이름의 새 폴더를 간단히 만듭니다.

### 3 - 플러그인 파일 만들기

새로 만든 폴더를 열고 다음 두 개의 빈 텍스트 파일(메모장)을 만듭니다.

* **main.qml**
* **toolbar.qml**

qml 파일 확장명은 Qt QML 언어용으로 작성된 스크립트용 Javascript 확장명입니다. 이를 통해 JavaScript 코드를 실행할 수 있을 뿐만 아니라 사용자 지정 UI도 만들 수 있습니다.

**main.qml** 파일은 필수 파일이며, 응용 프로그램에서 플러그인을 로드하기 위해 검색하는 첫 번째 파일입니다. 그러나 원하는 이름으로 추가 파일을 만들 수 있으므로 스크립트를 여러 부분으로 분할하여 보다 쉽게 관리할 수 있습니다. 이 경우 **toolbar.qml**&#x200B;은(는) 플러그인이 인터페이스에 추가할 버튼의 모양을 설명하는 데 사용됩니다.

### 4 - 스크립트 내용

스크립트 파일을 메모장++ 등의 텍스트 편집기로 열고 다음 코드 조각을 붙여넣습니다. 자세한 내용은 코드 주석을 참조하십시오.

**toolbar.qml**

```
import QtQuick 2.7 

import AlgWidgets 2.0 

import AlgWidgets.Style 2.0 

 

AlgButton 

{ 

 tooltip: "" 

 iconName: "" 

 text: "Export Textures" 

}
```


**main.qml**

```
// Default includes, to acces Qt/QML 

// and Substance 3D Painter APIs 

import QtQuick 2.7 

import Painter 1.0 

 

// Root object for the plugin 

PainterPlugin 

{ 

 // Disable update and server settings 

 // since we don't need them 

 tickIntervalMS: -1 // Disabled Tick 

 jsonServerPort: -1 // Disabled JSON server 

 

 // Implement the OnCompleted function 

 // This event is used to build the UI 

 // once the plugin as been loaded by Substance 3D Painter 

 Component.onCompleted: 

 { 

  // Create a toolbar button 

  var InterfaceButton = alg.ui.addToolBarWidget("toolbar.qml"); 

 

  // Connect the function to the button 

  if( InterfaceButton ) 

  { 

   InterfaceButton.clicked.connect( exportTextures ); 

  } 

 } 

 

 // Custom function called by the Button, 

 // this is the core of the plugin 

 function exportTextures() 

 { 

  // Catch errors in the script during execution 

  try 

  { 

   // Verify if a project is open before  

   // trying to export something 

   if( !alg.project.isOpen() ) 

   { 

    return; 

   } 

 

   // Retrieve the currently selected Texture Set (and sub-stack if any) 

   var MaterialPath = alg.texturesets.getActiveTextureSet() 

   var UseMaterialLayering = MaterialPath.length > 1 

   var TextureSetName = MaterialPath[0] 

   var StackName = "" 

 

   if( UseMaterialLayering ) 

   { 

    StackName = MaterialPath[1] 

   } 

 

   // Retrieve the Texture Set information 

   var Documents = alg.mapexport.documentStructure() 

   var Resolution = alg.mapexport.textureSetResolution( TextureSetName ) 

   var Channels = null 

 

   for( var Index in Documents.materials ) 

   { 

    var Material = Documents.materials[Index] 

 

    if( TextureSetName == Material.name ) 

    { 

     for( var SubIndex in Material.stacks ) 

     { 

      if( StackName == Material.stacks[SubIndex].name ) 

      { 

       Channels = Material.stacks[SubIndex].channels 

       break 

      } 

     } 

    } 

   } 

 

   // Create the export settings 

   var Settings = { 

    "padding":"Infinite", 

    "dithering":"disbaled", // Hem, yes... 

    "resolution": Resolution, 

    "bitDepth": 16, 

    "keepAlpha": false 

   } 

 

   // Build the base of the export path 

   // Files will be located next to the project 

   var BasePath = alg.fileIO.urlToLocalFile( alg.project.url() ) 

   BasePath = BasePath.substring( 0, BasePath.lastIndexOf("/") ); 

 

   // Export the each channel 

   for( var Index in Channels ) 

   { 

    // Create the stack path, which defines the channel to export 

    var Path = Array.from( MaterialPath ) 

    Path.push( Channels[Index] ) 

 

    // Build the filename for the texture to export 

    var Filename = BasePath + "/" + TextureSetName 

 

    if( UseMaterialLayering ) 

    { 

     Filename += "_" + StackName 

    } 

 

    Filename += "_" + Channels[Index] + ".png" 

 

    // Perform the export 

    alg.mapexport.save( Path, Filename, Settings ) 

    alg.log.info( "Exported: " + Filename ) 

   } 

  } 

  catch( error ) 

  { 

   // Print errors in the log window 

   alg.log.exception( error ) 

  } 

 } 

} 
```


완료하면 파일을 저장하고 닫습니다.

### 5 - 플러그인 불러오기 및 활성화

Substance 3D Painter을 시작하면 기본적으로 새로운 플러그인이 자동으로 로드되고 활성화됩니다.

프로젝트를 연 다음 플러그인에서 만든 UI 버튼을 클릭하여 현재 선택한 텍스처 세트의 채널을 내보냅니다.

![](../../assets/button-plugin.png)

플러그인을 활성화하거나 비활성화하려면 인터페이스 위쪽에 있는 Javascript 메뉴를 사용합니다.

![](../../assets/disable-plugin.png)
