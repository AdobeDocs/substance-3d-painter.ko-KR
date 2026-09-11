---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/pipeline-and-integration/resource-management/adding-resource-paths-by-editing-preferences-manually/editing-the-shelf-preferences-with-python.html"
breadcrumb-title: ''
description: 자동화된 리소스 경로 관리를 위해 Substance 3D Painter에서 Python 스크립팅을 사용하여 셸프 환경 설정을 편집하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Pipeline and integration > Resource management > Adding resource paths by editing preferences manually > Edit Shelf Preferences with Python
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Python을 사용하여 선반 환경 설정 편집
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 2%

---


# Python을 사용하여 선반 환경 설정 편집

다음은 리소스 경로를 조작하기 위해 Windows 레지스트리를 수정하는 예제 Python 스크립트입니다.

## 레지스트리 키 경로

적절한 레지스트리 키 경로를 사용하려면 아래 표를 참조하십시오.

<table data-preserve-html="true"> <colgroup> <col/> <col/> <col/> </colgroup> <tbody> <tr> <th>시스템</th> <th>버전</th> <th>경로</th> </tr> <tr> <td rowspan="2"><p><strong>Windows</strong></p><p>(레지스트리)</p></td> <td><strong>7.2</strong> 이상</td> <td>HKEY_CURRENT_USER\Software\Adobe\Adobe Substance 3D Painter</td> </tr> <tr> <td>레거시</td> <td>HKEY_CURRENT_USER\Software\Allegorithmic\Substance Painter</td> </tr> <tr> <td rowspan="2"><p><strong>Mac</strong></p><p>(라이브러리)</p></td> <td><strong>7.2</strong> 이상</td> <td>/Users/[사용자 이름]/Library/Preferences/com.adobe.Adobe Substance 3D Painter.plist</td> </tr> <tr> <td>레거시</td> <td>/Users/[사용자 이름]/Library/Preferences/com.substance3d.Substance Painter.plist</td> </tr> <tr> <td rowspan="2"><strong>리눅스</strong></td> <td><strong>7.2</strong> 이상</td> <td>/home/[사용자 이름]/.config/Adobe/Adobe Substance 3D Painter.conf</td> </tr> <tr> <td>레거시</td> <td>/home/[사용자 이름]/.config/Allegorithmic/Substance Painter.conf</td> </tr> </tbody> </table>

## 새 패스 추가

리소스 경로를 추가하려면 목록을 새 경로로 증가시키려면 이미 존재하는 경로를 확인해야 합니다.

다음 코드에서는 이미 정의된 경로의 현재 수를 확인한 후 레지스트리 키에 새 셸프 경로를 추가합니다.

>[!NOTE]
>
> 하위 키 **Shelf**(**pathInfos**&#x200B;과(와) 함께)가 레지스트리에 없을 수 있습니다. 응용 프로그램을 시작할 때 나타나게 하려면 환경 설정([편집] > [설정])을 연 다음 [확인]을 클릭하고 응용 프로그램을 닫습니다.

```
import winreg 

 

RegistryKeyName = "SOFTWARE\Adobe\Adobe Substance 3D Painter\Shelf\pathInfos" 

 

ShelfName = "myshelf" #Needs to be lowercase 

ShelfPath = "C:/Temp" 

ShelfStatus = "false" #false = not disabled 

 

RegConnection = winreg.ConnectRegistry( None, winreg.HKEY_CURRENT_USER ) 

  

## Open parent registry key

Key = winreg.OpenKey( RegConnection, RegistryKeyName, winreg.KEY_READ  ) 

 

## Iterate over each sub-key to retrieve the biggest Shelf number

SubKeyCount = winreg.QueryInfoKey( Key )[0] 

ShelfNumber = 0 

 

for x in range(SubKeyCount) : 

 SubKeyName = winreg.EnumKey(Key, x) 

 ShelfNumber = max( ShelfNumber, int(SubKeyName) ) 

 

ShelfNumber += 1 

 

## Create the new Key and add its values

NewKey = winreg.CreateKey( Key, str( ShelfNumber ) ) 

 

winreg.SetValueEx( NewKey, "disabled", 0, winreg.REG_SZ, ShelfStatus) 

winreg.SetValueEx( NewKey, "name", 0, winreg.REG_SZ, ShelfName) 

winreg.SetValueEx( NewKey, "path", 0, winreg.REG_SZ, ShelfPath) 

 

NewKey.Close() 

 

## Increment the Shelf path counter

Count = winreg.QueryValueEx( Key, "size" ) 

Key.Close() 

 

Key = winreg.OpenKeyEx( RegConnection, RegistryKeyName, 0, winreg.KEY_SET_VALUE  ) 

winreg.SetValueEx( Key, "size", 0, winreg.REG_DWORD, Count[0] + 1 ) 

Key.Close()
```


## 리소스 경로 비활성화 또는 활성화

생성된 모든 경로는 더 이상 필요하지 않으면 제거할 수 있지만 모두 제거할 수 없는 기본 경로에 대해서는 비활성화됩니다.

다음 코드는 Windows 레지스트리를 구문 분석하고 기본 셸프(&quot;starter\_assets&quot;로 이름 지정)를 비활성화합니다.

```
import winreg 

 

RegistryKeyName = "SOFTWARE\Adobe\Adobe Substance 3D Painter\Shelf\pathInfos" 

RegConnection = winreg.ConnectRegistry( None, winreg.HKEY_CURRENT_USER ) 

 

## Open registry key

Key    = winreg.OpenKey( RegConnection, RegistryKeyName, winreg.KEY_READ ) 

SubKeyCount  = winreg.QueryInfoKey( Key )[0] 

 

## Iterate over each sub-key

for x in range(SubKeyCount) : 

 SubKeyName = winreg.EnumKey(Key, x) 

 SubKey = winreg.OpenKey( 

  RegConnection, 

  RegistryKeyName + "\" + SubKeyName, 

  winreg.KEY_READ ) 

 SubKeyValueCount = winreg.QueryInfoKey( SubKey )[1] 

 

## Read subkey values

 Values = [] 

 for i in range( SubKeyValueCount ) : 

  Values.append( winreg.EnumValue( SubKey, i ) ) 

 

## Note : Values is a table of tuples

 FoundKey = False 

 for Value in Values : 

  if Value[0] == "name" : 

   if Value[1] == "starter_assets" : 

    FoundKey = True 

 

 SubKey.Close() 

 

## Found the path ? Then we edit the Key

 if FoundKey : 

  print( " - Editing Windows Registry" ) 

 

## Re-Open key in edition mode

  SubKey  = winreg.OpenKey(   

   winreg.HKEY_CURRENT_USER, 

   RegistryKeyName + "\" + SubKeyName, 

   0, 

   winreg.KEY_SET_VALUE ) 

 

## Assign new value

  winreg.SetValueEx(SubKey, "disabled", 0, 1, "true" ) #use "false" to Enable that shelf path 

 

  SubKey.Close() 

 

## Finish

Key.Close()
```
