---
helpx_url: "https://helpx.adobe.com/kr/substance-3d-painter/release-notes/know-issues.html"
breadcrumb-title: ''
description: Substance 3D Painter에 대해 알려진 문제를 검토하여 현재 제한 사항 및 해결 방법에 대해 최신 버전을 통해 최신 정보를 확인하십시오.
helpx_creative_field: ""
helpx_description: Substance 3D Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 알려진 문제
user-guide-description: ''
user-guide-title: ''
source-git-commit: 50df3a58ec4719d302999421774a1c67ce3e0ef1
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---


# 알려진 문제

이 페이지에는 Substance 3D Painter v12.1.3에 있는 알려진 모든 문제가 나열됩니다.

* `[Baking]` 단순 큐브의 AO가 잘못되었습니다.
* `[Baking]` 이름 접미사 일치가 잘못되었습니다.
* mes 다시 가져오기 후 `[Baking]`개의 Uv 솔기가 나타나지 않습니다.
* 일부 설정이 포함된 격자 모양 아티팩트 `[Baking]`개
* `[Baking]` 앰비언트 오클루전 메쉬 이름으로 백페이스 무시 기능이 작동하지 않음
* `[Baking]` `[AMD]` 높은 폴리 메쉬로 굽는 동안 장치 손실

* `[Substance]` 리소스 맞춤법 오류
* `[Substance]`개의 공백은 가시성을 위한 조건을 나눕니다.
* 일부 재질에 대한 `[Substance]` 사전 설정을 불러오는 데 너무 오래 걸림
* `[Substance]`이(가) 혼합 사용과 함께 리소스를 가져올 수 없습니다.

* 텍스처 집합에 타일 1001이 없는 경우 스마트 재질을 사용할 때 `[Engine]` 오류가 발생합니다.
* `[Engine]` 일반 채널 이동 색상에서 복제 도구를 사용하여 페인팅이 잘못됨
* `[Engine]` 모양 마스크가 인스턴스화된 레이어가 있는 UV 테두리에 아티팩트를 표시합니다.

* `[Color Management]` 호환되지 않는 바인딩과 생성기가 마스크에 사용되지 않습니다.
* `[Color Management]` 필터 출력이 제대로 고려되지 않음
* Linux에서 ACE를 사용한 `[Color Management]` HDR 색상 공간 변환은 클램프된 색상을 생성합니다.

* `[Shelf]` 리소스를 특정 이름의 폴더에 배치하면 잘못된 사용이 발생합니다.
* `[Shelf]` `[Substance]` 사용자 데이터가 셸프 축소판 생성을 고려하지 않음

* `[Shader]` &quot;camera_vp_matrix_inverse&quot; 매개 변수를 인식할 수 없습니다.
* `[Shader]` user0 채널은 항상 특정 셰이더를 사용하여 sRGB로 읽을 수 없습니다.

* 내보내기 함수에서 디더링 매개 변수를 지정할 때 `[Scripting]` `[Javascript]` 오타가 &quot;해제됨&quot;
* `[Scripting]` `[Python]` substance_painter.project 모듈의 다양한 오타

* `[USD]` 경우에 잘못된 usda 할당이 있습니다.
* 내보낸 USD 기하학이 UV 테두리를 따라 밀어넣음`[USD]`

* 기본 색상 보기에 저장된 `[Single Channel View]` 프로젝트가 Painter 버전 업데이트 후 더 어둡게 보입니다.
* 기본 색상 보기에 저장된 `[Single Channel View]` 프로젝트가 Painter 버전 업데이트 후 더 어둡게 보입니다.

