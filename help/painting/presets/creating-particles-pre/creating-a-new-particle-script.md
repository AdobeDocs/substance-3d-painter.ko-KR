---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/painting/presets/creating-particles-presets/creating-a-new-particle-script.html"
breadcrumb-title: ''
description: Substance 3D Painter에서 새 입자 스크립트를 만들어 사용자 정의 입자 브러시 비헤이비어 및 효과를 정의하는 방법에 대해 알아봅니다.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Creating A New Particle Script
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 새 입자 스크립트 만들기
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---


# 새 입자 스크립트 만들기

사전 설정된 PokinFX 패키지 다운로드: [Templates\_EmitterReceiver.pkkg](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/spdoc/files/67403778/68419585/1/1411557944000/templates-emitterreceiver.pkkg)

이 패키지는 Substance 3D Painter에서 편집하고 가져올 방출기와 수신기가 포함된 &quot;시작 키트&quot;입니다.

## 팝콘 FX 설정

팝콘FX 편집기를 실행하고 새 프로젝트를 만든 다음 엽니다.

프로젝트에서 빈 영역을 마우스 오른쪽 버튼으로 클릭하고 &quot;팝콘 패키지 가져오기&quot;를 선택합니다. 그런 다음 &quot;Templates\_EmitterReceiver.pkkg&quot;를 선택합니다.

이제 다음을 수행해야 합니다.

* 파티클 시스템 &quot;\_Emitter&quot;는 Emitter의 기본 템플릿입니다.
* Receiver의 기본 템플릿인 파티클 시스템 &quot;\_Receiver&quot;
* 구 메쉬가 장면의 기본 배경으로 사용됩니다.

&quot;\_Emitter&quot; 및 &quot;\_Receiver&quot;는 이미 &quot;Painter ready&quot;입니다. 그들은 이미 필요한 진화자, 필드, 배경 등으로 구성되었습니다.

## 메시 가져오기

팝콘FX는 **FBX**&#x200B;만 지원합니다. 메시를 이 형식으로 내보내야 합니다. 내보내기 단계에서 메시 크기를 확인하여 &quot;실제&quot;의 올바른 단위에 맞춥니다.

프로젝트의 &quot;망&quot; 폴더에 복사하여 붙여 넣습니다(PostonFX에서 &quot;망&quot; 폴더를 마우스 오른쪽 버튼으로 클릭하고 &quot;파일 위치 열기&quot;를 선택).

편집기로 돌아와서 메시를 열고(두 번 클릭) &quot;**빌드**&quot;를 클릭합니다. 창을 닫고 변경 사항을 저장합니다.

## 이미터/수신기 편집

우리는 기존의 입자 시스템을 복제하고 새로운 메쉬를 올바르게 고려하도록 적응시킬 것이다.

&quot;Particles&quot; 폴더에서 입자 시스템 &quot;\_Emitter&quot;를 마우스 오른쪽 단추로 클릭하고 &quot;복제&quot;(또는 &quot;복제&quot;)를 선택하여 자체 이미터를 만듭니다.

이 파일을 열고 &quot;Particle Treeview&quot; 창(왼쪽 아래)에서 &quot; **Layer\_Model** &quot;을(를) 선택합니다. 이 모델은 &quot;Editor Properties => Backdrop => 3D Layers&quot; 위치에 있어야 합니다.

그런 다음 &quot;Node Properties&quot; 창에서 &quot;dummymesh.fbx&quot;를 모델로 바꿉니다. 수정 내용을 저장하고(파일 => 저장) 이미터 창을 닫습니다.

이제 **&quot;\_Receiver** **&quot;**(&quot;Particles&quot; 폴더에서)을(를) 복제하여 이 폴더에서 자체 수신기를 만드십시오.

연 다음 방출기에서 더미 메시를 &quot;Layer\_Model&quot;의 모델로 바꿉니다. **화면에 표시된** **메시를 수정했습니다**. 그러나 **파티클이 사용한** **메시**&#x200B;도 수정해야 합니다.

그렇게 하려면 &quot;입자 트리 보기&quot; 창에서 &quot; **모양**&quot;을 클릭합니다. 위치: &quot;입자 효과 => 스패너 => 레이어\_1 => 샘플러 => 메시&quot;

그런 다음 &quot;MeshResource&quot;를 모델로 바꿉니다.

작업이 완료되면 마지막으로 해야 할 일이 있습니다. 송신기와 수신기를 방금 만든 송신기와 &quot;연결&quot;해야 합니다.

수신기의 트리 보기에서 &quot;편집기 속성&quot;을 선택한 다음 &quot;OverSpawnEffect&quot;에서 에미터를 선택합니다. 수신기를 저장하십시오.

방출기(이전에 복제한 것)를 열고 &quot;입자 트리 보기&quot; 창에서 &quot;이벤트&quot;를 클릭합니다. 이벤트 위치는 &quot;입자 효과 => Spawner&quot;입니다. 그런 다음 &quot;외부&quot;를 클릭하여 수신기를 수신기로 교체하십시오.\
완료되었습니다! 이제 3D 보기(이미터 또는 수신기)를 선택하는 경우 &quot;공간&quot; 버튼을 눌러 입자를 만들 수 있습니다.

## 선택 사항: 수신기 동작 수정

수신기를 열고 &quot;Particles Treeview&quot; 창에서 &quot; CParticleEvolver\_Script &quot; (본인 전용 상단 스크립트 :)&quot;를 선택합니다. 이 스크립트 위치는 &quot;Particle Effect => Layer\_1 => State\_0&quot;이어야 합니다.

&quot;특수 노드 편집기&quot; 창에서 함수에서 &quot;Life = 0.5;&quot;을 추가하여 파티클 수명을 변경합니다. 그런 다음 &quot;Ctrl+s&quot; 단축키를 사용하여 스크립트를 저장합니다. 3D 보기의 차이를 확인할 수 있어야 합니다.

작동 방식에 대한 자세한 내용은 아래 링크를 참조하십시오.

<http://wiki.popcornfx.com/index.php/Main_Page>

## Substance 3D Painter에서 이미터/수신기 가져오기

Substance 3D Painter에서 &quot;파일&quot; > &quot;파티클 가져오기&quot; 또는 Ctrl-Alt-R을 누른 다음 팩에서 이미터 및 수신기(모두 .pkfx 형식)를 선택합니다.

Substance 3D Painter은 요구 사항(입자 필드, OnCollize 이벤트)을 자동으로 감지하여 pkfx가 이미터, 수신기인지 아니면 호환되지 않는지 결정합니다.

이제 선반에 있는 이미터 / 리시버를 &quot;이미터&quot;와 &quot;리시버&quot; 탭에서 볼 수 있습니다.

이를 사용하려면 먼저 &quot;파티클 토글&quot; 버튼을 클릭해야 합니다.

그런 다음 &quot;도구&quot; 창의 &quot;물리학&quot;에서 이미터(&quot;기본\_이미터&quot; 대체)와 수신기(&quot;기본\_수신기 대체)를 선택할 수 있습니다.

이제 &quot;도구&quot; 창을 마우스 오른쪽 버튼으로 클릭하고 도구를 저장할 수 있습니다.
