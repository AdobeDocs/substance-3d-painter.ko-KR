---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/scripting-and-development/scripts-and-plugins/remote-control-with-scripting.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 원격 제어 스크립팅을 사용하여 작업 과정을 자동화하고 응용 프로그램을 프로그래밍 방식으로 제어하는 방법을 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Scripting and development > Scripts and plugins > Remote control with scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 스크립팅을 사용한 원격 제어
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# 스크립팅을 사용한 원격 제어

이 페이지에서는 Javascript 또는 Python 명령을 실행하기 위해 애플리케이션을 원격으로 제어하는 방법에 대해 설명합니다.\
이를 위해서는 특정 명령줄 인수가 필요하므로 간단한 Python 스크립트는 기존 Javascript 및 Python API에서 사용 가능한 모든 명령을 실행할 수 있습니다.

## 응용 프로그램 시작

응용 프로그램을 원격으로 제어하려면 다음 명령줄로 Substance 3D Painter을 실행해야 합니다.

```
"Adobe Substance 3D painter.exe" --enable-remote-scripting
```


>[!NOTE]
>
> 스크립트를 실행하기 전에 응용 프로그램이 이 명령으로 실행 중인지 확인하십시오. 애플리케이션이 여전히 시작 중이거나 아직 준비되지 않은 경우 스크립트가 실패할 수 있습니다.

## 원격 제어 스크립트

다음 Python 스크립트는 애플리케이션과 통신하는 라이브러리 역할을 할 수 있습니다.

다음 스크립트를 **lib\_remote.py** 파일에 저장하여 아래 예제가 제대로 작동하도록 합니다.

```
import sys 

import json 

import base64 

import subprocess 

 

if sys.version_info >= (3, 0): 

 import http.client as http 

else: 

 import httplib as http 

 

class RemotePainter() : 

 def __init__(self, port=60041, host='localhost'): 

  self._host = host 

  self._port = port 

 

## Json server connection

  self._PAINTER_ROUTE = '/run.json' 

  self._HEADERS = {'Content-type': 'application/json', 'Accept': 'application/json'} 

 

## Execute a HTTP POST request to the Substance Painter server and send/receive JSON data

 def _jsonPostRequest( self, route, body, type ) : 

  connection = http.HTTPConnection(self._host, self._port, timeout=3600) 

  connection.request('POST', route, body, self._HEADERS) 

  response = connection.getresponse() 

 

  data = response.read() 

  connection.close() 

 

  if type == "js" : 

   data = json.loads( data.decode('utf-8') ) 

 

   if 'error' in data: 

    OutJson = json.loads( body.decode() ) 

    print( base64.b64decode( OutJson["js"] ) ) 

    raise ExecuteScriptError(data['error']) 

  else : 

## Python can return nothing, so decoding can fail

   try: 

    data = data.decode('utf-8').rstrip() 

   except: 

    pass 

 

  return data 

 

 def checkConnection(self): 

  connection = http.HTTPConnection(self._host, self._port) 

  connection.connect() 

 

## Execute a command

 def execScript( self, script, type ) : 

  Command = base64.b64encode( script.encode('utf-8') ) 

 

  if type == "js" : 

   Command = '{{"js":"{0}"}}'.format( Command.decode('utf-8') ) 

  else : 

   Command = '{{"python":"{0}"}}'.format( Command.decode('utf-8') ) 

 

  Command = Command.encode( "utf-8" ) 

 

  return self._jsonPostRequest( self._PAINTER_ROUTE, Command, type ) 

 

class PainterError(Exception): 

 def __init__(self, message): 

  super(PainterError, self).__init__(message) 

 

class ExecuteScriptError(PainterError): 

 def __init__(self, data): 

  super(PainterError, self).__init__('An error occured when executing script: {0}'.format(data)) 

 
```


## 예

다음은 응용 프로그램에서 지원하는 두 API에서 명령을 실행하는 방법을 보여 주는 두 가지 간단한 예입니다.

### Javascript 명령 실행

API의 대부분의 Javascript 함수는 Python 스크립트 내에서 쉽게 조작할 수 있는 String 또는 Json 데이터를 반환합니다. 데이터를 주고받는데 큰 문제가 없어야 한다.

이름이 **example\_js.py**&#x200B;인 python 스크립트 파일을 만들고 다음 코드를 추가합니다.

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## Print the API version

Version = Remote.execScript( "alg.version.painter", "js" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library:

Files = Remote.execScript( 'alg.resources.findResources("starter_assets", "*")', "js" ) 

 

for File in Files : 

 print( File )
```


응용 프로그램이 명령줄을 사용하여 실행 중인 경우 이 스크립트를 실행하면 명령이 실행되고 해당 결과가 검색됩니다.

### 파이썬 명령 실행

대부분의 Python 함수는 원격 스크립트로 전달할 수 없는 개체를 반환할 수 있으며, 이는 데이터를 받기 위해 명시적으로 문자열 또는 Json 사전으로 변환해야 한다는 것을 의미합니다.

응용 프로그램 시작 중에 로드되는 사용자 지정 python 스크립트를 만들거나 인라인 변환에 의존하지 않고도 이러한 종류의 변환을 처리하는 호출 함수를 만들 수 있습니다.

이름이 **example\_py.py**&#x200B;인 python 스크립트 파일을 만들고 다음 코드를 추가합니다.

```
import lib_remote 

 

Remote = lib_remote.RemotePainter() 

Remote.checkConnection() 

 

## import the substance_painter module to make

## its API available to us

Remote.execScript( "import substance_painter", "python" ) 

 

## Print the API version

Version = Remote.execScript( "substance_painter.__version__", "python" ) 

print( Version ) 

 

## Get a list of all the files in the default shelf/library

## Because the search function return objects, we have to convert

## the information into a string within the same command (inline)

Command = 'substance_painter.resource.search( "p:starter_assets/" )' 

Command = '"|||".join( [ x.identifier().url() for x in {0}] )'.format( Command ) 

 

Files = Remote.execScript( Command, "python" ) 

Files = Files.split( "|||" ) 

 

for File in Files : 

 print( File )
```


응용 프로그램이 명령줄을 사용하여 실행 중인 경우 이 스크립트를 실행하면 명령이 실행되고 해당 결과가 검색됩니다.
