---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/painting/presets/creating-particles-presets/overview-of-the-particle-editor.html"
breadcrumb-title: ''
description: Substance 3D Painter의 입자 편집기를 사용하여 텍스처 페인팅을 위한 사용자 정의 입자 브러시 사전 설정을 만드는 방법을 살펴보세요.
helpx_creative_field: ""
helpx_description: Painter > Painting > Presets > Creating particles presets > Overview of the particle editor
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 입자 편집기 개요
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 0%

---


# 입자 편집기 개요

이 페이지에서는 팝콘FX 입자 편집기의 여러 측면에 대해 다룹니다. 일부 창 제목 및 매개 변수는 사용된 편집기의 버전에 따라 변경될 수 있습니다.

## 뷰포트 설정

### 나만의 메쉬를 가져오는 방법

팩의 &quot;메시&quot; 폴더에 메시를 복사하여 붙여넣습니다. 그런 다음 편집기에서 메시를 열고 &quot;빌드&quot;를 클릭합니다.

이제 입자 시스템에서 트리 뷰에서 &quot;Backdrop&quot;으로 이동하고 &quot;3D Layers&quot;, &quot;New Backdrop&quot;, &quot;CNEdEditorBackdrop\_Model3D&quot;를 마우스 오른쪽 버튼으로 클릭한 다음 &quot;Resource Model&quot;에서 메쉬를 선택합니다.

Substance 3D Painter에서 메쉬는 각 축의 크기가 [-1;1]인 상자 안에 오도록 비율이 조정됩니다. [편집기]에서 Substance 3D Painter을 사용하여 적절한 배율을 조정하려면 이미 해당 상자에 맞게 배율이 조정된 메시를 (쉬운 방법으로) 가져오거나 [편집기]에서 배율을 사용해야 합니다.

참고: FBX 메시 형식만 지원됩니다.

#### 그리드 표시 방법

Ctrl-G. &quot;편집기 속성&quot; &quot;GridColor&quot;에서 그리드의 색상을 사용자 정의할 수 있습니다.

## 이미터

### &quot;OnColare&quot; 이벤트 생성 방법

피직스 에벌버는 장면의 배경 메시와의 충돌을 처리합니다. Substance 3D Painter에서 장면은 메쉬가 됩니다.

물리학의 첫 번째 진화는 &quot;WorldInteractionMode&quot;를 &quot;OneWay&quot;로 설정하여 입자 충돌을 가능하게 합니다. 그런 다음 &quot;OnCollize&quot;라는 이벤트를 만들면 물리학 진화기가 장면과 충돌하면서 이를 트리거합니다.

Substance 3D Painter에서 장면은 작업 중인 모델이며, &quot;OnCollare&quot;라는 모든 이벤트는 현재 브러시의 이미터 입자 시스템에 의해 재정의됩니다.

#### 카메라에서 파티클을 발사하는 방법

뷰 포트 상단에서 네 번째 버튼 &quot;카메라 평면에 생성 제한&quot;을 활성화합니다.

Substance 3D Painter은 기본적으로 카메라에서 방출기를 비춥니다.

#### 어떻게 위에 비처럼 입자를 내뿜는가

활성화된 경우 &quot;카메라 평면에서 생성 제한&quot;을 비활성화합니다.

&quot;전역&quot;이라는 입자 특성을 만들면 이제 Substance 3D Painter에서 입자를 원점에 생성합니다.

메쉬 상단에 산란을 하려면 모양 Sampler BOX 또는 CYLINDER를 추가하고 그 위에 놓은 다음 [산포 스크립트]에서 샘플링합니다.

예를 들어 &quot;Spawn&quot;이라는 [모양] Sampler 상자를 사용하여 이를 Spawner Script에 추가합니다.

*위치 = Spawn.samplePosition();*

## 수신기

### 수신기를 만들거나 편집하는 동안 에미터를 만드는 방법

수신기를 편집하는 동안 Substance 3D Painter 작업 과정에 더 가까이 다가가기 위해 만든 파티클 시스템을 재정의하도록 [편집기]를 설정할 수 있습니다.

수신기의 트리 보기에서 &quot;Editor Properties&quot;를 선택한 다음 &quot;UserOverSpawn&quot;을 활성화하고 &quot;OverSpawnEffect&quot;에서 에미터를 선택합니다.