* `[gltf]` Babylon 내보내기 도구를 통해 내보낸 파일을 열 수 없습니다.
* 페인팅 시 `[Displacement]` 결함
* `[Polygon Fill Tool]` 대칭이 있는 잘못된 선택
* 페인팅 시 `[2D view]`개의 선이 나타나지 않는 경우가 있습니다.
* 단축키와 연결된 `[Console]` 기호를 쓸 수 없습니다.
* `[LOG]` 내보내기 실패 시 오류 메시지가 잘못됨
* `[3D View]` 스텐실이 복제된 개체에서 작동하지 않습니다.
* `[Resource updater]` 셸프에 있는 같은 이름의 다른 리소스가 하나의 리소스로 읽혀집니다.
* 미리 보기 샘플에서 `[Sample]`개의 끊어진 카메라
* `[Instancing]` `[Projection]` 평면 프로젝트에서 인스턴스를 선택하면 다른 텍스처 세트에서 다른 평면 프로젝트가 선택됩니다
* 커서가 창에서 나가면 `[Slider]` 숫자 입력이 선택 해제됨
* 마스크 콘텐츠를 복사하여 붙여넣을 때 `[Anchor point]`개의 끊어진 참조
* `[Mesh export]` 새 텍스처 집합 이름을 고려하지 않음
* `[Anchor Points]` 생성기에서 사용할 때 색상이 잘못되었습니다.
* `[Bakers]` ID 맵 제빵사는 3ds Max 2021 실제 재질을 고려하지 않습니다.
* `[UV Tiles]` 특정 메시로 겹치는 UV 공간에 오류 메시지가 없습니다.
* `[GLTF]` `[Crash]` 압축된 gltf 파일로 프로젝트를 만들면 충돌이 발생합니다
* `[UV Tile sequence]` 위치 맵을 올바르게 가져오지 못했습니다.
* `[UVTiles]` Height 조합 마스크가 UV 타일 마스크로 새로 고쳐지지 않음
* `[Import]`에서 &quot;nan&quot; 값이 있는 obj 파일을 가져올 수 없습니다.
* `[Export]` GLTF 내보내기의 크기가 잘못되었습니다.
* `[Texture Set]` 이름은 비워 둘 수 있습니다.
* `[Layer stack]` 재질 모드로 마스크 전환 복사
* 브러시 메이커 설정의 `[UI]` 오타
* `[Texture Set Settings]` 이름 변경 후 셰이더 인스턴스 이름이 잘못되었습니다.
* `[Blending]` 색상 및 채도 혼합 모드도 밝기 변경
* 경로 창별 저장된 검색 및 필터의 `[Librairies]` 너비가 변경되었을 때 저장되지 않음
* 메시 및 인스턴스 레이어를 다시 가져올 때 `[Geometry mask]` 문제
* 타일 1001이 없는 경우 `[Color management]` 색상 공간을 찾을 수 없습니다.
* 특정 UV 타일이 설정된 상태에서 `[Export mesh]` 변위를 내보내지 못했습니다.
* `[RedHat]` 색상 피커 문제
* `[Regression]` `[UI]` 마우스 오른쪽 클릭 메뉴가 hd 화면에서 너무 작습니다.
* `[Resources]` 가져온 메시 맵이 자동 업데이트에서 무시됩니다.
* `[User Channels]` 색상 혼합 공간 미리 보기가 잘못되었습니다.
* 베이크 모드로 전환한 후 `[Mask]` 도형 선택이 여전히 활성 상태입니다.
* `[Sonoma]` 아이콘이 메뉴에 나타나지 않습니다.
* `[Path]` Height이 여러 경로를 혼합하면 아티팩트가 발생할 수 있습니다.
* `[Polygon Fill]` 기본 색상의 색상 공간을 변경해도 색상 피커가 업데이트되지 않습니다.
* 내보낼 때 텍스처를 4k에서 8k로 업스케일할 때 `[UV Padding]`개 아티팩트
* `[Performances]` Painter이 VRAM 사용을 호스팅함
* `[Generator]` &quot;텍스처 사용&quot;을 false로 설정해도 텍스처 입력의 사용이 비활성화되지 않습니다.
* 정사각형이 아닌 리소스는 브러시 채널의 슬롯에서 사용할 때 늘어납니다.
* Substance를 디코딩하지 못했습니다.
* 완벽하게 겹치지 않는 UV는 가공물을 만들 수 있습니다
* 일부 fbx가 있는 메시 표준이 잘못되었습니다.
* 수준의 영향을 받는 채널을 변경할 때 보기가 업데이트되지 않음
* 하나의 텍스처가 설정된 프로젝트가 기본 색상 솔로 모드에서 다시 열립니다
* 재질/페인트 속성에서 채널 버튼의 UI가 깨질 수 있음
* 속성의 채널 순서가 손상될 수 있음
* L16F 및 RBG16F로 만든 획은 가공물을 표시할 수 있습니다
* 복원 단추 동작이 카메라 설정의 잠금 키와 상호 작용하지 않음
* Photoshop 내보내기는 모양 마스크 선택을 무시합니다
* 흐림 효과 경사 및 뒤틀기 필터는 텍스처 설정 해상도에 따라 다름
* 이름이 없는 맵은 내보내기 폴더 외부에 생성됩니다.
* 브러시 사전 설정을 변경할 때 스텐실이 업데이트되지 않음
* PSD 파일의 투명도 문제
* 상황별 도구 모음에서 수정한 브러시 매개 변수가 기록에 표시되지 않음
* 이 세션에서 이미 삭제했다가 다시 만든 내보내기 사전 설정의 이름은 바꾸거나 삭제할 수 없습니다
* 경우에 따라 투영 도구 미리 보기에 대해 채널 매핑이 작동하지 않습니다
* 3D 투영 편집 중 저장 시 뷰포트 고정
* 재질 레이어 해상도가 너무 낮음

## 안정성

* `[Crash]` 프로젝트를 만들지 못한 후 텍스처 집합 목록을 클릭하면 충돌이 발생합니다
* `[Crash]` 동일한 프로젝트가 두 번 열려 있을 때 심각한 오류가 발생했습니다.
* `[Crash]` 메시를 로드하지 못한 경우 &quot;메시 내보내기&quot;를 선택합니다
* `[Crash]` 이전 프로젝트를 연 후 &quot;페인팅 시작&quot;을 클릭
* `[Crash]` 리본에서 매우 긴 텍스트를 만들면 충돌할 수 있습니다.
* `[Crash]` 장치가 베이킹에서 손실된 후 페인팅 모드로 돌아가기
* `[Crash]` 맵 내보내기 취소 후 Painter 종료
* `[Crash]` 카메라 이름에 특수 기호가 있는 메시 내보내기