&quot;OnColare&quot; 이벤트가 현재 편집 중인 수신기를 생성하도록 하려면 아직도 Emitter를 열어야 합니다.

#### 입자 필드를 설정하는 방법

다음은 수신자에게 있어야 할 입자 필드에 대한 설명입니다.

*&quot;Size&quot; float*

Substance 3D Painter에서 브러시 크기의 곱자입니다.

*&quot;불투명도&quot; 부동*

Substance 3D Painter에서 브러시 불투명도의 곱자입니다.

*&quot;UV&quot; float3*

입자 메쉬의 텍스처 좌표입니다.

Evolver 스크립트에서 투영 Evolver가 제공한 파라메트릭 좌표를 사용하여 모양 Sampler &quot;메쉬&quot;를 샘플링합니다.

UV = Mesh.sampleTexcoord(pCoords);

*&quot;표준&quot; float3*

입자 아래 메쉬 표면의 법선입니다.

Evolver 스크립트에서 투영 Evolver가 제공한 파라메트릭 좌표를 사용하여 모양 Sampler &quot;메시&quot;를 샘플링합니다.

Normal = normalize(Mesh.sampleNormal(pCoords));

*&quot;시드&quot; int*

Substance 3D Painter에 대해 임의로 생성된 값:

Evover 스크립트에서 다음을 추가합니다.

시드 = int(rand(0,20000000));

*&quot;pCords&quot; int3*

Substance 3D Painter에서 사용하지 않지만 메쉬 상에서 입자 투영을 수행하고 다른 필드를 샘플링하는 데 없어서는 안 됩니다.

#### 메쉬에 입자를 투영하는 방법

수신기의 &quot;State\_0&quot;에 Projection Evolver를 추가합니다.

각 프레임에서 투영 이볼버는 모양 Sampler의 가장 가까운 표면에 입자를 투영합니다.

투영 이볼버는 &quot;OutputParametricCoordsField&quot;에 의해 지정된 입자 필드에 투영의 파라메트릭 좌표를 채울 수 있습니다(&quot;pCoords&quot; 입자 필드 참조).

또한 &quot;ReprojectedField&quot;를 사용하여 메시 표면에 벡터를 다시 투사할 수 있습니다.

여기서는 Sampler 모양 &quot;망&quot;에 입자를 투영하고 int3 입자 필드 &quot;pCoords&quot;에서 파라메트릭 좌표를 채우고 표면에도 &quot;속도&quot;를 투영합니다.

#### 메쉬를 샘플링하는 방법

Substance 3D Painter에서 &quot;Mesh&quot; 및 &quot;ShapeType&quot; &quot;MESH&quot;라는 모든 모양 샘플러는 Substance 3D Painter에서 사용되는 메쉬로 재정의됩니다.<b>\
</b>

[편집기]에서 배경과 같은 메시로 설정합니다.

스크립트에서 사물을 샘플링하려면 스크립트에 &quot;Mesh.sample~Something~(pCoords)&quot;이라고 쓰면 됩니다. 이 설명서는 다음과 같습니다.

<https://wiki.popcornfx.com/index.php/CParticleSamplerShape#Script_bindings>

몇 가지 유용한 코드 조각:

```
// UV is the texture coordinate of the particle on the mesh

// Must be after CParticleEvolver_Projection

UV = Mesh.sampleTexcoord(pCoords);

// Normal is the Normal of the surface on the mesh just below the particle

// Must be after CParticleEvolver_Projection

Normal = normalize(Mesh.sampleNormal(pCoords));
```


## 일반 팁

### Substance 3D Painter에서 이미터/수신기를 가져오는 방법

Substance 3D Painter에서 &quot;파일&quot; > &quot;파티클 가져오기&quot; 또는 Ctrl-Alt-R을 누른 다음 팩에서 Emitter.pkfx 또는 Receiver.pkfx를 선택합니다.

Substance 3D Painter은 요구 사항(입자 필드, OnCollize 이벤트)을 자동으로 감지하여 pkfx가 이미터, 수신기인지 아니면 호환되지 않는지 결정합니다.

이제 선반에 이미터/수신기가 표시됩니다.

#### 실행 가능한 입자 크기로 입자를 디버깅하는 방법

Substance 3D Painter에서 브러시 크기의 승수가 되려면 &quot;크기&quot; 입자 필드가 0에서 1 사이여야 하므로 편집기에서 입자가 너무 클 수 있습니다. 따라서 Billboard Particle Renderer에서 입자를 더 잘 보기 위한 &quot;SizeField&quot;로 사용할 사용자 정의 필드 부동 소수점 &quot;BBSize&quot;를 스패너 스크립트에서 0.01로 추가합니다.

#### 진화 주문을 망치지 않는 방법

진화의 순서는 매우 중요할 수 있다.

예를 들어, 두 개의 마지막 이볼버를 항상 투영 이볼버로 지정하고 스크립트 이볼버로 지정하여 투영 이볼버에서 생성된 pCoords로 UV 및 Normal을 샘플링할 수 있습니다.

진화하는 사람의 순서는 문자 그대로 프레임 내에서 실행되는 순서라는 점을 명심하고 Substance 3D Painter은 입자 필드 값과 각 프레임의 끝을 수집합니다.

#### 메시 노멀 맵 샘플링 방법

Substance 3D Painter은 &quot;NormalMap&quot;이라는 모든 텍스처 샘플러를 메쉬 노멀 맵(가져온 경우)로 대체합니다.

현재 보유할 수 있는 유일한 텍스처로, Substance 3D Painter에서 다른 모든 텍스처에 액세스할 수 없습니다.

&quot;NormalMap&quot;이라는 텍스처 Sampler을 추가한 후 스크립트에서 샘플링할 수 있습니다.

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerTexture>

몇 가지 유용한 코드 조각:

```
// In Evolver Script convert the NormalMap texture in tangent space to world space normal

// /!\ the "Normal" particle field must always be the normal of the mesh not influenced by the normal map

// /!\ dont forget to initialize your particle fields in your Spawn Script

// otherwise pCoords and Normal will be invalid at the first update

float normalFactor = 1.0; // change the intensity of the normal map

float3 meshnormal = Normal;

float4 rawtangent = Mesh.sampleTangent(pCoords);

float3 binormal = normalize(cross(meshnormal, rawtangent.xyz) * rawtangent.w);

float3 tangent = normalize(cross(meshnormal, binormal));

float3 tsNormal = normalize(((NormalMap.sample(UV).xyz * 2.0 - 1.0).xyz) * float3(-normalFactor, normalFactor, 1));

float3 normal = normalize(tsNormal.x * tangent + tsNormal.y * binormal + tsNormal.z * meshnormal);
```


#### 난기류를 만드는 방법

[편집기]에서 Turbulence Sampler 를 만듭니다.

<http://www.popcornfx.com/wiki/index.php/CParticleSamplerProceduralTurbulence>

그런 다음 난류를 샘플링하여 입자에 영향을 주는 두 가지 방법을 사용할 수 있습니다.

##### 쉬운 방법

레이어의 Physics Evolver에서 &quot;VelocityFieldSampler&quot;를 Turbulence Sampler 이름으로 설정하고 &quot;Drag&quot;를 0 이상의 값으로 설정합니다.

##### 매개 변수가 있는 방법

Evover Script에서 Turbulence Sampler으로 생성된 속도 필드를 샘플링하여 속성으로 난류를 조정합니다.

2개의 입자 속성을 만듭니다.

* float &quot;TurbulencePower&quot; minmax: [0;5]
* float &quot;TurbulenceScale&quot; minmax: [0.001; 5] (0보다 커야 함)

그런 다음 3개의 입자 필드를 만듭니다.

float &quot;TurbPower&quot; 및 float &quot;TurbScale&quot;

속성을 [스패너 스크립트]에 저장하려면 다음과 같이 하십시오.

* TurbScale = 1.0 / TurbulenceScale;
* TurbPower = TurbulencePower;

float3 회전 모드의 &quot;VelocityField&quot;

이 필드는 Physics Evover에서 &quot;VelocityField&quot; 로 사용됩니다 ( 이미 &quot; VelocityField&quot; 필드로 기본 설정됨 ).

따라서 물리학이 진화하기 전에, 스크립트 진화자에서 &quot;뒤틀기&quot;라고 불리는 난기류 Sampler을 샘플링합니다.

VelocityField = Turb.sample(위치 \* TurbScale) \* TurbPower;

#### Dt, 델타 시간을 올바르게 사용하는 방법

델타 시간은 각 프레임 업데이트 간의 시뮬레이션 시간(초)입니다. 편집기에서 델타 시간은 실제 경과 시간으로 업데이트됩니다. Substance 3D Painter에서는 델타 시간이 수정되며 마지막 업데이트가 완료되는 즉시 각 업데이트가 실행됩니다.

60FPS로 실행되는 게임의 델타 시간은 1/60= 0.016초이므로 브러시가 델타 시간의 0.016초 전후로 실행되도록 하십시오.

* 큰 델타 시간 > 0.016s
* PRO 빠른 업데이트

업데이트 사이의 시간이 크면 파티클의 이동이 더 커지므로 Substance 3D Painter에서 브러시가 더 빠르게 실행됩니다.

* 콘 어림

팝콘FX는 일종의 큰 이산화 시스템이기 때문에 dt가 클수록 더 큰 절상을 하게 된다. 난류에 대한 큰 델타 시간 의미를 확인합니다. <http://www.popcornfx.com/wiki/index.php/CParticleEvolver_Physics#Dealing_with_turbulences_at_low_framerates>

* 콘 스플릿

델타 시간이 크면 프레임 간의 입자 이동도 커집니다. 따라서 Substance 3D Painter에서는 직선 대신 작은 얼룩이 표시될 수 있습니다.

이 오류는 Substance 3D Painter이 각 프레임의 끝에 각 파티클에 대해 한 개의 선 포인트를 그리고 마지막 프레임과 현재 타임라인 사이에 각 파티클에 대해 선을 그리지 않기 때문에 발생합니다.

* 델타 시간이 거의 없음 &lt; 0.016s
* PRO 정밀도

델타 시간이 작을수록 브러시 획 사이의 거리가 짧아지고 드로잉이 더 선명해집니다. 그리고 시뮬레이션의 이산화도 더 좋을 것이다.

* 콘 슬로우

델타 시간이 작을수록 동일한 거리 거리를 그리는 데 더 많은 업데이트가 필요합니다.

델타 시간에 대한 최종 팁 : 오른쪽 dt를 얻는 좋은 방법은 큰 값(0.1s)으로 시작한 다음 단계별로 줄여서 원하는 결과를 얻는 것입니다.

#### 입자 시스템의 매개변수를 표시하는 방법

Substance 3D Painter은 입자 시스템의 입자 특성을 수집하여 물리적 브러시 매개 변수에 표시합니다.

<http://www.popcornfx.com/wiki/index.php/Particle_effect_attributes>

팝콘FX에는 Evolve 스크립트의 속성에 액세스할 수 있도록 하는 &quot;Attributes in Evolve&quot;라는 기능이 있습니다. 이를 수행하지 마십시오 . 대신 입자 필드를 만들고 [Spawner Script]에 특성을 저장한 다음 [Evobler Scripts]에서 해당 입자 필드를 사용합니다. (나중에 수정할 수 있음)

#### 문제가 있는 입자를 감지하는 방법

당신은 이상한 입자 필드 값을 가진 입자를 가지고 있어서는 안 된다, 그래서 당신은 때때로 문제가있는 것을 탈피할 수 있다:

<http://www.popcornfx.com/wiki/index.php/Particle_tips_BreakOnProblematicParticle>

#### Substance 3D Painter에서 입자 시스템 문제를 해결하는 방법

Substance 3D Painter 설치 디렉토리에서 &quot;팝콘.htm&quot;이라는 파일을 찾을 수 있습니다. 이 파일에는 팝콘FX의 모든 로그가 포함되어 있으며, 내부를 살펴보아 어떤 문제가 발생할 수 있는지 확인하십시오.

#### 입자 필드를 올바르게 초기화하는 방법

첫 번째 프레임에서 유효한 UV 및 [표준]을 얻으려면 이를 [스패너 스크립트]에 추가하십시오.

<b>  
</b>

```
// PostEval() will be called after particles have been translated to their respective spawn locations

// so, PostEval() is executed in world space

function void PostEval()

{

// we need to initialize correctly the values needed by Substance 3D Painter:

pCoords = Mesh.projectParametricCoords(Position);

UV = Mesh.sampleTexcoord(pCoords);

Normal = normalize(Mesh.sampleNormal(pCoords));

}
```
