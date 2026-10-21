---
breadcrumb-title: ''
description: Substance 3D Painter 버전 전체의 모든 변경 내용 및 업데이트를 검토하여 시간의 흐름에 따른 기능 변화 및 개선 사항을 추적하세요.
title: 모든 변경 내용
user-guide-description: ''
user-guide-title: ''
source-git-commit: 479eb327180dd223bbff362e3f200995565cbcfa
workflow-type: tm+mt
source-wordcount: '40713'
ht-degree: 0%
---

# 모든 변경 내용

이 페이지에는 Substance 3D Painter의 이전 모든 릴리스에 대한 릴리스 정보가 포함되어 있으며, 최신 릴리스에서 이전 릴리스까지 정렬되어 있습니다.

>[!NOTE]
>
> Painter에 영향을 줄 수 있는 알려진 문제를 확인하려면 [전용 문서 페이지](known-issues.md)를 참조하세요.

## 버전 12

### 12.2.0

출시일: **2026/10/21**

요약: **이 업데이트는 주요 릴리스이며 베이킹을 위한 새로운 케이지 페인팅 기능을 추가하고 다각형 채우기 기능을 개선합니다. 자세한 내용은 전체 릴리스 정보를 참조하십시오.**

**추가됨:**

* 베이킹, 케이지 페인팅
* &lbrack;케이지 페인팅&rbrack; 기본 케이지 페인트 UI 만들기
* &lbrack;케이지 페인팅&rbrack; 새로운 케이지 시각화 옵션
* &lbrack;케이지 페인팅&rbrack; 편집 가능한 선택/채우기 도구
* &lbrack;케이지 페인팅(&amp;r); 도구 모음에서 혼합 모드 표시
* &lbrack;케이지 페인팅&rbrack; HDR 슬라이더 UI 변경 사항
* &lbrack;케이지 페인팅&rbrack; 시각화 셰이더
* &lbrack;케이지 페인팅&rbrack; 스택 재설정 옵션
* 다각형 채우기 도구 개선
* &lbrack;다각형 채우기(&amp;r); 다각형 패치 추가
* &lbrack;다각형 채우기(&amp;r); 다각형 추가 루프
* &lbrack;다각형 채우기(&amp;r); 루프/패치 대칭 지원
* &lbrack;다각형 채우기(&amp;r); 대칭 가장자리 미리 보기
* &lbrack;다각형 채우기&rbrack; 루프 및 부분 루프가 있는 삼각형 제거
* 활성 텍스처 세트에만 표시되는 &lbrack;다각형 채우기&rbrack; 와이어프레임
* &lbrack;다각형 채우기&rbrack; 클릭할 수 없는 삼각형의 빨간색 가장자리 강조
* &lbrack;다각형 채우기&rbrack; 채우기 모드 옵션을 비활성화하지 않음
* &lbrack;다각형 채우기&rbrack; 다각형 채우기를 사용하여 모든 채널 속성 설정 허용
* &lbrack;다각형 채우기&rbrack; 이전 획 다시 시작 다각형 채우기 사용
* &lbrack;다각형 채우기&rbrack; 비활성 텍스처 세트에 금지된 커서 표시
* &lbrack;다각형 채우기(&amp;r); ALT 빠른 미리 보기
* Polyloop로 임시 전환(SHIFT+A)을 위한 &lbrack;Polygon Fill&rbrack; 단축키
* &lbrack;뷰포트(&amp;r); 텍스처 세트 표시 / UV 타일 선택 강조 표시
* &lbrack;Viewport&rbrack; 실시간 뷰포트에서 주문 독립 투명도 지원 추가
* &lbrack;표시 설정&rbrack; 표시 설정을 새 그룹으로 다시 구성
* &lbrack;도구(&amp;r); 브러시 획을 사용한 추가 혼합 지원 추가
* &lbrack;도구(&amp;r); 다각형 칠을 사용한 추가 혼합 지원 추가
* &lbrack;USD&rbrack; 불투명도 맵이 있는 내보낸 USD이 아놀드에서 모든 투명도를 렌더링합니다.
* &lbrack;Nvidia&rbrack; 최신 Nvidia 드라이버에 대한 경고 추가(616.56 ~ 617.14)
* 새 &quot;mesh_uv_neighbor&quot; 엔진 맵 입력 추가
* 베이커를 버전 3.23.0으로 업데이트
* Substance 엔진을 버전 9.6.1로 업데이트

**고정:**

* &lbrack;Baking&rbrack; 앰비언트 오클루전 메쉬 이름별 배경 무시가 작동하지 않음
* &lbrack;Baking&rbrack; &lbrack;AMD&rbrack; 장치가 두꺼운 높은 폴리 메쉬로 굽을 때 손실됨
* &lbrack;성능&rbrack; Painter hogs VRAM 사용
* &lbrack;Viewport&rbrack; HDPI 화면에서 프로젝트를 열 때 누락된 텍스처
* 마스크에서 페인팅할 때 &lbrack;Tool&rbrack; 혼합 모드가 회색으로 표시됩니다.
* 네트워크에서 내보낸 후 임시 폴더가 삭제되지 않음
* &lbrack;USD&rbrack; 내보낸 USD 형상이 UV 테두리를 따라 분할됩니다.
* &lbrack;USD&rbrack; 잘못된 형식의 USDz를 로드할 때 고정

### 12.1.5

출시일: **2026/09/15**

요약: **부 릴리스**

**고정:**

* 셸프에서 네트워크로 이미지 내보내기가 더 이상 작동하지 않습니다.
* &lbrack;Generator&rbrack; &quot;텍스처 사용&quot;을 false로 설정해도 텍스처 입력 사용이 비활성화되지 않습니다.
* 3D 투영 편집 중 저장 시 뷰포트 고정
* 재질 레이어 해상도가 너무 낮음

### 12.1.4

출시일: **2026/09/04**

요약: **부 릴리스**

**고정:**

* 파일 이름에 ASCII가 아닌 문자가 포함된 파일을 가져오거나 내보낼 때 &lbrack;충돌&rbrack; 충돌

### 12.1.3

출시일: **2026/08/26**

요약: **부 릴리스**

**추가됨:**

* Substance 엔진을 버전 9.4.6으로 업데이트

**고정:**

* &lbrack;회색 음영 피커&rbrack; 도구 변경 후 피커가 열려 있음
* &lbrack;기울이기 굽기&rbrack; 페인팅 및 실행 취소 시 기울이기 교정이 중단됨
* &lbrack;투영 도구&rbrack; 뷰포트 상호 작용이 투영 도구에 의해 차단됨
* &lbrack;동적 선&rbrack; 브러시 속성에서 동적 선 매개 변수가 누락되었습니다.
* 네트워크로 내보내기가 더 이상 작동하지 않습니다

### 12.1.2

출시일: **2026/08/03**

요약: **부 릴리스**

**고정:**

* &lbrack;충돌&rbrack; 일부 Substance은 렌더링 시 충돌으로 이어질 수 있습니다.
* &lbrack;충돌&rbrack; 굽기 모드에서 메시 다시 가져오기
* &lbrack;충돌&rbrack; 그래픽 표시를 초기화하지 못하면 충돌이 발생할 수 있습니다.
* &lbrack;충돌&rbrack; 경우에 따라 로그를 업데이트하는 동안 텍스처 내보내기가 충돌이 될 수 있습니다.
* 환경 맵을 로드/업데이트할 때 가끔씩 베이킹 모드에서 &lbrack;충돌&rbrack; 충돌
* &lbrack;굽기&rbrack; 높은 폴리 파일을 수정한 후 굽기를 다시 실행하면 멈춤 현상이 발생할 수 있습니다
* &lbrack;Photoshop으로 보내기&rbrack; 레이어의 마스크 내보내기 실패
* &lbrack;엔진&rbrack; 고정점 결과가 마스크와 색상 채널 간에 렌더링되지 않음

### 12.1.1

출시일: **2026/07/09**

요약: 마이너 릴리스

추가됨:

* &lbrack;기울이기 굽기&rbrack; 기울이기 기본 노출 표준 모드: 메시 또는 삼각형별
* &lbrack;등록 정보&rbrack; 균일 색상을 항상 채널의 기본값으로 재설정합니다.
* 텍스처 생성을 위해 OpenPBR 내보내기 창에서 범주별로 출력 템플릿 다시 그룹화(&lbrack;&rbrack;)
* Substance 엔진을 버전 9.4.5로 업데이트

수정:

* &lbrack;프로젝트&rbrack; 일부 프로젝트를 열고 저장하는 데 평소보다 시간이 오래 소요될 수 있습니다.
* &lbrack;충돌&rbrack; 여러 메시를 다시 로드하면 충돌이 발생할 수 있습니다.
* 마스크 보기 모드에서 충돌을 삭제하면 채널이 나옵니다(&lbrack;&rbrack;)
* &lbrack;충돌&rbrack; 일부 Substance은 렌더링 시 충돌으로 이어질 수 있습니다.
* 페인트 스큐에서 &lbrack;페인트 스큐&rbrack; 선택한 도구가 페인팅 모드로 전환한 후 선택된 상태로 유지
* &lbrack;Baking Common Settings&rbrack; 케이지 거리 설정이 케이지 와이어프레임 및 셰이더 시각화를 업데이트하지 않음
* &lbrack;엔진&rbrack; UV 패딩 &quot;3D Space Neighbor&quot; 모드가 얇은 삼각형에서 제대로 작동하지 않음
* &lbrack;엔진&rbrack; 고정점 결과가 마스크와 색상 채널 간에 렌더링되지 않음

### 12.1.0

출시일: **2026/06/23**

요약: **이 업데이트는 주요 릴리스이며 새 베이킹 기본 UI 상태, 페인팅 기울이기 맵, 자동 다시 베이크, 하드 표면 메시 및 OpenPBR에 대한 자동 UV 감싸기 해제의 새 옵션을 통한 베이커 개선 사항이 포함되어 있습니다. 자세한 내용은 전체 릴리스 정보를 참조하십시오.**

**추가됨**:

* &lbrack;기울이기 굽기&rbrack; 기울이기 페인팅 도구
* &lbrack;Skew Baking&rbrack; 기울이기 맵을 페인트할 때 기울이기 미리 보기 셰이더 및 기울이기 방향 벡터 시각적 요소 추가
* &lbrack;기울이기 굽기&rbrack; 가장자리 보호 추가 옵션
* &lbrack;기울이기 굽기&rbrack; 자동 다시 굽기
* &lbrack;Skew Baking&rbrack; 메시 맵 목록 UI 다시 작업
* &lbrack;기울이기 굽기&rbrack; 메시 맵 분할/공통 굽기 설정 + 메시 맵 목록 기준 색상 또는 마스크만 공통 설정 외부 이동
* &lbrack;기울이기 굽기&rbrack; 뷰포트 도구 모음 변경 단추
* &lbrack;기울이기 굽기&rbrack; 상단 도구 모음에서 브러시에 대한 대칭 전환 표시
* &lbrack;Skew Baking&rbrack; 메시 맵 목록 동기화 메뉴의 이름 바꾸기 옵션
* &lbrack;기울이기 굽기&rbrack; 동기화 및 체크 상태 업데이트 대화 상자
* &lbrack;기울이기 굽기&rbrack; 회색 음영 색상 피커 변형 만들기
* &lbrack;기울이기 굽기&rbrack; 굽기 모드 업데이트 아이콘
* &lbrack;자동 줄 바꿈 해제&rbrack; 하드 서피스 통합 옵션
* &lbrack;OpenPBR&rbrack; OpenPBR 1.1에 대한 지원 추가
* &lbrack;OpenPBR&rbrack; OpenPBR을 기본 워크플로우 및 셰이더로 설정
* &lbrack;OpenPBR&rbrack; USD을 통해 OpenPBR 재질 및 텍스처 가져오기
* &lbrack;OpenPBR&rbrack; USD을 통해 OpenPBR 재질 및 텍스처 내보내기
* &lbrack;OpenPBR&rbrack; 텍스처 이름 지정 규칙을 표시하는 내보내기 창 업데이트
* &lbrack;OpenPBR&rbrack; 지원 OpenPBR 변경 사항에 대한 설명서 추가
* &lbrack;OpenPBR&rbrack;&lbrack;Iray&rbrack; Iray에서 OpenPBR 1.1을 지원하는 새 MDL 추가
* USD 내보내기에 대한 몇 가지 사소한 개선 사항
* &lbrack;UI&rbrack; 다른 텍스처 세트에서 페인트를 시도할 때 뷰포트에 경고를 추가합니다.
* &lbrack;병합&rbrack; 텍스처 세트 전체에서 모든 인스턴스 레이어를 병합하도록 허용
* &lbrack;텍스처 세트 설정&rbrack; 새 창을 통해 한 번에 여러 채널을 선택할 수 있도록 허용
* &lbrack;History&rbrack; &quot;value&quot; 업데이트 매개 변수 이름을 반영하는 실행 취소 항목 단어
* &lbrack;레이어 스택&rbrack; 마스크의 채우기 효과를 기본적으로 흰색(1.0)으로 설정
* &lbrack;Substance&rbrack; 새 &quot;mesh_hard_edges_triangle&quot; 엔진 맵 입력 추가
* &lbrack;Substance&rbrack; 새 &quot;mesh_hard_edges&quot; 엔진 맵 입력 추가
* &lbrack;Shader&rbrack; 동일한 이름을 공유하는 셰이더 인스턴스를 방지합니다
* &lbrack;Shader&rbrack; USD 또는 GLTF 파일을 가져올 때 프로젝트 템플릿의 셰이더를 사용합니다
* Adobe Color Engine을 버전 7.0으로 업데이트
* 최소 MacOSX 버전을 13.0 (Ventura)으로 업그레이드
* &lbrack;Content&rbrack; OpenPBR을 위한 새 프로젝트 템플릿
* &lbrack;Content&rbrack; 새 OpenPBR 셰이더를 사용하도록 샘플 프로젝트 업데이트
* &lbrack;Python&rbrack; UI에서와 같이 포함 및 제외 모드를 허용하도록 지오메트리 마스크 API 확장

**고정**:

* &lbrack;충돌&rbrack;&lbrack;메시 맵 설정&rbrack; 다른 텍스처 세트에 설정 적용
* 세계 공간 정상 없이 맵에서 곡률을 굽는 경우 &lbrack;충돌&rbrack;
* &lbrack;충돌&rbrack;&lbrack;Baking&rbrack; 사용자 정의 케이지가 활성화되었지만 파일이 선택되지 않은 충돌 굽기
* &lbrack;충돌&rbrack; AO 굽기 취소
* &lbrack;Auto-Cage&rbrack; 높은 폴리 파일 경로가 잘못된 경우 무한 로드
* &lbrack;Linux&rbrack;&lbrack;Windows&rbrack; 색상 피커가 완전히 검정이거나 나타나지 않을 수 있습니다
* &lbrack;다각형 채우기 도구(&amp;r); 도구가 PBR이 아닌 경우 작동하지 않습니다.
* &lbrack;&lbrack; 페인트&rbrack; 기본 색상 채널을 삭제해도 이전에 칠한 색상이 삭제되지 않음
* &lbrack;USD&rbrack; 셰이더 인스턴스가 모두 올바르게 감지되지 않음
* &lbrack;Substance&rbrack; 입력/출력 노드의 첫 번째 사용만 고려됩니다.
* &lbrack;Shader&rbrack; 앰비언트 오클루전은 다른 혼합 방법을 사용하여 텍스처 세트에 두 번 적용됩니다
* &lbrack;엔진&rbrack; 빈 파란색 텍스처(검정)가 있는 일반 채널은 잘못된 혼합 결과를 초래할 수 있습니다.
* &lbrack;GLTF Import&rbrack; 모든 텍스처 세트에서 알파 혼합 사용
* &lbrack;GLTF Export&rbrack; 알파 혼합은 내보낼 때 항상 활성화됩니다.
* &lbrack;Export&rbrack; GLTF 파일을 가져올 때 양면 기하 도형이 항상 비활성화됩니다.
* &lbrack;Javascript&rbrack; 음영 설정 수정이 실행 취소 기록에 기여하지 않음
* 모임 매트의 디스플레이 설정에서 &lbrack;Samples&rbrack; 서브서피스 분산이 활성화되지 않음

### 12.0.3

출시일: **2026/05/05**

요약: **부 릴리스**

**추가됨:**

* 베이커를 버전 3.22.2로 업데이트
* Substance 엔진을 버전 9.4.3으로 업데이트
* &lbrack;Python&rbrack; 특정 위치에 스마트 재질 저장

**고정:**

* 재질 선택 시 &lbrack;Ubuntu&rbrack; 충돌
* 다른 앱 데이터에 대한 액세스를 요청하는 &lbrack;Mac&rbrack; 반복 팝업이 나타납니다
* &lbrack;Baking&rbrack; 가공물은 곡률 맵에 나타날 수 있습니다.
* &lbrack;Baking&rbrack; Baking이 느린 경우도 있습니다.
* &lbrack;형상으로 뒤틀기&rbrack; 형상으로 뒤틀기는 경우에 따라 비활성화됩니다
* &lbrack;UV 타일&rbrack; 고정점의 추출된 알파가 다른 타일에서 무시됨
* &lbrack;Python&rbrack;&lbrack;Mac&rbrack; SSL이 있는 Python 콘솔의 예외
* &lbrack;Python&rbrack; Qt 위젯이 남은 상태에서 종료 시 Painter 충돌

### 12.0.2

출시일: **2026/04/07**

요약: **부 릴리스**

**추가됨:**

* &lbrack;색상 관리&rbrack; 색상 피커의 기본 색상 공간을 지정하는 새 OCIO 추가
* &lbrack;Python&rbrack; Python API에서 자동 줄 바꿈 설정 노출

**고정:**

* &lbrack;충돌&rbrack; 디스크 공간이 부족한 상태로 저장하면 프로젝트가 충돌 또는 손상될 수 있습니다
* &lbrack;충돌&rbrack; &lbrack;리본&rbrack; 리본을 사용하면 일부 프로젝트에 충돌이 발생할 수 있습니다.
* .assbin 파일을 폴더에 쓸 수 없는 경우 &lbrack;충돌&rbrack; &lbrack;Baking&rbrack; 충돌
* &lbrack;Import&rbrack; Stager의 OBJ 메시가 프로젝트 생성 시 실패할 수 있음
* &lbrack;Import&rbrack; OBJ에 경우에 따라 얼굴이 누락됩니다
* &lbrack;Import&rbrack; 재료가 할당되지 않은 USD 메시는 가져올 때 충돌 가능
* &lbrack;채워진 경로&rbrack; 대칭의 영향을 받지 않음
* &lbrack;Stencil&rbrack; 미리 보기의 해상도가 페인트 결과보다 낮음
* &lbrack;UI&rbrack; &#39;uv island&#39;가 ID 맵 색상 소스 도구 설명에 여전히 언급됨
* &lbrack;Display&rbrack; 그림자가 반전됨
* &amp;lbrport&rbrack; 굽기 모드로 전환한 후에도 뒤틀기 투영이 남아 있습니다.
* &lbrack;Warp&rbrack; Z축에서 크기 조정이 0으로 설정되고 [기하 도형으로 비틀기]가 활성화된 경우 그리드가 사라짐
* &lbrack;Python&rbrack; 범위 수정 채널을 추가하는 동안 예기치 않은 오류가 발생했습니다.

### 12.0.1

출시일: **2026/03/18**

요약: **부 릴리스**

**고정:**

* &lbrack;충돌&rbrack;&lbrack;고정&rbrack; 특정 프로젝트에서 내보내기

### 12.0.0

출시일: **2026/03/09**&#x200B;요약: **주요 릴리스입니다. 이 릴리스에는 레이어 병합, 형상 뒤틀기, 새 포스트 효과, 새 프로젝트 창 개선 및 기타 개선 사항이 포함되어 있습니다.**

**추가됨**:

* &lbrack;레이어 병합&rbrack; 레이어 스택 내부의 레이어 병합
* &lbrack;레이어 병합&rbrack; 병합된 레이어를 디스크로 내보내기
* &lbrack;형상으로 뒤틀기&rbrack; 뒤틀기 투영에 새로운 자동 뒤틀기 기능 추가
* &lbrack;Post-effects&rbrack; 포스트 효과를 새 글꼴이 추가된 것으로 바꿉니다.
* &lbrack;Post-effects&rbrack; 톤 매퍼 업데이트
* &lbrack;Post-effects&rbrack; Post-effects 에셋에 대한 새로운 사용 추가
* &lbrack;Content&rbrack;&lbrack;Post-effects&rbrack; 라이브러리에 기본 사후 효과 에셋 통합
* &lbrack;새 프로젝트&rbrack; 프로젝트 생성을 위한 UI 개선
* &lbrack;새 프로젝트&rbrack;메시 기능 다시 가져오기 변경 사항
* &lbrack;새 프로젝트&rbrack; \*.geo.usd 파일 열기 허용
* &lbrack;프로젝트 구성&rbrack; 프로젝트 구성을 위한 UI 개선
* USD 라이브러리를 버전 25.05로 업데이트
* Substance 엔진을 버전 9.3.4로 업데이트
* AMD GPU의 경우 최소 드라이버를 25.3.1/25.Q2으로 올립니다.
* Qt를 6.8.6으로 업데이트
* &lbrack;Scripting&rbrack; JavaScript API를 버전 1.1.20으로 업데이트
* Python을 3.13으로 업데이트

**고정:**

* &lbrack;충돌&rbrack; 마스크에서 재질 채널 출력을 변경하면 충돌 가능
* &lbrack;Import&rbrack; USD 파일을 가져올 때 EXR 텍스처가 선형 대신 sRGB로 강제 적용됨
* &lbrack;UV 타일&rbrack; 단일 이미지가 있는 이미지 시퀀스도 다른 UV 타일을 채웁니다.
* &lbrack;Baking&rbrack; AO는 CPU 굽기와 GPU 굽기가 다릅니다.
* &lbrack;색상 관리&rbrack;&lbrack;MacOS&rbrack; 뷰포트 기본 색상이 색상 피커와 일치하지 않음
* &lbrack;USD&rbrack; 균일 값을 가져오지 않는 경우가 있습니다

## 버전 11

### 11.1.3

출시일: **2026/02/12**&#x200B;요약: **부 릴리스**

**고정**:

* &lbrack;페인트&rbrack; 스텐실 및 대칭이 작동하지 않는 경우가 있습니다.
* &lbrack;패스&rbrack; 손가락 획 불투명도 슬라이더를 변경할 때 업데이트 없음
* &lbrack;프로젝트&rbrack; 일부 형상을 페인트 할 수 없음
* 텍스처 세트 해상도 변경 시 &lbrack;Ribbon&rbrack; 인스턴스화된 경로가 사라짐
* &lbrack;UI&rbrack; 색상 피커가 축소되고 경우에 따라 사라질 수 있습니다

### 11.1.2

출시일: **2026/01/13**&#x200B;요약: **부 릴리스**

**추가됨**:

* &lbrack;Baking&rbrack; 비동기 저장을 통해 UV 타일 프로젝트의 굽기 시간 개선
* &lbrack;Shaders&rbrack; Vulkan 마이그레이션 후 셰이더 API 변경 사항 언급
* OpenEXR을 버전 3.4.4로 업데이트

**고정**:

* nvidia GTX 10xx 시리즈에서 시작하는 동안 &lbrack;충돌&rbrack; 충돌
* &lbrack;충돌&rbrack; 다른 텍스처 세트에서 색상 피커를 사용하면 애플리케이션을 종료할 때 충돌이 발생할 수 있습니다
* &lbrack;Performance&rbrack; 레이어가 많은 프로젝트에서 페인트할 때 성능 문제
* 그래픽 태블릿 펜으로 페인팅할 때 뒤틀기(&lbrack; Performance&rbrack; Lag)
* &lbrack;UI&rbrack; 카메라 설정은 렌더링 모드에서 비활성화된 상태로 유지됩니다(Iray)
* &lbrack;Ribbon&rbrack; 경로가 어떤 경우에는 모서리 뒤에 예기치 않게 겹칠 수 있습니다
* &lbrack;Ribbon&rbrack; UV 타일 성능 문제
* &lbrack;Substance&rbrack;&lbrack;UI&rbrack; 축소 시 이미지 입력이 사라짐
* 중첩된 Substance을 숨기는 경우 표시되더라도 &lbrack;group&rbrack;&lbrack;UI&rbrack; 중첩 그룹이 남아 있을 수 있습니다.
* &lbrack;Baking&rbrack;&lbrack;UI&rbrack; 곡률 샘플링 반경을 0.01 이상으로 설정할 수 없음
* &lbrack;Baking&rbrack;&lbrack;UI&rbrack; 최대 폐색기 거리를 1을 초과하여 설정할 수 없음
* &lbrack;Baking&rbrack; AO 설정 &quot;자체 오클루전&quot;은 몇 개의 [텍스처 설정]과 함께 무시되고 [낮음]은 [높음]으로 무시됩니다
* &lbrack;Baking&rbrack; ID 맵이 [낮음]에서 [높음]으로 FBX에서 꼭지점 색상을 굽지 않습니다.
* &lbrack;Content&rbrack; 하이패스 필터를 사용하면 색상 관리 채널의 색상이 바랜 것처럼 표시됩니다

### 11.1.1

출시일: **2025/12/09**&#x200B;요약: **부 릴리스**

**추가됨**:

* &lbrack;Performance&rbrack; 부분 텍스처 계산 시 UV 타일 성능 향상
* &lbrack;Bakers&rbrack; 버전 3.15.4로 업데이트

**고정**:

* &lbrack;충돌&rbrack;&lbrack;MacOS&rbrack; 이전 버전에서 프로젝트를 저장하면 항상 충돌
* &lbrack;충돌&rbrack; 프로젝트를 닫으면 때때로 충돌이 발생할 수 있습니다.
* &lbrack;Project&rbrack; 이전 버전에서 만든 프로젝트를 열 때 &quot;멤버 수 불일치&quot; 오류 발생
* &lbrack;Baking&rbrack; UV 타일이 있는 경우 이전 베이크 결과와 결합되지 않음
* &lbrack;Baking&rbrack; 장치가 Nvidia GTX 10XX 시리즈에서 광선 추적을 비활성화했는데도 손실됨
* &lbrack;Baking&rbrack; AO(표준 포함)에는 패딩이 없으므로 가장자리에 아티팩트가 있음
* &lbrack;Baking&rbrack; AO 설정 &quot;자체 오클루전&quot;이 여러 텍스처 세트와 &quot;이름별 일치&quot;에서 무시됩니다.
* &lbrack;Baking&rbrack; ID 맵은 하이 폴리 메시에 꼭지점 색상이 없는 경우 완전히 검정색입니다.
* 알파 혼합 모드에 대한 &lbrack;Ribbon&rbrack; 도구 설명이 선형 닷지 대신 화면 혼합 모드를 언급함
* 점이 패스 끝에 가깝게 이동하면 &lbrack;패스&rbrack; 접선이 예기치 않은 루프를 만듭니다.
* 마스크에서 투영을 사용하는 경우 &lbrack;도구&rbrack; 질감 미리 보기가 작동하지 않음
* &lbrack;Engine&rbrack; 작은 획을 페인트하면 깨진 가공물이 생길 수 있습니다
* &lbrack;Shader&rbrack; 셰이더 인스턴스 생성을 실행 취소해도 제대로 제거되지 않습니다
* &lbrack;GLTF 내보내기의 내보내기&rbrack; Alpha 모드가 항상 MASK로 설정되어 있습니다.
* &lbrack;Python&rbrack; 범위 수정 블록 외부의 레이어 스택을 편집할 때 예기치 않은 오류가 발생했습니다.

**알려진 문제**:

* &lbrack;Ribbon&rbrack; UV 타일 성능 문제
* &lbrack;Ribbon&rbrack; 경로가 어떤 경우에는 모서리 뒤에 예기치 않게 겹칠 수 있습니다
* &lbrack;충돌&rbrack;&lbrack;리본&rbrack; 리본에서 매우 긴 텍스트 만들기 충돌 가능
* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작음
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨
* &lbrack;Engine&rbrack; 일반 채널 이동 색상에서 복제 도구로 페인팅이 잘못됨
* &lbrack;Python&rbrack; 고스트 위젯이 여전히 작동하는 스크립트에 의해 삭제된 것으로 나타남

### 11.1.0

릴리스 날짜: **2025/11/18**&#x200B;요약: **이 업데이트는 주요 릴리스이며 전용 새 콘텐츠가 포함된 새 리본 도구, 칠 레이어에 대한 대칭 지원, 변위에 대한 물리적 크기 매개 변수, 업데이트된 베이커를 통한 향상된 성능, Windows 및 Linux에 대한 전체 Vulkan 지원 및 기타 개선 사항이 포함되어 있습니다.**

**추가됨**:

* 새 리본 도구
* &lbrack;도구(&amp;r); 매끄러운 패스를 만들기 위한 새로운 리본 도구 추가
* &lbrack;리본(&amp;r); 등록 정보 창에서 리본 사전 설정 바로 가기 추가
* &lbrack;Ribbon&rbrack; 패스에 있는 정점당 리본의 불투명도를 변경할 수 있습니다.
* &lbrack;Ribbon&rbrack; 패스의 정점당 리본 크기 변경 허용
* &lbrack;Ribbon&rbrack; 경로가 닫혀 있을 때 Substance에 정의된 시작/끝 제거
* &lbrack;Ribbon&rbrack; 페인트/지우개/손가락 패스 도구의 속성 창에서 패스/재질 제거 미리 보기
* &lbrack;Ribbon&rbrack; 자체 중첩 시 알파 및 일부 채널에 대한 혼합 모드를 추가합니다.
* 칠 대칭
* &lbrack;Fill&rbrack; 칠 레이어 및 효과의 대칭 지원 추가
* &lbrack;Fill&rbrack;&lbrack;UI&rbrack; 칠 레이어 및 효과에 대한 속성 창의 노출 대칭 설정
* &lbrack;Fill&rbrack; 뷰 포트 메뉴 및 속성 창에서 대칭 설정 UI 재작업
* 뒤틀기 모드에서 투영할 때 일반 텍스처의 방향을 올바르게 조정하는 &lbrack;Fill&rbrack;
* 물리적 크기 변위
* &lbrack;변위&rbrack; 물리적 크기를 변위 단위로 사용
* 성능 향상
* &lbrack;성능&rbrack; 큰 삼각형에서 작은 브러시 획의 렌더링 향상
* &lbrack;성능&rbrack; 셰이더 컴파일 시간 개선
* &lbrack;Performance&rbrack; Windows 및 Linux에 대한 전체 Vulkan 지원
* &lbrack;Performance&rbrack; 더 빠른 GPU 렌더링 및 AMD 광선 추적 지원으로 업데이트된 베이커
* &lbrack;UI&rbrack; 도구 속성을 그룹으로 다시 구성하고 기본적으로 일부 축소
* &lbrack;엔진&rbrack; Substance 엔진을 버전 9.2.5로 업데이트
* &lbrack;Substance&rbrack; 도구 및 채우기의 Substance 리소스에 대한 해상도 재정의 노출
* &lbrack;내보내기&rbrack; 메쉬 맵 업데이트 내보내기 사전 설정을 사용하여 회색 음영 텍스처 내보내기
* Python
* &lbrack;Baking&rbrack;&lbrack;Python&rbrack; 베이커 업데이트 후 변경 사항 나누기를 변경 로그에 표시
* &lbrack;Python&rbrack; Python에 채우기 대칭 설정 노출
* 콘텐츠 및 새 콘텐츠
* &lbrack;내용&rbrack; 리본 도구에 대한 75개의 새로운 도구 사전 설정 추가
* &lbrack;Content&rbrack; 리본과 호환되도록 그레이디언트 작성기 리소스 업데이트

**고정**:

* &lbrack;충돌&rbrack; 패스 스냅이 활성화된 상태에서 다른 프로젝트를 로드하면 충돌 가능
* &lbrack;충돌(&amp;r); 클립보드에 있는 다른 세션의 정보를 사용하여 충돌 가능 패스 패널을 마우스 오른쪽 버튼으로 클릭
* &lbrack;UI&rbrack; 인터페이스가 패스를 만들 때 도구 속성에서 위로 스크롤됩니다.
* 경로 뷰포트 시각화가 숨겨지면 &lbrack;UI&rbrack; 마우스 커서가 사라짐
* &lbrack;패스(&amp;r); 패스 패널에서 다른 도구 속성을 복사/붙여넣기하면 속성이 불안정해집니다
* &lbrack;도구(&amp;r); 지우개 및 손가락 도구 사전 설정이 항상 채널 선택을 업데이트하는 것은 아닙니다
* &lbrack;Tool&rbrack; Painted 값은 회색이지만 UI는 마스크에 색상이 지정된 도구 사전 설정을 로드한 후 흰색을 표시합니다.
* 마스크에서 만든 &lbrack;도구&rbrack; 사전 설정은 다른 사전 설정에서 로드한 채널 값을 유지합니다.
* &lbrack;Substance&rbrack; 그래프에 정의된 표준 색상 공간 재정의가 고려되지 않습니다.
* &lbrack;Content&rbrack; 기본 브러시 모양 리소스가 오래된 Substance을 사용함

**알려진 문제**:

* 셰이더 인스턴스 기록이 제대로 추적되지 않았습니다.
* &lbrack;Ribbon&rbrack; UV 타일 성능 문제
* &lbrack;Ribbon&rbrack; 경로가 어떤 경우에는 모서리 뒤에 예기치 않게 겹칠 수 있습니다
* 점이 패스 끝에 가깝게 이동하면 &lbrack;Ribbon&rbrack; 접선이 원치 않는 루프를 만듭니다.
* &lbrack;충돌&rbrack;&lbrack;리본&rbrack; 리본에서 매우 긴 텍스트 만들기 충돌 가능
* 마스크에서 투영을 사용하는 경우 &lbrack;도구&rbrack; 질감 미리 보기가 작동하지 않음
* &lbrack;Baking&rbrack; AO 설정 &quot;자체 오클루전&quot;은 여러 텍스처 세트에서 무시되고 &quot;이름별 일치&quot;는 활성화됨
* &lbrack;Baking&rbrack; AO(정상)의 경우 패딩이 누락되어 가장자리에 아티팩트가 있습니다.
* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작음
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨
* &lbrack;Engine&rbrack; 일반 채널 이동 색상에서 복제 도구로 페인팅이 잘못됨
* &lbrack;Python&rbrack; 고스트 위젯이 여전히 작동하는 스크립트에 의해 삭제된 것으로 나타남

### 11.0.3

출시일: **2025/08/05**&#x200B;요약: **부 릴리스**

**추가됨**:

* &lbrack;Substance 3D Assets&rbrack; 3D 에셋 패널에 알림 점 추가
* &lbrack;VFX Platform 2025&rbrack; 색상 관리 설정에 ACE 2.0 구성 추가
* &lbrack;VFX Platform 2025&rbrack; OCIO을 버전 2.4.2로 업데이트
* Iray를 버전 2024.10으로 업데이트
* &lbrack;엔진&rbrack; Substance 엔진 v.9.2.3으로 업데이트
* &lbrack;Nvidia&rbrack; Nvidia 최소 드라이버 버전을 572.60(Win) 및 570.169(Linux)로 올리기

**고정**:

* &lbrack;Python&rbrack; 범위 수정이 작업 내역 창에 나타나지 않습니다.

**알려진 문제**:

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작음
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨
* &lbrack;Engine&rbrack; 일반 채널 이동 색상에서 복제 도구로 페인팅이 잘못됨
* &lbrack;Python&rbrack; 고스트 위젯이 여전히 작동하는 스크립트에 의해 삭제된 것으로 나타남

### 11.0.2

출시일: **2025/06/10**&#x200B;요약: **부 릴리스**

**추가됨**:

* &lbrack;Mac&rbrack; 특정 운영 체제 버전에 대한 경고를 추가하여 가공물로 연결
* &lbrack;자동 업데이트&rbrack; 자산 오류 로그에 대한 부 UX 개선
* &lbrack;자동 언랩&rbrack; 시밍 개선 사항을 사용하여 버전 1.3.2로 업데이트
* &lbrack;USD&rbrack;&lbrack;FBX&rbrack; 스파스 데이터가 있는 여러 UV 세트에 대한 지원 추가
* &lbrack;FBX으로 내보낸 Export&rbrack; 메시를 가져올 때 추가 UV 세트가 누락됩니다.

**고정**:

* 네트워크 드라이브에 저장할 때 &lbrack;MacOS&rbrack;&lbrack;Linux&rbrack; 충돌
* &lbrack;Win&rbrack;&lbrack;Tablet&rbrack; 패닝 시 깜박임
* 패스 도구로 작업할 때 &lbrack;SpaceMouse&rbrack; 문제
* &lbrack;Auto-cage&rbrack;에서 메시를 다시 로드한 후 구울 수 없음
* 첫 번째 타일이 없는 경우 &lbrack;Auto-update&rbrack; 이미지 시퀀스가 다시 로드되지 않음
* &lbrack;패스&rbrack; 사용자 정의 접선은 다른 접선에 영향을 줄 수 있습니다.
* 첫 번째 점이 다른 텍스처 세트에 있는 경우 &lbrack;패스&rbrack; 패스가 텍스처 세트에 나타나지 않습니다.
* &lbrack;UI&rbrack; 프로젝트를 연 후 일부 메뉴가 항상 비활성화됩니다(예: 대칭).
* &lbrack;등록 정보&rbrack;는 채워진 경로 도구로 도구 사전 설정을 사용/불러올 수 없습니다.
* &lbrack;USD&rbrack; USD 파일을 사용할 때 사용자 정의 셰이더에서 여러 UV 세트를 인식할 수 없음
* &lbrack;USD&rbrack; 같은 이름의 카메라가 재정의됩니다
* &lbrack;내보내기&rbrack; Photoshop으로 보내면 색상 및 회색 음영 결과에 대해 잘못된 색상 공간이 생성됩니다
* &lbrack;Export&rbrack; 알파가 있는 회색 음영 채널은 PNG 형식이 있는 회색 음영 대신 색상으로 내보내집니다
* &lbrack;내보내기&rbrack; 회색 음영 채널을 PSD으로 내보내면 파일이 잘못되거나 잘립니다.
* 다방향 모드에서 &lbrack;Content&rbrack; 뒤틀기 필터가 작동하지 않습니다.
* &lbrack;Python&rbrack; 레이어 스택 노드를 크롤링할 때 목록 오류를 할당할 수 없습니다.

**알려진 문제**:

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작음
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨
* &lbrack;Engine&rbrack; 일반 채널 이동 색상에서 복제 도구로 페인팅이 잘못됨
* &lbrack;Python&rbrack; 고스트 위젯이 여전히 작동하는 스크립트에 의해 삭제된 것으로 나타남

### 11.0.1

출시일: **2025/04/10**&#x200B;요약: **부 릴리스**

참고: **Linux CCD 버전이 4월 29일까지 지연됩니다.**

**추가됨:**

* Qt 6.5.8로 업데이트
* &lbrack;Substance&rbrack; 여러 이미지 입력이 동일한 사용량을 공유하는 경우 필터에 대한 로그 메시지 추가
* &lbrack;Nvidia&rbrack; 최신 Nvidia 드라이버에 대한 경고 추가(572.47)

**고정:**

* &lbrack;충돌&rbrack; 단일 채널 슬롯에 용도가 있는 sbsar를 드래그하여 놓을 때
* &lbrack;path&rbrack;&lbrack;Path&rbrack; 특정 패스를 클릭하지 않을 때 충돌 유형 변경 옵션이 회색으로 표시되지 않음
* &lbrack;칠 패스&rbrack;에서는 Substance 재질을 선택할 수 없어야 합니다.
* &lbrack;Engine&rbrack; 브러시 획을 따른 가공물
* &lbrack;엔진&rbrack; 경로는 특정 설정으로 끊어질 수 있습니다.
* 스포이드 색상 공간의 드롭다운 문제
* &lbrack;자동 업데이트&rbrack; &lbrack;Python&rbrack; 버전 없이 ResourceID를 사용할 때 잘못된 오류 메시지 표시
* 일부 프로젝트를 열 때 &lbrack;Shader&rbrack; 충돌

**알려진 문제:**

* 패스 도구로 작업할 때 &lbrack;SpaceMouse&rbrack; 문제
* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작음
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨
* &lbrack;Engine&rbrack; 일반 채널 이동 색상에서 복제 도구로 페인팅이 잘못됨
* &lbrack;Python&rbrack; 고스트 위젯이 여전히 작동하는 스크립트에 의해 삭제된 것으로 나타남

### 11.0.0

릴리스 날짜: **2025/03/11**&#x200B;요약: **주요 릴리스, 새로운 자동 업데이트 기능, 채워진 경로 도구 및 기타 경로 개선, 새로운 필터 및 베이킹을 위한 실험적인 자동 케이지 생성**

**추가됨**:

* 자동 업데이트
* &lbrack;자동 업데이트&rbrack; 에셋 패널의 수정된 에셋 자동 업데이트
* &lbrack;자동 업데이트&rbrack; 수정된 에셋 자동 업데이트
* &lbrack;자동 업데이트&rbrack; 기본적으로 자동 업데이트 해제 유지
* &lbrack;자동 업데이트&rbrack; 리소스 매개 변수가 일치하지 않는 경우 업데이트(선택 사항)(.sbsar, .glsl, .ai, .svg)
* &lbrack;자동 업데이트&rbrack; 자동 업데이트 기능을 비활성화하는 환경 변수 추가
* &lbrack;Auto-update&rbrack;&lbrack;SBSAR&rbrack; 리소스 매개 변수가 일치하지 않을 경우 업데이트를 선택적으로 지정합니다.
* 채워진 패스
* &lbrack;패스&rbrack;&lbrack;채우기&rbrack; 채워진 패스를 만들기 위한 새 도구 추가
* 경로 개선 사항
* &lbrack;패스&rbrack; 다각형에 스냅되는 패스 만들기
* &lbrack;경로(&amp;r); 경로 유형 전환 허용
* &lbrack;패스&rbrack; 콘텐츠와 마스크 간에 패스 정점 데이터 복사 및 붙여넣기 허용
* &lbrack;패스&rbrack; 새 점을 만들 때 각도를 제한할 수 있도록 허용
* &lbrack;패스&rbrack; 선에 구속점 생성 허용
* &lbrack;패스&rbrack; 한 번의 클릭으로 모양 닫기
* &lbrack;경로(&amp;r); 경로 정보 표시
* &lbrack;패스(&amp;r); 패스 정점의 비율 조정 및 회전 허용
* &lbrack;Path&rbrack;&lbrack;UX&rbrack; 변형 기즈모의 액세스를 더 쉽게 설정
* &lbrack;패스(&amp;r); 패스 미리 보기 추가
* &lbrack;패스(&amp;r); Shift + P로 패스 미리 보기 비활성화
* &lbrack;패스&rbrack; 측면 보기에서 접선 버전 개선
* &lbrack;Path&rbrack; 3D 패스에 포커스 허용
* UI를 껐다가 다시 전환할 때 &lbrack;패스&rbrack; 정점이 선택 상태를 유지해야 함
* &lbrack;패스(&amp;r); 백스페이스를 사용하여 패스 삭제 허용
* &lbrack;Path&rbrack; 사용자가 확장한 경우 Keep path list open
* &lbrack;Path&rbrack;&lbrack;Path&rbrack; 복사/붙여넣기 시 레이어 스택 이름을 올바르게 바꿉니다.
* &lbrack;패스&rbrack; UI 및 도구 설명 개선
* 성능
* &lbrack;성능&rbrack; 높은 쪽맞춤 레벨을 사용할 때 뷰포트 성능 향상
* &lbrack;성능&rbrack; 새 칠 레이어/효과에서 첫 번째 채널만 활성화
* &lbrack;성능&rbrack; 브러시 획 계산 병렬화
* 베이킹
* &lbrack;Baking&rbrack; 높은-폴리 메쉬로 굽기 위한 새로운 완전 자동 케이지 생성 옵션 추가(시험적)
* 콘텐츠
* &lbrack;Content&rbrack; 6개의 새로운 필터 추가: 스타일화, 정량화, 이방성 쿠와하라, 베벨 매끄럽게, 방향 거리, 회색 음영 변환
* &lbrack;Content&rbrack; Designer(새로운 2D Voronoi 포함)에서 노이즈와 Grunges를 최신 버전으로 업데이트
* &lbrack;Content&rbrack; 3개의 새로운 텍스처 생성기 추가(Tile Random, Triangle Grid, Scratches 생성기)
* &lbrack;Content&rbrack; 언리얼 엔진 템플릿 이름 바꾸기 및 사전 설정 내보내기
* Python
* &lbrack;Shelf&rbrack;&lbrack;Python&rbrack; Python에서 스마트 재질 또는 스마트 마스크를 디스크에 저장
* &lbrack;Python&rbrack; Python API에 베이킹 자동 케이지 추가
* &lbrack;Python&rbrack; 텍스처 세트/UV 타일 이름 및 설명 편집 허용
* &lbrack;Python&rbrack; 벡터 및 글꼴 소스에 대한 해상도 설정 공유
* &lbrack;Auto-update&rbrack;&lbrack;Python&rbrack; Python에서 프로젝트 자동 업데이트 기능 노출
* 기타
* &lbrack;내보내기&rbrack; 새 패널을 사용하면 보내기 옵션에 더 쉽게 액세스할 수 있습니다.
* &lbrack;Nvidia&rbrack; 최신 Nvidia 드라이버에 대한 경고 추가(572.16)
* 각도 스냅은 오브젝트/월드 공간 선택의 영향을 받아야 합니다.
* &lbrack;텍스처 세트 목록&rbrack; UV 타일에 사용자 정의 이름을 추가하고 내보낼 때 사용할 수 있도록 허용
* Mac
* &lbrack;Mac&rbrack; 그래픽 렌더링에 OpenGL 대신 Metal 사용
* &lbrack;Mac&rbrack; Mac Intel 지원 삭제

**고정**:

* &lbrack;충돌&rbrack; 이미지 입력 삭제
* 레이어 스택 단추를 통해 스마트 매트를 추가할 수 없습니다.
* GroupLayerNode에서 &lbrack;Python&rbrack; 효과를 찾을 수 없습니다.

**알려진 문제**:

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작음
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨
* 일부 사전 설정을 가져올 때 &lbrack;MacOS Intel&rbrack; 충돌
* &lbrack;Engine&rbrack; 일반 채널 이동 색상에서 복제 도구로 페인팅이 잘못됨
* &lbrack;Python&rbrack; 고스트 위젯이 여전히 작동하는 스크립트에 의해 삭제된 것으로 나타남
* &lbrack;RedHat&rbrack; 색상 피커 문제

## 버전 10

### 10.1.2

출시일: **2024/12/3**&#x200B;요약: **마이너 릴리스, 버그 수정**

**고정**:

* &lbrack;충돌&rbrack; 이미지 입력 삭제
* 레이어 스택 단추를 통해 스마트 매트를 추가할 수 없습니다.
* GroupLayerNode에서 &lbrack;Python&rbrack; 효과를 찾을 수 없습니다.

**알려진 문제**:

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작음
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨
* 일부 사전 설정을 가져올 때 &lbrack;MacOS Intel&rbrack; 충돌
* &lbrack;Engine&rbrack; 일반 채널 이동 색상에서 복제 도구로 페인팅이 잘못됨
* &lbrack;Python&rbrack; 고스트 위젯이 여전히 작동하는 스크립트에 의해 삭제된 것으로 나타남
* &lbrack;RedHat&rbrack; 색상 피커 문제

### 10.1.1

출시일: **2024/11/5**&#x200B;요약: **마이너 릴리스, 버그 수정**

**추가됨**:

* &lbrack;프로젝트&rbrack; 새 프로젝트 선택이 검증될 때까지 현재 프로젝트를 열어 둡니다.
* &lbrack;자동 언랩&rbrack; 텍셀 밀도를 통해 UV 섬을 UDIM으로 더 잘 분할할 수 있습니다.
* &lbrack;Baking&rbrack; 메시 맵의 컨텍스트 메뉴에서 모호한 사본 수정
* &lbrack;뒤틀기&rbrack; Z(깊이) 축에 대한 뷰포트에서 비율 제거
* &lbrack;가져오기/내보내기&rbrack; 사용하지 않는 이미지 파일 형식에 대한 지원 제거
* Substance 엔진을 9.1.4로 업데이트

**고정**:

* 에셋에서 리소스를 재배치하고 프로젝트를 저장한 후 &lbrack;충돌&rbrack;
* aiserver 라이브러리에 대한 &lbrack;충돌&rbrack; 문제
* 드문 경우지만 &lbrack;충돌&rbrack; Illustrator 서버 충돌
* 드물게 애플리케이션을 종료할 때 &lbrack;충돌&rbrack;
* 일부 컴퓨터에서 충돌 보고서를 보낼 수 없음
* &lbrack;Baking&rbrack; 꼭지점 색상이 제대로 읽히지 않음
* &lbrack;UI&rbrack; windows 및 시작 시 새로운 기능 위치가 이동됨
* &lbrack;Assimp&rbrack; Maya의 StandardSurface가 ID 굽기에서 인식되지 않음
* &lbrack;Python&rbrack; SSL lib 누락 시 오류가 출력됩니다.
* &lbrack;Python&rbrack;&lbrack;Win&rbrack; QColorConstants.Transparent를 호출할 때 오류 발생
* &lbrack;Python&rbrack; Python을 통해 생성된 레이어 축소판은 레이어 스택 내부를 클릭할 때까지 새로 고쳐지지 않습니다
* &lbrack;Shader&rbrack; 셰이더 API 변경 로그의 끊어진 링크
* &lbrack;3D Assets&rbrack; 3D Assets에 액세스할 때 OS 프록시 설정을 사용합니다.

**알려진 문제**:

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작습니다.
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨
* 일부 사전 설정을 가져올 때 &lbrack;MacOS Intel&rbrack; 충돌
* &lbrack;Engine&rbrack; 일반 채널 이동 색상에서 복제 도구로 페인팅이 잘못됨
* 스크립트를 통해 삭제된 것 같은 &lbrack;Python&rbrack; 위젯이 아직 작동 중임
* &lbrack;RedHat&rbrack; 색상 피커 문제

### 10.1.0

릴리스 날짜: **2024/09/17**&#x200B;요약: **주요 릴리스, 새 콘텐츠: 채우기 영역 마스크/색상 필터, 자수 데칼 필터 및 6개의 일반 Substance 필터, 재질 및 셰이더 속성이 포함된 USD 가져오기, 성능 개선, VFX 플랫폼 2024 호환 및 Linux RedHat으로의 마이그레이션**

**추가됨**:

* &lbrack;내용&rbrack; 새 채우기 영역 마스크/색상 필터 추가
* &lbrack;Content&rbrack; 새 자수 데칼 필터 추가
* &lbrack;Content&rbrack; 6개의 새로운 일반 Substance 필터(FXAA, 픽셀화, 하이패스, 포스터화, 스무딩 단계, 임계값) 추가
* &lbrack;USD&rbrack; 정의된 ASM 재질이 있는 USD 레이어 내보내기
* &lbrack;USD&rbrack; 재료 및 셰이더 속성이 있는 USD 가져오기
* &lbrack;성능&rbrack; 기본적으로 최적화된 레이어 스택 축소판 사용
* &lbrack;성능&rbrack; 프로젝트 파일 열기 시간 및 메모리 사용량 감소(데이터 디코딩)
* VFX 플랫폼 2024 호환
* &lbrack;VFX Platform 2024&rbrack; Python 3.11로 업데이트
* &lbrack;VFX Platform 2024&rbrack; OpenEXR 3.2로 업데이트
* &lbrack;VFX Platform 2024&rbrack; &lbrack;USD&rbrack; OpenSubdiv 3.6.0 업데이트
* &lbrack;VFX Platform 2024&rbrack;&lbrack;Color Management&rbrack; OCIO 2.3.2로 업데이트
* &lbrack;Linux&rbrack; Linux RedHat으로의 마이그레이션
* &lbrack;Linux&rbrack; Nvidia 드라이버 최소 버전을 535.171.04로 업데이트
* &lbrack;가져오기&rbrack; GLTF 메시를 가져올 때 노멀 맵 뒤집기 옵션을 추가합니다
* &lbrack;UI&rbrack; 드래그 이벤트 감지 거리에 운영 체제 기본값 사용
* &lbrack;Substance 엔진&rbrack; 실행 파일에서 기호를 제거하기 위한 호출 스트립 기능 추가
* &lbrack;스플래시 화면&rbrack; 새 스플래시 화면 형식으로 업데이트
* Substance 엔진을 버전 9.1.3으로 업데이트
* &lbrack;Python&rbrack; 레이어 스택 설명서 메뉴에서 예제에 대한 링크를 표시합니다.
* &lbrack;JavaScript&rbrack; Javascript 플러그인을 javascript/플러그인 하위 폴더로 이동

**고정**:

* 특정 경우에 .ai 그래픽이 포함된 UV 타일을 내보내는 &lbrack;Illustrator&rbrack; 충돌
* &lbrack;Roles&rbrack;&lbrack;Path&rbrack; Random per stroke가 패스에서 작동하지 않습니다.
* 타일링이 균일하지 않으면 &lbrack;UI&rbrack;&lbrack;Properties&rbrack; Lock이 활성화됩니다.
* Painter 프로젝트를 두 번 클릭하면 디버그 TXT 파일이 생성됨
* &lbrack;USD&rbrack;&lbrack;Export&rbrack; 일부 텍스처가 누락될 수 있습니다.
* &lbrack;ASM&rbrack; 분산 색상 채널은 금속색을 무시합니다.
* &lbrack;Content&rbrack; 흐림 효과 필터가 &quot;작업&quot; 색상 공간에서 작동하지 않음
* &lbrack;내용&rbrack; Height 조정 필터도 레이어의 알파를 수정합니다

**알려진 문제**:

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;Win&rbrack;&lbrack;충돌&rbrack; &lbrack;ACE&rbrack; sRGB 색상 공간을 디스플레이 변환에 사용하지 않음
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작음
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨
* 일부 사전 설정을 가져올 때 &lbrack;MacOS Intel&rbrack; 충돌
* &lbrack;충돌&rbrack; 자원 재배치 및 프로젝트 저장
* &lbrack;Engine&rbrack; 일반 채널 이동 색상에서 복제 도구로 페인팅이 잘못됨
* &lbrack;Python&rbrack; 고스트 위젯이 여전히 작동하는 스크립트에 의해 삭제된 것으로 나타남
* &lbrack;RedHat&rbrack; 색상 피커 문제

### 10.0.1

출시일: **2024/06/11**&#x200B;요약: **마이너 릴리스, 버그 수정**

**추가됨:**

* &lbrack;Library&rbrack; Substance 글꼴을 일반 글꼴 파일로 변환
* &lbrack;Illustrator&rbrack;&lbrack;SVG&rbrack; 범위 선택 영역에 밝은 회색 배경을 축소합니다.
* &lbrack;Python&rbrack; 사용 가능한 색상 공간을 나열하기 위해 비트맵 소스에 함수 추가

**고정**:

* 다른 폴더로 이동하거나 다른 폴더에서 이동할 때 &lbrack;레이어 스택&rbrack; 폴더가 항상 닫힘
* &lbrack;Save&rbrack; 프로젝트 파일은 &quot;사본으로 저장&quot; 또는 특정 경우에 자동 저장이 실패하면 유실됩니다.
* &lbrack;Import&rbrack; 이름은 같지만 확장명이 다른 에셋은 무시됩니다.
* 이미지 입력에서 고정점을 사용할 때 &lbrack;등록 정보&rbrack; 설정이 누락됨
* &lbrack;Illustrator&rbrack; Painter을 다시 시작하지 않은 경우 서버 충돌 후 Illustrator 파일을 가져올 수 없음
* &lbrack;Python&rbrack; 인스턴스 상위는 &quot;properties&quot; 유형으로 설정할 수 없습니다.
* &lbrack;Python&rbrack; 하이 폴리를 베이킹 매개 변수로 설정해도 하이 폴리가 로드되지 않습니다
* &lbrack;Python&rbrack; set_color_space()에 대한 오류 메시지가 너무 일반적입니다.
* &lbrack;Python&rbrack; 참조 소스가 주기 생성을 허용합니다.

**알려진 문제**:

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작음
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨
* 일부 사전 설정을 가져올 때 &lbrack;MacOS Intel&rbrack; 충돌
* 특정 경우에 .ai 그래픽이 포함된 UV 타일을 내보내는 &lbrack;Illustrator&rbrack; 충돌
* &lbrack;Roles&rbrack;&lbrack;Path&rbrack; Random per stroke가 패스에서 작동하지 않습니다.

### 10.0.0

출시일: **2024/05/16**&#x200B;요약: **주요 릴리스, Python API와 레이어 스택 버전, 기본 Illustrator 파일 읽기, 3D 에셋과 새로운 텍스트 리소스 통합**

**추가됨**:

* &lbrack;Illustrator&rbrack; Painter에서 아트 보드와 함께 Illustrator 파일 사용
* &lbrack;Illustrator&rbrack;&lbrack;SVG&rbrack; 범위 선택에 미리 보기 추가
* &lbrack;Substance 3D Assets&rbrack; Painter에서 직접 3D 에셋 검색, 선택 및 다운로드
* &lbrack;Substance 3D Assets&rbrack;&lbrack;UI&rbrack; 새 패널
* &lbrack;Substance 3D Assets&rbrack; 환경 지도 및 재료 지원
* &lbrack;Substance 3D Assets&rbrack; 새 Substance 3D Assets 패널에서 위치 폴더를 다시 로드하고 탐색하고 열 수 있음
* &lbrack;Substance 3D Assets&rbrack; 다운로드 관리자 추가
* &lbrack;텍스트 리소스&rbrack; 포함 가능한 글꼴 사용 허용
* &lbrack;텍스트 리소스&rbrack; 메시에서 글꼴/텍스트 렌더링 허용
* &lbrack;Text Resource&rbrack; 사용자 및 기타 공유 경로의 글꼴을 에셋 패널에 새 범주로 표시합니다
* &lbrack;텍스트 리소스&rbrack;&lbrack;등록 정보&rbrack; 고급 글꼴 등록 정보 지원 추가
* &lbrack;Text Resource&rbrack; 미니 쉘프의 글꼴 검색/보기 허용
* 호환되지 않는 글꼴을 가져올 때 &lbrack;텍스트 리소스 &rbrack; 오류 메시지/대화 상자 추가
* 기타
* &lbrack;칠 투영&rbrack; 작은 값을 사용할 때 비율 조작기 비헤이비어 개선
* &lbrack;조작기&rbrack; Ctrl 단축키를 누를 때 새로운 정밀 모드를 추가합니다.
* &lbrack;조작기&rbrack; 번역 시 표면 조작기 안정성 향상
* &lbrack;Export&rbrack; SBSAR 출력에 색상 공간 이름 추가
* &lbrack;성능&rbrack; 디스크의 에셋에 대한 라이브러리 검색 시간 향상
* &lbrack;Substance&rbrack; Substance 엔진 버전 9.1.2로 업데이트
* &lbrack;드래그 앤 드롭&rbrack; 뷰포트에 놓을 때 데칼 회전을 카메라에 정렬
* &lbrack;Python&rbrack; 레이어 스택 버전
* &lbrack;Python&rbrack; UI에서 레이어, 효과, 마스크, 지리적 마스크 선택 허용
* &lbrack;Python&rbrack; 레이어 혼합 모드 가져오기/설정 허용
* &lbrack;Python&rbrack; 채우기 레이어 투영 설정을 가져오거나 설정할 수 있도록 허용
* &lbrack;Python&rbrack; 채우기 레이어에서 Substance 재료 색상을 쿼리할 수 있도록 허용
* &lbrack;Python&rbrack; 레이어 및 효과의 균일 색상 및 리소스를 쿼리하고 설정할 수 있도록 허용
* &lbrack;Python&rbrack; 레이어 스택에서 텍스트 리소스 작성 및 편집 허용
* &lbrack;Python&rbrack; 레이어 및 효과의 활성 채널 편집 허용
* &lbrack;Python&rbrack; 일괄 처리 작업으로 한 번의 실행 취소/다시 실행을 허용합니다.
* &lbrack;Python&rbrack; 벡터 소스 매개 변수 로드/편집 허용
* &lbrack;Python&rbrack; 색상 관리를 사용한 레이어 및 효과 색상 속성 편집 허용
* &lbrack;Python&rbrack; 인스턴스 레이어 쿼리 및 만들기 허용
* &lbrack;Python&rbrack; 색상 선택 효과 추가 허용
* &lbrack;Python&rbrack; 비트맵 이미지 색상 관리를 제어할 수 있도록 허용
* &lbrack;Python&rbrack; 일시 중지/일시 중지 취소 허용
* &lbrack;Python&rbrack; 동위 멤버 및 상위 노드로 이동 허용
* &lbrack;Python&rbrack; 필터/생성기 효과 생성 허용
* &lbrack;Python&rbrack; 레벨 효과 추가 허용
* &lbrack;Python&rbrack; 레이어에 스마트 마스크 추가 허용
* &lbrack;Python&rbrack; 고정점 생성/편집 허용
* &lbrack;Python&rbrack; 레이어의 마스크 가져오기/설정 허용
* &lbrack;Python&rbrack; 마스크 비교 효과 만들기 허용
* &lbrack;Python&rbrack; Substance 리소스의 사전 설정 쿼리 및 사용 허용
* &lbrack;Python&rbrack; Substance 리소스에 대한 internal_properties 함수를 통해 사전 설정 및 해당 값을 나열할 수 있도록 허용
* &lbrack;Python&rbrack; 미리 정의된 내보내기 사전 설정을 나열하도록 허용
* &lbrack;Python&rbrack; 라이브러리에서 사용 가능한 내보내기 사전 설정을 나열하도록 허용
* &lbrack;Python&rbrack; 내보내기 사전 설정의 콘텐츠 검색 허용

**고정**:

* &lbrack;충돌&rbrack; Ctrl-Z로 &quot;셰이더 인스턴스 제거&quot; 실행 취소
* &lbrack;충돌&rbrack; 마지막 선택이 효과인 경우 빈 스택에 레이어 만들기
* &lbrack;SVG&rbrack; 사용자 정의 자른 영역 값 문제
* &lbrack;자동 언랩&rbrack; UV 방향을 변경하지 않고 패킹만 다시 계산하면 충돌이 발생합니다.
* &lbrack;드래그 앤 드롭&rbrack; 외부 리소스로 인한 지연이 여러 번 미리 로드됩니다.
* &lbrack;UI&rbrack; 리소스 축소판 끌어서 놓기 시 레이어 스택에서 경고 메시지를 숨길 수 있음
* &lbrack;성능&rbrack; 마스크된 UV 타일은 계속 계산됩니다.
* &lbrack;USD&rbrack; 범위 선택에 대한 잘못된 강조 표시
* 일반 채널에서 페인팅하고 프로젝트를 저장한 후 &lbrack;Resource&rbrack; 비트맵 이미지가 손상됨
* &lbrack;USD&rbrack; 왼손잡이 정점 메시 순서 지원
* &lbrack;Substance&rbrack; 기본값으로 재설정(각도 위젯의 경우 항상 0으로 돌아가기)
* &lbrack;Engine&rbrack; 스텐실에서 SVG을 사용한 페인팅이 작동하지 않습니다.
* 실행 취소 후 &lbrack;엔진&rbrack; 노멀 맵 브러시 획 나누기
* &lbrack;내용&rbrack; 재질 필터에 대한 그래픽의 알파 혼합 및 색상 공간이 잘못됨
* &lbrack;Content&rbrack; Tile Generator 혼합 모드가 작동하지 않음
* &lbrack;Content&rbrack; 막대 그래프 스캔 필터는 경우에 따라 밴딩을 생성합니다.
* &lbrack;Content&rbrack; 스타일화된 구운 조명은 페인팅된 Height을 고려하지 않습니다
* &lbrack;Python&rbrack; 셰이더 변경 후 인스턴스화된 레이어 정보를 검색할 때 예기치 않은 오류가 발생했습니다.
* &lbrack;Save&rbrack; 프로젝트 파일은 특정 경우에 &quot;다른 이름으로 저장&quot;이 실패하면 유실됩니다.

**알려진 문제**:

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;충돌&rbrack;&lbrack;리눅스&rbrack;&lbrack;AMD&rbrack; Wayland OS의 레이어 스택에서 리소스 드래그 앤 드롭
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작음
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨
* &lbrack;Save&rbrack; Spp 프로젝트 파일이 특정 경우에 &quot;사본으로 저장&quot;이 실패하면 유실됩니다.
* 일부 사전 설정을 가져올 때 &lbrack;MacOS Intel&rbrack; 충돌
* &lbrack;Illustrator&rbrack; Painter을 다시 시작하지 않은 경우 서버 충돌 후 Ai 파일을 가져올 수 없음
* &lbrack;Import&rbrack; 이름은 같지만 확장명이 다른 에셋은 무시됩니다.

## 버전 9

### 9.1.2

출시일: **2024/01/30**&#x200B;요약: **마이너 릴리스, 버그 수정**

**추가됨**:

* &lbrack;성능&rbrack; 새 프로젝트에서 첫 번째 채우기 레이어 생성 시간 개선
* &lbrack;성능&rbrack; 대용량 환경 맵의 로드 시간 단축
* &lbrack;Substance&rbrack; 축소판 생성 시에도 프로젝트 저장/닫기 허용

**고정**:

* 뷰포트가 수정될 때 이전 버전 프로젝트에서 저장이 실패함
* &lbrack;충돌&rbrack; 사용자 정의 AO 및 색상 관리를 사용할 때 메시 다시 가져오기
* &lbrack;칠 투영&rbrack; 배율 조작기를 클릭하면 &quot;채색 가능 아님&quot; 메시지가 표시됨
* &lbrack;Brush&rbrack; UV 정렬로 페인팅하면 가공물이 생김
* 스택이 매우 길면 &lbrack;레이어 스택&rbrack; 레이어 이름 바꾸기가 느립니다.
* &lbrack;레이어 스택&rbrack; 마스크에서 호환되지 않는 필터를 사용할 때 잘못된 오류 메시지가 표시됨
* &lbrack;레이어 스택&rbrack; 선택 항목이 삭제 후 다시 상위 레이어로 전환됩니다.
* &lbrack;내보내기&rbrack; 생성된 일반 텍스처는 항상 3D 공간 인접 패딩 모드에 있습니다.
* &lbrack;내보내기&rbrack; 텍스처 알파가 2D 보기 내보내기 사전 설정으로 생성되지 않습니다.
* &lbrack;Export&rbrack; SBSAR 내보내기에서 변환된 맵에 잘못된 사용이 있습니다.
* &lbrack;Shader&rbrack; 셰이더 API 변경 로그가 최신 ASM 변경 사항으로 최신 상태가 아닙니다.

**알려진 문제**:

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;충돌&rbrack;&lbrack;리눅스&rbrack;&lbrack;AMD&rbrack; Wayland OS의 레이어 스택에서 리소스 드래그 앤 드롭
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 HD 화면에서 너무 작음
* &lbrack;충돌&rbrack;&lbrack;Python&rbrack; USD 내보내기가 TextureStateEvent에 의해 트리거됨

### 9.1.1

릴리스 날짜: **2023/12/05**&#x200B;요약: **마이너 릴리스, 버그 수정 및 After Effects으로 보내기 기능**

**추가됨:**

* &lbrack;Interop&rbrack; 텍스처가 입혀진 메쉬를 After Effects(Ae 24.1)로 보낼 수 있도록 허용

**고정:**

* &lbrack;Fill&rbrack; UV 세트를 UV 세트 투영으로 설정한 경우 UV 세트가 2개 이상 읽히지 않습니다.
* &lbrack;충돌&rbrack; 16K 환경 맵 사용
* &lbrack;충돌&rbrack; Exr가 이미지 입력으로 사용됨
* &lbrack;충돌&rbrack; 프로젝트 간에 패스 복사 및 붙여넣기
* &lbrack;QoL&rbrack; 데칼 모드에서 Alpha 리소스를 드래그하여 놓으면 마스크에 UV 투영이 생성됩니다.
* &lbrack;패스(&amp;r); 패스 정점을 복사하면 프로젝트를 다시 열 때 대상 패스 이름도 변경됩니다.
* &lbrack;Linux&rbrack; 색상 선택은 여러 화면으로 끊길 수 있습니다.
* &lbrack;텍스트 밀도 제어의 자동 줄 바꿈 해제&rbrack; UI 문제
* &lbrack;색상 관리&rbrack; UI 피드백은 대소문자를 구분하지만 엔진은 그렇지 않습니다.
* &lbrack;색상 관리&rbrack; 사용자 데이터 재정의가 있는 마스크에서 잘못된 색상 공간 선택

**알려진 문제:**

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* 레이어 스택에 리소스를 드래그하여 놓을 때 AMD의 Linux Wayland가 있는 &lbrack;충돌&rbrack;&lbrack;Linux&rbrack;
* &lbrack;충돌&rbrack;&lbrack;Mac&rbrack; Monterey OS에서 이방성 필터링 값 변경
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 hd 화면에서 너무 작음
* &lbrack;Python&rbrack; 충돌이 TextureStateEvent에 의해 트리거된 USD을 내보냅니다.

### 9.1.0

릴리스 날짜: **2023/11/07**&#x200B;요약: **SVG 및 투명도 지원과 드래그 앤 드롭 및 패스 도구 개선 사항이 포함된 주요 릴리스**

**추가됨:**

* &lbrack;SVG&rbrack; 벡터 파일(SVG) 가져오기 허용
* &lbrack;SVG&rbrack;&lbrack;UI&rbrack; SVG 특정 등록 정보 지원 추가
* &lbrack;SVG&rbrack; 원본 이미지 비율을 쉽게 유지하는 옵션 추가
* &lbrack;SVG&rbrack; 투명도가 있는 SVG 알파 자동 사용 허용
* &lbrack;Interop&rbrack; 텍스처가 입혀진 메쉬를 After Effects(Ae 24.1 beta)로 보낼 수 있도록 허용
* &lbrack;Interop&rbrack; After Effects으로 보내기 설정 추가
* &lbrack;QoL&rbrack;&lbrack;Assets&rbrack;&lbrack;UI&rbrack; UI 슬롯에 드래그하여 놓을 때 에셋 자동 가져오기
* &lbrack;QoL&rbrack; 외부 에셋을 레이어 스택에 끌어다 놓을 수 있음
* &lbrack;QoL&rbrack;&lbrack;레이어 스택&rbrack; 에셋 패널에서 레이어 스택으로 텍스처 드래그 앤 드롭
* &lbrack;QoL&rbrack;&lbrack;Viewport&rbrack; 드래그하여 놓기 생성기, 메쉬의 필터 허용
* &lbrack;QoL&rbrack;&lbrack;Viewport&rbrack; 외부 에셋을 메쉬에 놓기 허용
* &lbrack;QoL&rbrack;&lbrack;Projection&rbrack; UV 세트 투영 모드에 새 UV 세트 추가
* &lbrack;QoL&rbrack; 뷰포트 및 레이어 스택에서 스마트 마스크를 새 레이어로 드래그 앤 드롭
* 마스크에서 사용할 때 여러 출력이 있는 생성기에 대한 선택기 추가(&lbrack;QoL&rbrack;)
* &lbrack;QoL&rbrack; 채우기 효과 위에 단일 채널 이미지 드래그 앤 드롭 허용
* &lbrack;QoL&rbrack;&lbrack;레이어 스택&rbrack; 드래그 앤 드롭과 함께 CTRL/ALT 수정자를 사용하여 효과/레이어를 만들 위치/방법을 지정합니다
* &lbrack;패스(&amp;r); 패스 패널에서 패스 가시성을 개별적으로 전환
* &lbrack;패스&rbrack; 패스 지점에 변형 조작기 사용 허용
* &lbrack;패스&rbrack; 교점당 접선 수동 제어 허용
* &lbrack;패스(&amp;r); 패스 속성 복사/붙여넣기
* &lbrack;패스&rbrack; 브레이크 탄젠트에 빈 단축키 도입
* &lbrack;Shader&rbrack; ASM 셰이더의 불투명도 및 반투명도 지원 추가
* &lbrack;Shader&rbrack; ASM 셰이더가 있는 흡수 색상 채널에 대한 지원 추가
* &lbrack;Shader&rbrack; ASM 셰이더 매개변수 개선 도구 설명
* &lbrack;Shader&rbrack; 반투명도 채널 기본 색상을 검정으로 변경
* &lbrack;표시 설정&rbrack; 기본적으로 임시 안티앨리어싱 활성화
* &lbrack;디스플레이 설정&rbrack; 기본적으로 하위 서피스 분산 설정 활성화
* &lbrack;Substance&rbrack; 그래프 입력/출력에서 ColorSpace 속성에 대한 지원 추가
* &lbrack;Substance&rbrack; Substance 엔진을 버전 9.0.3으로 업데이트
* &lbrack;UI&rbrack; 앱 창이 작더라도 상황별 도구 모음 버튼에 액세스할 수 있게 합니다.
* &lbrack;자동 줄 바꿈 해제&rbrack; 텍스트 밀도가 있는 컨트롤 UV 타일 번호
* &lbrack;Baking&rbrack; 기본적으로 AMD GPU에서 GPU 광선 추적 비활성화
* &lbrack;성능&rbrack; 16비트 이미지에 손실 없는 압축을 적용하여 프로젝트 풋프린트 감소
* &lbrack;Python&rbrack; 3D 보기에서 기본 카메라 조작 허용
* &lbrack;Python&rbrack; 스크립팅을 통해 메시를 내보내는 기능 노출
* &lbrack;Content&rbrack;&lbrack;Samples&rbrack; 새 샘플 프로젝트 &quot;프랑스어 레스토랑 테이블&quot; 추가
* &lbrack;Content&rbrack; Substance 로고 알파를 새 버전으로 업데이트
* &lbrack;Content&rbrack; 3개의 SVG 중심 재질 필터 추가(사용자정의 스티커, 사용자정의 스프레이 및 질감에 그래픽)

**고정:**

* &lbrack;충돌(&amp;r); 대칭 도구를 사용하지 않을 때 조작기 크기 변경
* &lbrack;충돌&rbrack; &lbrack;레이어 스택&rbrack; 아무것도 선택되지 않은 경우 레이어 만들기
* 사용되지 않는 리소스를 제거한 후 &lbrack;프로젝트&rbrack; 메시 맵이 손상될 수 있습니다.
* 이미지를 다시 가져오거나 다시 굽은 후 &lbrack;프로젝트&rbrack; 리소스가 손상됨
* &lbrack;Assets&rbrack; 에셋을 다시 로드하면 즐겨찾기에서 제거됩니다
* 에셋 패널에 &quot;검색 결과 없음&quot;이 있는 경우 &lbrack;Import&rbrack;에서 리소스를 가져올 수 없습니다.
* &lbrack;UI&rbrack; 상황별 도구 모음 화살표가 나타나지 않는 경우가 있습니다
* 부울 값에 대한 &lbrack;Substance&rbrack; 나란히 단추가 지원되지 않습니다.
* &lbrack;Level&rbrack; 마스크에 사용할 때 잘못된 채널 레이블
* &lbrack;Export&rbrack;&lbrack;glTF&rbrack; Painter에서 내보낸 glTF/GLB 파일에는 물리적 크기 단위가 없습니다
* &lbrack;내용&rbrack; 흐림 효과 필터 강도가 16으로 고정됨
* &lbrack;Content&rbrack; 색상 일치 필터 &quot;대상 색상&quot; 이미지 입력이 표시되지 않음

**알려진 문제:**

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* 레이어 스택에 리소스를 드래그하여 놓을 때 AMD의 Linux Wayland가 있는 &lbrack;충돌&rbrack;&lbrack;Linux&rbrack;
* &lbrack;충돌&rbrack;&lbrack;Mac&rbrack; Monterey OS에서 이방성 필터링 값 변경
* &lbrack;충돌&rbrack; Exr가 이미지 입력으로 사용됨
* &lbrack;충돌&rbrack; 16K 환경 맵 사용
* &lbrack;텍스트 밀도 제어의 자동 줄 바꿈 해제&rbrack; UI 문제
* &lbrack;회귀&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 클릭 메뉴가 hd 화면에서 너무 작음
* &lbrack;Python&rbrack; 충돌이 TextureStateEvent에 의해 트리거된 USD을 내보냅니다.
* &lbrack;QoL&rbrack; 데칼 모드에서 Alpha 리소스를 드래그하여 놓으면 마스크에 UV 투영이 생성됩니다.

### 9.0.1

릴리스 날짜: **2023/09/19**&#x200B;요약: **몇 가지 개선 사항이 포함된 부수적인 버그 수정 릴리스**

**추가됨:**

* &lbrack;가져오기&rbrack; 가져오기 창에서 기본 가져오기 위치 설정
* &lbrack;베이킹 모드&rbrack; 매개변수를 기본값으로 재설정할 수 있도록 허용
* &lbrack;Baking&rbrack; 프로젝트 생성 시 베이크를 페인트 해상도로 설정
* &lbrack;대칭&rbrack; 단축키 Q에서 대칭 특정 조작기 바인딩 해제
* &lbrack;Menu&rbrack; 도움말 메뉴에 &quot;로그 표시&quot; 옵션 추가
* &lbrack;뷰포트(&amp;r); 그림자 렌더링 속도 향상
* &lbrack;Substance&rbrack; 엔진을 버전 9.0.1로 업데이트
* &lbrack;색상 관리&rbrack; OCIO 구성 파일은 모든 확장자 유형을 가질 수 있습니다.
* &lbrack;Assets&rbrack; &#39;decal&#39; 사용이 있는 Sbsar 리소스는 뒤틀기 프로젝션으로 자동 설정되어야 합니다.
* &lbrack;Path&rbrack; UI 및 기즈모가 숨겨진 상태에서 패스 도구와 상호 작용하려고 할 때 메시지를 표시합니다

**고정:**

* &lbrack;충돌&rbrack; Alt + 패스 패널 드래그
* &lbrack;리소스 가져오기&rbrack; 가져올 리소스를 제거할 때 임의 충돌
* 압축된 GLB 파일을 가져올 때 충돌 발생
* UV를 공유하는 메시에서 페인팅하는 동안 문제 발생
* 캐시를 다시 계산하거나 로드할 때 메시 플래시 블랙
* &lbrack;등록 정보&rbrack; 매개 변수를 재설정하는 마우스 오른쪽 버튼 클릭 메뉴가 드롭다운에 표시되지 않음
* &lbrack;Level&rbrack; 입력 슬라이더가 이전 레벨로 잠김
* &lbrack;AMD&rbrack;&lbrack;Sparse&rbrack; SVT 옵션(활성화된 경우 아티팩트가 생성됨)
* 정점을 두 번 클릭할 때 나타나는 &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; 충돌
* &lbrack;패스&rbrack; UI 및 패스가 베이킹 모드에서 표시됨
* &lbrack;가시성 재생 시 AMD&rbrack; 텍스처 손실
* &lbrack;Sparse&rbrack; 메시 돌리기 시 해상도가 너무 낮음

**알려진 문제:**

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성

### 9.0.0

릴리스 날짜: **2023/06/20**&#x200B;요약: **3D 곡선, 새 기본 재질, 레거시 재질 정리 및 3D 곡선에 대한 새 사전 설정을 허용하는 페인트가 있는 주요 릴리스**

**추가됨:**

* &lbrack;패스(&amp;r); 패스를 따라 새 페인트 추가 도구
* &lbrack;패스(&amp;r); 패스 도구에 빈 단축키 추가
* &lbrack;패스(&amp;r); 기존 패스에 새 점 추가 허용
* &lbrack;Path&rbrack; 현재 단축키 생성을 종료하려면 경로를 추가합니다.
* &lbrack;패스(&amp;r); 패스에 대한 브러시 속성 편집 허용
* &lbrack;패스&rbrack; 점을 배치할 때 접선을 자동으로 조정
* &lbrack;패스&rbrack; 점이 이동하면 접선 다시 계산
* &lbrack;패스&rbrack; 새로 만든 점을 메시 표면에 스냅
* &lbrack;패스&rbrack; 정점당 압력 편집 허용
* &lbrack;패스&rbrack; 인접 지점에서 새로 만든 점의 압력을 조정합니다.
* &lbrack;패스&rbrack; 점을 매끄러운/모퉁이로 변환 허용(탄젠트 브레이크)
* &lbrack;패스&rbrack; 새로 추가된 점을 즉시 이동할 수 있도록 허용
* &lbrack;패스(&amp;r); 기존 패스에서 점 제거 허용
* &lbrack;패스(&amp;r); 패스 방향을 반전하도록 허용
* &lbrack;패스&rbrack; 뷰포트에서 패스 선택 허용
* &lbrack;패스&rbrack; 선택 윤곽 선택으로 패스 점 선택 허용
* &lbrack;패스&rbrack; 패스의 모든 점을 선택하는 CTRL-A 단축키 도입
* &lbrack;패스(&amp;r); 패스 닫기 허용
* &lbrack;패스&rbrack; 속성에서 패스 위 축 지정 허용
* &lbrack;패스&rbrack; 문맥 도구 모음에 정점 컨트롤 메뉴 추가
* &lbrack;패스&rbrack; 패스 도구에 페인트/지우기/손가락 모드 도입
* &lbrack;Path&rbrack; 뷰포트에 있는 패스에 대한 시각적 피드백 만들기
* &lbrack;Path&rbrack; 경로 방향에 대한 시각적 표시기 추가
* &lbrack;패스(&amp;r); 패스 표시 설정에 선 Thickness 추가
* &lbrack;패스(&amp;r); 패스 숨기기 허용 UI
* &lbrack;패스(&amp;r); 현재 선택된 레이어의 패스를 나열하는 [패스 추가] 패널
* &lbrack;패스(&amp;r); 패스 패널에서 패스 위로 마우스를 가져가면 시각적 피드백을 추가합니다
* 패스 도구를 선택할 때마다 &lbrack;패스(&amp;r); 패스 패널 표시
* &lbrack;패스(&amp;r); 패스 패널에서 패스 이름 바꾸기, 삭제, 복사, 잘라내기, 복제 허용
* &lbrack;Path&rbrack; [패스] 도구를 사용하여 2D 뷰포트에서 상호 작용하려고 할 때 메시지를 표시합니다.
* &lbrack;Library&rbrack; 새 내용 통합(패스 도구 및 기본 재질)
* &lbrack;역동적인 획&rbrack; 역동적인 획에 대한 거리 등록 정보 추가
* &lbrack;역동적인 획&rbrack; 역동적인 획에 크기 및 간격 속성 추가
* &lbrack;역동적인 획&rbrack; 역동적인 획에 대한 시작/중간/끝 등록 정보 추가
* &lbrack;Python&rbrack;&lbrack;USD&rbrack; USD 형식에 대한 프로젝트 구성 매개 변수를 표시합니다.
* &lbrack;Python&rbrack;&lbrack;USD&rbrack; USD 형식에 대한 프로젝트 생성 매개 변수를 표시합니다.
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; 내보낸 USD 파일 내에 프로젝트 경로 정보 추가
* &lbrack;GLTF&rbrack; GLTF 파일을 다시 로드할 때 라이브러리의 텍스처 업데이트
* &lbrack;Shader&rbrack; 방향이 다른 UV 섬에 대한 심 아티팩트 감소
* &lbrack;엔진&rbrack; Substance 엔진 버전 9.0으로 업데이트

**고정:**

* &lbrack;Import&rbrack; 텍스처가 있는 일부 GLB가 Painter에서 텍스처를 가져오지 않음
* 모든 3D 투영 채우기의 테두리에 있는 &lbrack;AMD&rbrack; 가공물
* 레이어 가시성을 전환할 때 &lbrack;엔진&rbrack; 텍스처 중단
* 혼합 모드를 변경하면 일부 위치에서 &lbrack;Engine&rbrack; 텍스처가 비어 있습니다
* 경우에 따라 &lbrack;엔진&rbrack; 텍스처/투영이 빈 뒤틀기 모드입니다.
* 렌더링 저장 시 &lbrack;Array&rbrack; 반복이 0으로 재설정됨
* 파일 > 새로 만들기 작업 시 &lbrack;Log&rbrack; USD 오류 메시지

**알려진 문제:**

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;레이어 스택&rbrack; 입력 소스가 레이어별로 저장되지 않음

## 버전 8

### 8.3.1

출시일: **2023/04/27**

**추가됨:**

* &lbrack;베이킹 모드&rbrack; 뷰포트 시각화를 표시하거나 숨기도록 (빈) 단축키 추가
* &lbrack;베이킹 모드&rbrack; &quot;베이킹 메시 숨기기&quot; 버튼을 사용할 때 항상 낮은 폴리 표시
* &lbrack;베이킹 모드&rbrack; 현재 텍스처 세트에 따른 이름별 일치에 대한 접미어 표시
* &lbrack;Import&rbrack; GLTF 이진 파일(glb)에 대한 지원 추가
* &lbrack;텍스처 세트 목록&rbrack; 셰이더 인스턴스를 선택하거나 만들 수 있는 [추가] 메뉴
* &lbrack;텍스처 세트 목록&rbrack; 텍스처 세트 및 UV 타일 해상도를 빠르게 변경할 수 있음
* &lbrack;물리적 크기&rbrack; UV 투영에서 물리적 크기 사용 시 조작기 동작 개선
* &lbrack;UI&rbrack; 기본 파일 메뉴에 &#39;다른 이름으로 저장&#39; 다시 가져오기
* &lbrack;UI&rbrack; UI 레이아웃에서 보기 선택 항목 저장(2D 전용, 3D 전용, 둘 다)
* &lbrack;USD&rbrack; 지원되지 않는 USD 모양이 있는 프로젝트 생성 시 덜 모호한 오류 메시지
* &lbrack;Python&rbrack; 굽기 진행을 따르기 위한 굽기 이벤트 추가
* &lbrack;Python&rbrack; 베이크 취소 허용
* &lbrack;Python&rbrack; 내보낼 때 파일 유형 및 비트 심도에 대해 &#39;출력 템플릿 기반&#39;을 표시합니다.
* &lbrack;Python&rbrack; TextureStateEvent.Update에 대한 새로 고침 시간 노출

**고정:**

* 프로젝트를 닫을 때 충돌이 드물게 발생하는 &lbrack;충돌&rbrack;
* &lbrack;충돌&rbrack; &lbrack;Baking&rbrack; 특정 프로젝트에서 Height 또는 곡률로 메시 맵 동기화 활성화
* &lbrack;충돌&rbrack;&lbrack;스크립팅&rbrack; 셰이더 충돌 생성 후 재질을 추가할 때의 인스턴스
* &lbrack;베이킹 모드&rbrack; 중립 재질의 AO 강도는 영향을 주지 않습니다.
* 모델이 로드되기 전에 베이킹 모드로 전환할 때 &lbrack;베이킹 모드&rbrack; 충돌
* &lbrack;베이킹 모드&rbrack; [베이킹 프로세스] 탭의 누락 오류 메시지
* &lbrack;베이킹 모드&rbrack; 망 다시 가져오기 후 중립 재료 설정이 영향을 주지 않음
* &lbrack;Baking Mode&rbrack; 뷰 포트 구분 기호는 각 모드가 아닌 전역으로 저장됩니다.
* &lbrack;베이킹 모드&rbrack; 시각화 문제: 평균 표준이 케이지 표면을 변경하지 않음
* &lbrack;색상 관리&rbrack; OCIO env var이 있으면 색상 공간 자동 감지 설정이 비활성화됩니다.
* &lbrack;Content&rbrack; 마스크 윤곽선 필터에 Height 입력의 아티팩트가 있습니다.
* &lbrack;내용&rbrack; 경사 흐림 효과 필터 강도 슬라이더가 1.0으로 고정되어 있습니다.
* &lbrack;Interop&rbrack; Sampler에서 GLTF가 포함된 프로젝트를 만들 수 없음
* &lbrack;레이어 스택&rbrack; 투영 타일링 값이 조작기에서 올바르게 업데이트되지 않음
* &lbrack;Linux&rbrack; HDPI가 100%보다 높은 그래픽 태블릿 펜과 커서 사이의 오프셋
* 프로젝트를 만든 후 메시를 다시 가져올 때 &lbrack;Python&rbrack; 충돌
* 메시를 다시 가져온 후 &lbrack;Substance&rbrack; 3D 노이즈가 끊김
* &lbrack;UV 타일&rbrack; UV 투영에 대한 오프셋이 1로 고정되어 있습니다.
* &lbrack;뷰포트&rbrack; 직선 시각적 피드백이 더 이상 표시되지 않음
* &lbrack;WhatsNew&rbrack; 기능 제목에서 잘못된 줄 반환이 발생함

**알려진 문제:**

* &lbrack;Import&rbrack; 텍스처가 있는 일부 GLB가 Painter에서 텍스처를 가져오지 않음

### 8.3.0

*(릴리스: 2023년 1월 10일*)요약: **새로운 베이킹 모드, USD 파일의 새로운 가져오기 및 내보내기, UV 투영에 대한 물리적 크기 지원이 포함된 주요 릴리스**

**추가됨:**

* &lbrack;베이킹 모드&rbrack; 베이킹 프로세스 전용 새 베이킹 모드

* &lbrack;베이킹 모드&rbrack; 베이킹 모드로 전환할 단축키를 F8로 설정

* &lbrack;베이킹 모드&rbrack; 뷰포트에 베이킹 시작 및 취소 버튼 추가

* &lbrack;베이킹 모드&rbrack; 텍스처 세트 목록에 베이킹 선택 추가

* &lbrack;베이킹 모드&rbrack; 새 메시 맵 베이커 추가 창에서 베이커 선택

* &lbrack;베이킹 모드&rbrack; 새 메시 맵 설정 추가 창에서 베이킹 설정 편집

* &lbrack;굽기 모드&rbrack; 굽기 프로세스를 따르려면 새 [굽기 로그] 창 추가

* &lbrack;베이킹 모드&rbrack; 작업 내역 창에 베이킹 매개변수 추가 및 실행 취소 작업

* &lbrack;베이킹 모드&rbrack; 메시 맵 설정에 탐색 경로 추가

* &lbrack;베이킹 모드&rbrack; 메시 맵 베이커 창에 메시 맵 축소판 추가

* &lbrack;베이킹 모드&rbrack; 3D 뷰포트에서 시각화 설정 축소 가능 메뉴 추가

* &lbrack;베이킹 모드&rbrack; 시각화 설정을 추가하여 하이 폴리 메쉬를 표시하거나 숨깁니다.

* &lbrack;베이킹 모드&rbrack; 케이지 메시 및 와이어프레임을 표시하거나 숨기기 위한 시각화 설정 추가

* &lbrack;베이킹 모드&rbrack; 낮은 폴리 메쉬를 표시하거나 숨기도록 시각화 설정 추가

* &lbrack;베이킹 모드&rbrack; 가시화 설정을 추가하여 UV 이음새가 없는 선명한 가장자리를 오류로 표시

* &lbrack;Baking Mode&rbrack; Baking Log가 표시되지 않는 경우 메시 및 베이크 오류에 대해 뷰포트에 알립니다.

* &lbrack;베이킹 모드&rbrack; 모든 텍스처 세트에서 베이커 설정을 동기화하는 동작 추가

  메시 맵 베이커 창에서 각 베이커 및 공통 설정은 해당 이름 옆에 있는 링크 아이콘을 클릭하여 텍스처 세트 간에 동기화할 수 있습니다. 이 작업을 수행하면 동일한 매개변수를 공유할 텍스처 세트를 선택할 수 있는 창이 열립니다.

* &lbrack;베이킹 모드&rbrack; 동작을 추가하여 베이커 설정 복사 및 붙여넣기

  메시 맵 베이커 창에서 창 상단의 전용 메뉴 또는 마우스 오른쪽 버튼으로 클릭하면 열리는 컨텍스트 메뉴를 통해 각 베이커 설정을 복사하여 텍스처 세트 간에 이동할 수 있는 작업을 사용할 수 있습니다.

* &lbrack;베이킹 모드&rbrack; 오류에서 오른쪽 설정으로 이동하려면 베이킹 로그의 [추가] 단추

  베이커가 실패하거나 메시가 제대로 로드되지 않으면 [베이킹 로그]에 오류 메시지가 나타납니다. 메시지 옆에 있는 버튼을 사용하여 메시 맵 베이커 및 메시 맵 설정 창을 변경하여 관련 설정을 표시할 수 있습니다. 이렇게 하면 문제의 원인을 보다 쉽게 격리하여 해결할 수 있습니다.

* &lbrack;베이킹 모드&rbrack; 텍스처 세트 및 베이커 선택 항목을 관리하는 메뉴 추가

  &quot;텍스처 세트 목록&quot;과 &quot;메시 맵 베이커&quot; 창 모두에 선택 항목을 복사하고 반전할 수 있는 작은 작업 메뉴가 추가되었습니다.

* &lbrack;베이킹 모드&rbrack; 텍스처 세트당 베이커 선택 목록 분할

* &lbrack;베이킹 모드&rbrack; 텍스처 세트당 공통 설정 분할

* &lbrack;베이킹 모드&rbrack; 인터페이스를 고정하지 않고 하이 폴리 및 케이지 메시 로드

* &lbrack;베이킹 모드&rbrack; 뷰 포트 진행 막대를 사용하여 메시 로딩을 표시합니다

* &lbrack;베이킹 모드&rbrack; 베이킹 로그에 메쉬 로딩 상태 추가

* &lbrack;굽기 모드&rbrack; 굽는 동안 뷰포트에서 메시 전환을 허용합니다.

* &lbrack;베이킹 모드&rbrack; 현재 메시 뷰 포트 가시성을 기반으로 베이킹 순서 설정

* &lbrack;베이킹 모드&rbrack; 뷰포트에 암시적 베이킹 케이지 표시

  사용자 정의 케이지 메시 파일을 사용하지 않는 경우 자동 케이지 메시가 생성되어 뷰포트에 표시됩니다. 이 크기는 일반 베이킹 설정에서 최대 정면 거리 매개 변수를 기반으로 합니다. 케이지 메쉬는 낮은 폴리와 높은 폴리 사이의 매칭이 얼마나 멀리 갈 것인지를 나타내기 위해 사용됩니다.

* &lbrack;굽기 모드&rbrack; 굽기 로그에 [이름별 일치]에 대한 일치하는 메시 이름 목록을 표시합니다.

* &lbrack;베이킹 모드&rbrack; 중간 재질을 사용하여 3D 모델을 뷰포트에 표시

* &lbrack;굽기 모드&rbrack; 굽기 모드에서 엔진 계산 비활성화

* &lbrack;베이킹 모드&rbrack; 베이킹이 진행되는 동안 앱을 종료할 때 경고를 표시합니다

* &lbrack;Bakers&rbrack; 앤티 앨리어싱 설정 레이블 업데이트

  앤티 앨리어싱 설정 값의 이름이 &quot;수퍼샘플링&quot;로 바뀌고 해당 동작을 명확히 하기 위해 명시적 승수 번호를 사용하여 바뀌었습니다.

* &lbrack;Bakers&rbrack; 베이커를 버전 2.5.7로 업데이트합니다.

* &lbrack;USD&rbrack; USD(Universal Scene Description) 파일 가져오기 및 내보내기

* &lbrack;USD&rbrack; USD 파일을 선택할 때 새 프로젝트 창에 USD 옵션 추가

* &lbrack;USD&rbrack; 새 범위 및 변형 추가 선택 창

  USD 파일을 가져올 때 새 프로젝트 또는 프로젝트 구성 창에서 변경 버튼을 클릭하면 가져올 USD 파일의 부품 및 변형을 선택할 수 있습니다.

* &lbrack;USD&rbrack; 서브디비전 수준 추가 옵션

  하위 구분이 포함된 USD 메시 파일로 새 프로젝트를 만들 때 슬라이더를 사용하여 하위 구분 레벨을 선택할 수 있습니다. 세분화된 메쉬로 프로젝트가 생성됩니다. 레벨은 프로젝트 구성을 통해 수정자가 될 수 있습니다.

* &lbrack;USD&rbrack; 특정 프레임에서 USD 스킨 메시 가져오기

  애니메이션이 포함된 USD 메시 파일로 새 프로젝트를 만들 때 포함된 프레임 시퀀스를 반영하는 슬라이더를 사용하여 타임라인을 선택할 수 있습니다. 프로젝트 구성을 통해 프레임을 수정자로 지정할 수 있습니다.

* &lbrack;USD&rbrack;&lbrack;Export&rbrack; USD 파일 내보내기 옵션 추가

  텍스처 내보내기 창에 새 USD 내보내기 확인란이 추가되었습니다. 이 옵션을 선택하면 모든 템플릿을 사용하여 텍스처 맵뿐만 아니라 USD 파일도 내보낼 수 있습니다.

* &lbrack;USD&rbrack;&lbrack;Export&rbrack; 메시 내보내기에 USD 파일 형식 추가

* &lbrack;USD&rbrack; 기존 &quot;USD PBR Metal Roughness&quot; 내보내기 사전 설정의 이름을 더 명확하게 바꿉니다

  이전에 &#39;USD PBR 금속 거칠음&#39;으로 알려진 USD 내보내기 텍스처는 내보내기 템플릿 > 출력 템플릿 > USDz(Apple AR)를 통해 계속 액세스할 수 있습니다.

* &lbrack;자동 줄 바꿈 해제&rbrack; 패킹에 대한 잠금 방향 추가

  패킹 기능을 사용할 때 기존 UV 섬의 방향을 유지할 수 있는 자동 줄 바꿈 설정 의 새로운 옵션입니다. 새 프로젝트 > 자동 언랩 옵션 > UV 섬 방향을 통해 액세스할 수 있습니다.

* &lbrack;물리적 크기&rbrack; 채우기 효과/레이어에서 물리적 크기를 자동으로 사용하도록 설정 추가

  물리적 크기가 포함된 재질을 사용할 때 물리적 크기 배율로 자동 전환하는 새로운 옵션이 추가되었습니다. 새 프로젝트 를 통해 또는 재질을 할당할 때 편집 > 프로젝트 구성 > 물리적 크기 > 칠 레이어 비율을 물리적 크기로 전환 을 통해 프로젝트별로 활성화할 수 있습니다.

* &lbrack;물리적 크기&rbrack; UV 투영 물리적 크기 노출

  이제 UV 투영에 물리적 크기 크기 조정을 사용할 수 있습니다. 이를 통해 메시 물리적 크기를 기반으로 재질의 자동 크기 조정이 활성화됩니다. 칠 레이어 또는 효과 속성 창에서 비율 > 물리적 크기를 통해 선택할 수 있습니다.

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 응용 프로그램 버전 쿼리 허용

* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; 새 베이킹 매개변수와 일치하도록 API 업데이트

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 베이킹 모듈: 베이킹 매개변수 편집

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 베이킹 모듈: 베이킹 실행/취소

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 베이킹 모듈: 곡률 방법 선택

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 베이킹 모듈: 베이커/uv 타일 선택

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 베이킹 모듈: 모든 텍스처 세트에서 베이커 설정을 동기화합니다.

* &lbrack;SVT&rbrack; AMD GPU에서 스파스 하드웨어 지원 활성화

  이제 AMD GPU를 사용하여 스파스 가상 텍스처 시스템의 하드웨어 가속을 활성화할 수 있습니다. 이 설정은 일반 환경 설정에서 자동으로 활성화됩니다.

* &lbrack;투영&rbrack; 원통형 투영 매개변수 이름 바꾸기

  &quot;실린더 캡 컬링&quot; 매개변수는 동작을 더 잘 나타내기 위해 &quot;백페이스 컬링&quot;으로 이름이 변경되었습니다. 연결된 툴팁이 적절하게 조정되었습니다.

* &lbrack;프로젝트&rbrack; 프로젝트에 응용 프로그램 버전을 저장하고 스크립팅을 통해 검색합니다.

  버전 8.2 이후 저장 시 응용 프로그램 버전이 spp 파일 내에 저장됩니다. 이 버전 번호는 Python API의 프로젝트 모듈에서 last_saved_substance_painter_version() 함수로 검색할 수 있습니다. 8.2 이전에 만든 프로젝트의 경우 반환된 값은 null입니다.

* &lbrack;Import&rbrack; 3D 모델의 일반적인 가져오기 시간 개선

  메쉬의 일반적인 가져오기 시간을 개선했습니다. 예를 들어, 베이킹을 위해 높은 폴리 메시를 로드할 때 대기 시간을 줄일 수 있습니다. 이러한 최적화는 특히 OBJ 파일 로딩에 적용됩니다.

**고정:**

* &lbrack;충돌&rbrack; 특정 스택으로 필터의 채널 변경

* &lbrack;Mac&rbrack;&lbrack;M1&rbrack; 채우기 레이어를 만들고 레이어 스택에서 나갈 때 충돌

  이 문제는 Mac OS 13(Ventura)으로 업데이트하여 해결할 수 있습니다.

* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 충돌 시 ui.add_dock_widget() 형식이 잘못되었습니다.

* &lbrack;Baking&rbrack; 베이크 실패 시 로그에 불완전한 오류 메시지 표시

* &lbrack;Baking&rbrack; 굽기가 완료되면 메모리가 해제되지 않음

* 효과 가시성을 변경할 때 &lbrack;Engine&rbrack; 텍스처 캐시가 업데이트되지 않음

* &lbrack;Export&rbrack; 2D 보기가 무작위로 균일 맵을 내보냅니다.

* 대형 메쉬로 프로젝트를 저장할 때 &lbrack;Project&rbrack; 메모리 할당 오류 발생

* &lbrack;Viewport&rbrack; TAA는 경우에 따라 페인팅 시 아티팩트를 발생시킨다

**알려진 문제:**

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;레이어 스택&rbrack; 입력 소스가 레이어별로 저장되지 않음

### 8.2.0

*(출시됨: 2022년 10월 6일*)요약: **새로운 온보딩 패널(새로운 시작 패널 및 새로운 기능 패널)이 포함된 주요 릴리스, SBSAR로 내보내기, 폴더에 대한 효과, 삶의 질을 위한 몇 가지 개선 사항 및 버그 수정.**

**추가됨:**

* &lbrack;Onboarding&rbrack; 온보딩 패널에서 신규 사용자를 환영합니다.

  새 CC 사용자가 Painter을 처음 열 때 새 시작 화면이 추가되었습니다.

* &lbrack;Onboarding&rbrack; 새로운 기능 검색 기능을 개선하는 새로운 기능 패널

  새로운 기능 화면이 추가되어 새로운 주요 기능이 표시됩니다. 주요 업데이트 후 Painter이 처음 열릴 때 자동으로 표시되며, [도움말] > [새로운 기능]을 통해 다시 액세스할 수 있습니다.

* &lbrack;Onboarding&rbrack; 이전 시작 파일의 이름을 &quot;홈 화면&quot;으로 바꾸기

  새 시작 화면과의 혼동을 방지하기 위해 이전 시작 화면이 홈 화면으로 이름이 변경되었습니다.

* &lbrack;UI&rbrack; 높은 DPI 화면에 대한 크기 조정 문제 해결

  사용자 정의 디스플레이 비율을 사용하여 HD 화면에서의 Painter UI 적용 성능을 개선했습니다.

* &lbrack;UI&rbrack; UI에서 영구적인 오류 메시지 방지

  이제 이전 프로젝트의 오류 메시지가 아래쪽 상태 표시줄에서 제거됩니다.

* &lbrack;UI&rbrack; 재작업 저장 메뉴

  이제 추가 저장 옵션이 하위 메뉴에 그룹화되고 일부 옵션은 일관성을 위해 이름이 변경되었습니다.

* &lbrack;UI&rbrack; 저장 및 내보내기/공유 UI 레이아웃

  [창] 메뉴에는 UI 레이아웃을 파일에 저장하고 다시 로드하는 새로운 작업이 있습니다. 페인팅 및 렌더링 레이아웃은 별도로 저장됩니다. UI 레이아웃을 저장, 재설정 및 로드하는 다양한 기능이 &quot;substance_painter.ui&quot;에 추가되었습니다.

* 레이어의 혼합 모드/불투명도에 대한 복사/붙여넣기 작업 추가

  레이어의 오른쪽 클릭 메뉴에 새로운 항목인 &#39;혼합 옵션&#39;이 추가되었습니다. 이 기능을 사용하면 한 레이어에서 다른 레이어로 모든 채널의 혼합 모드와 불투명도를 복사하여 붙여넣을 수 있습니다.

* 레이어의 모든 채널에 혼합 모드/불투명도 적용

  레이어의 혼합 모드와 불투명도에 마우스 오른쪽 버튼 클릭 기능을 추가하여 현재 클릭한 설정을 모든 채널에 적용할 수 있습니다.

* 키보드 단축키로 메시 다시 로드(CTRL+SHIFT+R)

  마지막으로 사용 가능한 설정으로 메시 파일을 다시 로드하도록 편집 가능한 단축키를 추가했습니다. 편집 > 메시 다시 가져오기 를 통해 액세스할 수도 있습니다.

* Substance 매개 변수를 기본값으로 재설정

  리소스를 기본값으로 다시 설정할 수 있는 .sbsar 리소스 아래쪽의 속성에 새 단추를 추가했습니다.

* 페인트 브러시를 기본값으로 재설정

  속성의 브러시 섹션에 기본 기본 브러시로 재설정할 수 있는 새 메뉴가 추가되었습니다.

* 마우스 오른쪽 버튼을 클릭하여 개별 Substance 매개 변수를 기본값으로 재설정

  마우스 오른쪽 버튼을 클릭하여 .sbsar 리소스 내의 개별 매개 변수를 재설정할 수 있는 가능성을 추가했습니다.

* &lbrack;에셋 패널&rbrack; &quot;핀&quot; 즐겨찾는 에셋이 에셋 패널 상단에 표시됨

  패널 상단에 즐겨찾기로 핀 할 수 있는 에셋 라이브러리에 대한 새로운 마우스 오른쪽 클릭 옵션을 추가했습니다. 저장된 검색을 통해 즐겨 찾는 모든 에셋을 조회할 수도 있습니다.

* &lbrack;에셋 패널&rbrack; 에셋 삭제, 다시 로드 및 이름 바꾸기

  사용자 라이브러리의 에셋을 삭제하고, 다시 로드하고, 이름을 바꿀 수 있는 마우스 오른쪽 버튼 클릭 메뉴 옵션이 추가되었습니다. 디스크의 라이브러리 위치에서 직접 삭제되고 원래 위치에서 다시 로드됩니다. .abr 또는 .sbsar와 같은 패키지의 일부인 에셋은 개별적으로 편집할 수 없습니다.

* &lbrack;색상 선택&rbrack; 색상 선택 효과에 혼합 모드 추가

* &lbrack;레이어 스택&rbrack; 혼합 모드 및 필터 불투명도 추가

* &lbrack;레이어 스택&rbrack; 칠 레이어/효과에 128보다 큰 타일링 값 허용

* &lbrack;레이어 스택&rbrack; 칠 레이어/효과의 원통형 투영에 대한 원통형 대문자

  이제 채우기 레이어 속성의 원통형 투영에 원통형 대문자 제거 옵션이 제공됩니다.

* &lbrack;Log&rbrack; UV 타일 프로젝트를 만들려고 할 때 메시 부분이 음수 공간에 있으면 오류 메시지를 표시합니다.

  네거티브 스페이스에서 UV 부분이 발견되므로 UV 타일 프로젝트를 만들지 못할 때 보다 명확한 오류 메시지가 추가되었습니다.

* &lbrack;프로젝트&rbrack; 프로젝트를 열 때 &quot;데이터가 너무 최근&quot; 오류 메시지에 버전을 표시합니다.

  너무 최근에 사용한 프로젝트를 열면 오류 메시지에 프로젝트의 버전이 표시되어 올바른 응용 프로그램 버전을 쉽게 식별할 수 있습니다.

* &lbrack;뷰포트&rbrack; 아래에서 메시 밝게 하기

  &quot;로컬&quot;로 설정된 경우 환경 맵 조명을 카메라에 정렬하기 위해 [디스플레이 설정] > [카메라] > [환경 설정]에 새로운 환경 정렬 매개 변수를 추가했습니다.

* &lbrack;Viewport&rbrack; 뷰포트에서 R, G, B 및 Alpha 보기(단독 디스플레이 모드)

  디스플레이 설정 > 뷰포트 설정 > 채널 디스플레이에는 단일 디스플레이 모드에서 채널의 R, G, B 또는 Alpha 구성 요소만 표시할 수 있는 새로운 색상 채널 설정이 있습니다.

* &lbrack;Shader&rbrack; 재질 레이어 셰이더에서 사용자 채널을 RGBA로 설정할 수 있도록 허용

  재질 레이어를 위해 셰이더 내에서 텍스처 세트 채널 구성을 설정할 때 이제 기본값에서 벗어날 채널의 형식을 지정할 수 있습니다. 이를 통해 특히, 회색 음영만 요청하지 않고 색상 사용자 채널을 요청할 수 있습니다.

* &lbrack;Export&rbrack; SBSAR로 텍스처 내보내기 허용

  파일 > 텍스처 내보내기 창을 통해 텍스처를 내보낼 때 SBSAR(Substance 아카이브) 파일 형식을 선택하여 그룹화할 수 있습니다. SBSAR의 콘텐츠는 사용된 출력 템플릿에 의해 구동됩니다. 내보내기 사전 설정에서도 SBSAR 파일 형식을 설정할 수 있습니다. 하이브리드 구성(SBSAR + 기타 형식) 텍스처를 사용하는 경우 SBSAR을 대상으로 하는 그룹이 함께 그룹화되고 나머지는 함께 내보냅니다.

* &lbrack;내보내기&rbrack; EXR 파일 형식에 대한 16비트 노출 옵션

  이제 EXR 텍스처 파일을 내보낼 때 텍스처 내보내기 창(내보내기 설정 및 내보내기 사전 설정 모두)에서 16f비트(절반 부동) 또는 32f비트(부동)를 선택할 수 있습니다. 이전 프로젝트 및 이전 내보내기 사전 설정은 기본적으로 16f 비트로 설정되어 이전 비헤이비어를 반영합니다.

* &lbrack;Python&rbrack; 텍스처 세트가 수정되는 시기를 알 수 있는 이벤트 추가

  새로운 &quot;substance_painter.event.TextureStateEvent&quot;를 통해 페인트 획으로 인해 텍스처 세트가 수정된 시기, 새 채널이 추가되었거나 채널이 제거된 시기를 알 수 있습니다.

* &lbrack;Python&rbrack; 텍스처 세트 설정에서 메시 맵 리소스 가져오기 및 설정 허용

  메시 맵 리소스를 가져오고 설정하는 새로운 기능이 &quot;substance_painter.project&quot; 모듈에 추가되었습니다. 이러한 기능을 사용하여 텍스처 세트 설정에서 참조하는 메시 맵을 업데이트할 수 있습니다.

* &lbrack;Plugins&rbrack; 다른 JS 플러그인을 가져오는 옵션 제거

  JavaScript 플러그인이 더 이상 사용되지 않는 Share 웹 사이트에서 호스팅되었기 때문에 이를 가져오는 옵션이 제거되었습니다.

* &lbrack;내용&rbrack; 새 Roblox 템플릿 추가 및 사전 설정 내보내기

  PBR 텍스처를 Roblox로 더 쉽게 내보낼 수 있도록 새로운 Roblox &quot;재질 변형&quot; 및 &quot;표면 모양&quot; 프로젝트 템플릿과 내보내기 사전 설정이 추가되었습니다. 템플릿은 파일 > 새 프로젝트 창에서 액세스할 수 있습니다.

* Substance 엔진을 마지막 버전(8.6.3)으로 업데이트

* &lbrack;Steam&rbrack; Apple Silicon 칩셋(Apple M1/M2)에 최적화된 빌드

**고정:**

* 16k exr을 사용할 때 충돌

* &lbrack;충돌&rbrack; 셰이더 인스턴스 삭제 후 Ctrl Z

* &lbrack;Iray&rbrack; IoR이 일부 셰이더에 대해 1로 차단됨

* &lbrack;Win&rbrack;&lbrack;Baking&rbrack; 일부 하이 폴리 로드 실패

* &lbrack;색상 관리&rbrack; 필터가 있는 UI의 색상 공간 이름이 잘못되었습니다.

* 가져오기 함수에 의해 반환된 &lbrack;Python&rbrack; 리소스 개체의 유형이 없습니다.

  Python에서 Substance 패키지를 가져올 때 함수가 해당 그래프 대신 패키지를 반환했습니다. 이제 리소스 모듈은 Substance 패키지의 그래프를 검색하는 함수 및 매개 변수를 제공합니다.

**알려진 문제:**

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;레이어 스택&rbrack; 입력 소스가 레이어별로 저장되지 않음
* &lbrack;Painting&rbrack; Temporal 앤티 앨리어스를 사용하면 경우에 따라 아티팩트가 발생합니다
* &lbrack;Export&rbrack; 2D 보기가 무작위로 균일 맵을 내보냅니다.

### 8.1.3

*(릴리스: 2022년 8월 25일*)요약: **보조 버그 수정 릴리스**

**추가됨:**

* Iray SDK 1.6 업데이트

**고정:**

* 이전 잘못된 셰이더가 있는 &lbrack;Shader&rbrack; 충돌
* &lbrack;재질 레이어 구성&rbrack; 프로젝트를 다시 열 때 재질이 사라질 수 있습니다.

**알려진 문제:**

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;레이어 스택&rbrack; 입력 소스가 레이어별로 저장되지 않음
* &lbrack;충돌&rbrack; 셰이더 인스턴스 삭제 후 Ctrl Z
* &lbrack;Iray&rbrack; IoR이 일부 셰이더에 대해 1로 차단됨

### 8.1.2

*(릴리스: 2022년 7월 19일*)요약: **보조 버그 수정 릴리스**

**추가됨:**

* &lbrack;자동 줄 바꿈 해제&rbrack; 세그먼테이션 알고리즘 선택을 위한 새로운 옵션 &quot;유기 메시에 최적화&quot;
* &lbrack;물리적 크기&rbrack; 새 프로젝트 및 프로젝트 구성의 단위 옵션 노출
* &lbrack;색상 관리&rbrack; ACE 사용 시 기본적으로 모니터 표시 사용
* &lbrack;색상 관리&rbrack;&lbrack;Python&rbrack; 프로젝트 생성 시 ACE env-var 사전 설정 파일 고려
* 구성이 변경될 때 새 프로젝트 창에서 색상 관리 설정 재설정(&lbrack; Color Management&rbrack;)
* &lbrack;색상 관리&rbrack; env-var이 있는 경우 OCIO 설정 액세스를 비활성화합니다.
* &lbrack;색상 관리&rbrack; 매개변수가 더 이상 존재하지 않을 때 ACE 설정을 안전하게 업데이트합니다.
* 버전 8.6.0으로 Substance 엔진 업데이트
* &lbrack;내보내기&rbrack; 변위를 지원하는 새 GLTF 내보내기 사전 설정 추가
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 리소스 정보 검색(사용자 정의 메타데이터 포함)
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 텍스처 세트당 메시 이름의 쿼리 목록에 함수 추가
* &lbrack;내용&rbrack; 새 블렌더 템플릿 추가 및 사전 설정 내보내기

**고정:**

* 경우에 따라 Iray를 실행할 때 &lbrack;MacOS&rbrack; 충돌
* &lbrack;축소판(&amp;r); 선반 축소판이 제대로 로드되지 않음
* 여러 UV 채널이 무시됩니다.
* &lbrack;자동 줄 바꿈 해제&rbrack; 긴 섬을 분할할 때 불필요한 계산
* &lbrack;자동 줄 바꿈 해제&rbrack; 옵션은 고려하지 않은 길쭉한 섬을 피합니다.
* &lbrack;자동 줄 바꿈 해제&rbrack; UV 재포장 시 추가 데이터(꼭지점 색상) 손실
* 색상 관리를 사용하는 경우 속성 창의 &lbrack;UI&rbrack; 수평 스크롤 막대
* &lbrack;색상 관리&rbrack; OCIO 구성에 substance_3d_painter_standard_srgb 역할이 없습니다.
* &lbrack;Generator&rbrack; 사용자 데이터를 잘못 사용함 &quot;disabled&quot;
* &lbrack;색상 관리&rbrack; 색상 공간 &quot;호환되지 않음&quot; 드롭다운을 클릭할 수 없습니다.
* &lbrack;색상 관리&rbrack;&lbrack;셰이더&rbrack; sRGB 재정의 정의가 더 이상 작동하지 않습니다
* &lbrack;Generator&rbrack; 사용자 데이터 &quot;disable&quot;의 잘못된 사용
* &lbrack;레이어 스택&rbrack; UV 타일 프로젝트의 깨진 미리 보기
* &lbrack;Shader&rbrack; API 설명서가 표준 구부리기를 사용하여 완전히 최신 상태가 아닙니다.
* &lbrack;Export&rbrack;&lbrack;Interoperability&rbrack; 특수 문자가 있는 Stager로 보낼 수 없음
* &lbrack;내용&rbrack; 일부 브러시 사전 설정 축소판이 비어 있거나 너무 어둡습니다.

**알려진 문제:**

* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성
* &lbrack;레이어 스택&rbrack; 입력 소스가 레이어별로 저장되지 않음
* &lbrack;충돌&rbrack; 셰이더 인스턴스 삭제 후 Ctrl Z
* &lbrack;Iray&rbrack; IoR이 일부 셰이더에 대해 1로 차단됨
* 이전 잘못된 셰이더가 있는 &lbrack;Shader&rbrack; 충돌

### 8.1.1

*(릴리스: 2022년 6월 28일*)요약: **부 릴리스 핫픽스**

**추가됨:**

* &lbrack;레이어 스택&rbrack; 마스크를 Alt로 클릭하면 더 이상 효과가 선택 해제되지 않습니다.

**고정:**

* &lbrack;충돌&rbrack; 단독 보기 모드에서 저장된 이전 프로젝트를 여는 중
* &lbrack;충돌&rbrack; 등록 정보에서 생성기 삭제
* &lbrack;텍스처 설정 설정&rbrack; 일반/앰비언트 오클루전 믹싱 및 일반 방법에 대한 Height이 중단됨
* &lbrack;Export&rbrack; 확산 패딩을 사용하여 내보내기 텍스처는 검정 맵을 렌더링합니다.

**알려진 문제:**

* Monterey에서 Iray를 실행할 때 &lbrack;MacOS&rbrack; 충돌
* &lbrack;미리 보기 축소판&rbrack; 단순화된 축소판은 앵커를 사용할 때 업데이트되지 않습니다
* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성

### 8.1.0

*(출시됨: 2022년 6월 7일*)요약: **ICC 지원이 포함된 주요 릴리스, 물리적 크기 데이터를 기반으로 한 재질 비율, 새로운 베이커, 색상 스포이드 개선 및 추가 콘텐츠의 범위**

**추가됨:**

* &lbrack;색상 관리&rbrack; Adobe Color Engine(ACE)가 있는 ICC 프로필에 대한 지원 추가
* &lbrack;색상 관리&rbrack; ICC의 작업 색상 공간으로 &#39;Adobe 98 RGB&#39;에 대한 지원 추가
* &lbrack;색상 관리&rbrack; 구성 파일을 통해 ACE/ICC 설정 구성 허용
* &lbrack;색상 관리&rbrack; 레거시 모드의 색상 피커에서 선형 색상 값 입력 허용
* &lbrack;색상 관리&rbrack; UI 외부에서 색상을 선택하는 데 사용되는 색상 프로필을 지정할 수 있도록 허용
* &lbrack;색상 관리&rbrack; 뷰포트에서 선택한 마지막 디스플레이 값 기억
* &lbrack;색상 관리&rbrack;&lbrack;Substance&rbrack; 색상 관리에서 생성기/필터가 제대로 작동하도록 만들기
* &lbrack;색상 관리&rbrack;&lbrack;Substance&rbrack; 새 색상 공간 재정의 키워드 추가 $working 및 $standardsrgb
* &lbrack;물리적 크기&rbrack;&lbrack;엔진&rbrack; 메쉬에서 물리적 크기 정보 추출
* &lbrack;물리적 크기&rbrack;&lbrack;엔진&rbrack; 물리적 크기 계산
* &lbrack;물리적 크기&rbrack; UI에서 물리적 크기를 사용하기 위한 노출 옵션
* &lbrack;물리적 크기&rbrack; 뷰포트에 시각적 도우미 추가
* &lbrack;굽기&rbrack; Height 베이커 추가
* &lbrack;굽기&rbrack; 표준 구부리기 추가 베이커
* &lbrack;굽기&rbrack; 불투명도 베이커 추가
* &lbrack;스포이드(&amp;r); 마우스 및 색상 관리 옆에 있는 새로운 색상 스포이드 미리 보기
* &lbrack;스포이드(&amp;r); 색상 피커 패널을 다시 열 때 마지막 위치에 다시 나타납니다
* &lbrack;스포이드(&amp;r); 재료 선택기의 새 아이콘
* &lbrack;스포이드(&amp;r); 색상 피커의 채널 미리 보기 관리
* &lbrack;스포이드(&amp;r); 스포이드에 클릭-선택 기능 추가
* &lbrack;스포이드(&amp;r); 재질 피커가 더 이상 비활성 채널을 활성화하지 않음
* &lbrack;스포이드(&amp;r); 스포이드와 단축키 사용 허용
* &lbrack; 스포이드(&amp;r); 스포이드가 해당하는 경우 관련 채널을 선택합니다.
* &lbrack;스포이드(&amp;r); 색상 피커 모드로 진입하면 모든 단축키가 비활성화됩니다
* &lbrack;스포이드(&amp;r); 16진수 필드의 자동 선택 항목 제거
* &lbrack;스포이드(&amp;r); 재질 피커를 사용할 때 패널을 닫지 않음
* &lbrack;스포이드(&amp;r); 채널을 선택할 수 없을 때 새로운 비활성화 상태
* &lbrack;Export&rbrack; glTF 내보내기에 탄젠트 속성 추가
* Substance 엔진을 v8.4로 업데이트
* 0.9.0으로 자동 줄 바꿈 해제 업데이트
* Qt 5.15.8로 업데이트
* Python 3.9로 업데이트
* &lbrack;Shader&rbrack; 표준 구부리기 음영 지원 추가
* &lbrack;MacOS&rbrack; 3DConnection SpaceMouse 지원
* &lbrack;Python&rbrack; API에 사용된 Python 버전을 문서화합니다
* &lbrack;내용&rbrack; 105개의 사전 설정으로 6개의 새로운 3D 노이즈 추가
* &lbrack;Content&rbrack; 20개의 새로운 그런지 맵 및 2개의 천 주름 패턴
* &lbrack;Content&rbrack; 새 베이커를 사용하도록 &quot;메시 맵&quot; 내보내기 사전 설정 업데이트
* &lbrack;내용&rbrack; 흐림 경사 및 뒤틀기 필터는 텍스처 설정 해상도에 따라 다름
* &lbrack;Content&rbrack; 3개의 새로운 베이커를 사용하도록 샘플 프로젝트 업데이트

**고정:**

* &lbrack;glTF&rbrack; 특수 문자가 있는 glTF를 열 수 없습니다.
* 비등방성 및 SVT가 비활성화된 &lbrack;Engine&rbrack; Artifact
* &lbrack;MacOS&rbrack;&lbrack;M1&rbrack; 스마트 재질이 올바르게 표시되지 않음
* &lbrack;메시 처리&rbrack; Modeler에서 메시를 가져올 수 없습니다.
* 색상 관리가 활성화된 새 프로젝트 창의 &lbrack;UI&rbrack; 가로 스크롤 막대
* 일부 OCIO 구성 시 색상 피커에 &lbrack;색상 관리&rbrack; 작업 영역 값이 없음
* &lbrack;색상 관리&rbrack; 뷰포트의 브러시 미리보기가 색상 관리가 아닙니다.
* &lbrack;SpaceMouse&rbrack; 피벗이 포커스 변경과 함께 즉시 업데이트되지 않으며 때때로 모델을 벗어납니다
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; 내보낸 USD 파일의 구조가 잘못되었습니다.
* 내보낼 때 &lbrack;USD&rbrack; 앰비언트 오클루전 문제
* &lbrack;Content&rbrack; 미리 보기 구 샘플 프로젝트와 일치하도록 축소판의 망을 업데이트합니다.

**알려진 문제:**

* 확산 패딩을 사용하여 텍스처 내보내기 시 검정 맵 렌더링
* 표준/앰비언트 오클루전 믹싱이 중단됨
* 드문 경우지만 Iray를 실행할 때 &lbrack;MacOS&rbrack; 충돌
* &lbrack;미리 보기 축소판&rbrack; 단순화된 축소판은 앵커를 사용할 때 업데이트되지 않습니다
* &lbrack;색상 관리&rbrack; Linux에서 ACE을 사용한 HDR 색상 공간 변환으로 클램프된 색상 생성

## 버전 7

### 7.4.3

*(릴리스: 2022년 4월 11일*)요약: **2D 뷰포트에서 3Dconnection SpaceMouse를 지원하는 버그 수정**

**추가됨:**

* &lbrack;SpaceMouse&rbrack; 2D 뷰포트에서 3DConnection SpaceMouse 지원

**고정:**

* &lbrack;색상 선택기&rbrack;에서 16진수 필드에 쓸 수 없음
* &lbrack;색상 관리&rbrack; 투영 모드에서 사용되는 리소스는 오버레이에서 색상이 관리되지 않습니다
* &lbrack;색상 관리&rbrack; 오류는 로그에 보고되지 않습니다.
* &lbrack;SpaceMouse&rbrack; 사용자에게 SpaceMouse가 없는 경우 일반 오류 메시지를 제거합니다.
* &lbrack;SpaceMouse&rbrack; 프로젝트를 로드할 때 피벗 지점은 항상 숨겨집니다
* &lbrack;Bakers&rbrack; &quot;Average normals&quot; 설정이 UV 타일 프로젝트에 영향을 주지 않음
* &lbrack;UV 타일&rbrack; 다른 타일로 메시를 다시 로드하면 비활성 uv 타일 오버레이가 사라짐
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 원격 스크립팅이 끊어짐
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; API에서 여러 채널을 쿼리할 수 없으며 오류가 발생합니다
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 충돌 시 ProjectEditionEntered 이벤트 사용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 충돌 시 get_active_stack() 호출

**알려진 문제:**

* 3Dconnection SpaceMouse는 MacOS에서 지원되지 않습니다.
* 새 프로젝트 창에 색상 관리가 표시된 &lbrack;UI&rbrack; 가로 스크롤 막대
* &lbrack;Mac M1&rbrack; 스마트 재질이 올바르게 표시되지 않음

### 7.4.2

*(출시됨: 2022년 3월 8일*)요약: **3Dconnection SpaceMouse 및 색상 관리(OCIO) 개선을 지원하는 버그 수정**

**추가됨:**

* &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; 탐색을 위한 3D 뷰포트에서 3D 연결 SpaceMouse 지원
* &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; 3D 뷰포트의 Pro 및 엔터프라이즈 SpaceMouse 모델에 대한 기본 단축키/키
* 3D 뷰포트의 &lbrack;SpaceMouse&rbrack;&lbrack;Windows&rbrack; 전용 회전 중심 아이콘
* &lbrack;색상 관리&rbrack; OCIO 구성의 역할을 사용하여 기본 설정 변경
* &lbrack;색상 관리&rbrack; 색상 관리 색상 위젯의 속성 창
* &lbrack;색상 관리&rbrack; 색상 관리 재질 미리보기에 대한 속성 창
* &lbrack;색상 관리&rbrack; 색상 피커의 색상 견본 관리
* &lbrack;색상 관리&rbrack; 표준 sRGB 색상 공간을 정의하기 위한 설정 추가
* &lbrack;색상 관리&rbrack; 색상 피커 표시 선택기 목록의 OCIO 구성에서 표준 sRGB 색상 공간 추가
* &lbrack;색상 관리&rbrack; 색상 공간 재정의 메뉴 개선
* &lbrack;색상 관리&rbrack; 표시 설정에서 환경 맵 색상 공간 재정의 허용
* &lbrack;색상 관리&rbrack; 현재 디스플레이를 기반으로 색상 피커 그라디언트 그리기
* 기본 색상 편집기의 색상 관리 &lbrack; 색상 관리 &rbrack;
* &lbrack;색상 관리&rbrack; 레거시 모드에서 필터에 통과(색상 공간 없음)를 사용합니다.
* &lbrack;색상 관리&rbrack; &lbrack;0-1&rbrack; 범위와 일치하도록 색상 편집기에 그레이디언트 제한 표시
* &lbrack;색상 관리&rbrack; 레거시 모드의 색상 피커에서 표시 선택기 숨기기
* &lbrack;색상 관리&rbrack; 색상 피커 16진수 필드를 항상 sRGB 색상 공간으로 만듭니다.
* &lbrack;색상 관리&rbrack; 데이터 채널에 대한 색상 피커 표시 드롭다운 비활성화
* &lbrack;최적화&rbrack; 뒤틀기 격자는 가려진 UV 타일만 다시 계산합니다.
* &lbrack;Export&rbrack; Sketchfab, USD 및 glTF에 대한 UV 타일 프로젝트 내보내기 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 톤매핑 함수 변경 허용

**고정:**

* &lbrack;Sketchfab&rbrack; 기존 모델을 업데이트하면 새 모델이 생성됩니다.
* 이전에 업데이트된 모델을 검색할 때 &lbrack;Sketchfab&rbrack; 충돌
* USD으로 내보낼 때 충돌
* 지오메트리 마스크에서 새 셰이더 인스턴스를 만들거나 지오메트리를 숨기는 경우 충돌
* 가져온 리소스 유형을 변경할 때 &lbrack;에셋 가져오기 창&rbrack; 충돌
* 표준 메시 맵이 레이어 스택에서 사용될 때 반전됨
* &lbrack;Substance&rbrack; 사용자 데이터 혼합 모드는 고려되지 않습니다.
* &lbrack;색상 관리&rbrack; 파일 이름에 색상 공간이 있는 비트맵을 UV 타일 시퀀스로 가져옵니다
* Substance 그래프의 색상 관리 출력(&lbrack;Color Management&rbrack;)이 잘못된 색상 공간에 있습니다.
* &lbrack;색상 관리&rbrack; 다각형 채우기 도구가 잘못된 색상을 표시합니다.
* &lbrack;색상 관리&rbrack; ACE 토네마퍼가 단독 모드에 있는 채널에 적용됨
* &lbrack;색상 관리&rbrack; 도구 미리 보기 구 조명이 색상 관리되지 않음
* &lbrack;색상 관리&rbrack;&lbrack;내보내기&rbrack; 변환된 맵은 잘못된 변환을 적용합니다
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack;&lbrack;Color Management&rbrack; 템플릿 및 OCIO 환경 변수로 만든 프로젝트는 레거시 모드에 있습니다.
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 시작할 때 JavaScript 평가 함수를 사용할 수 없습니다
* &lbrack;3D Adobe 오퍼&rbrack;에서 기본적으로 지원되지 않는 언어로 지역 설정을 사용할 때 Painter을 실행할 수 없음

**알려진 문제:**

* 3Dconnection SpaceMouse는 MacOS에서 지원되지 않습니다.
* 새 프로젝트 창에 색상 관리가 표시된 &lbrack;UI&rbrack; 가로 스크롤 막대
* &lbrack;Bakers&rbrack; &quot;Average normals&quot; 설정이 UV 타일 프로젝트에 영향을 주지 않음
* &lbrack;Mac M1&rbrack; 스마트 재질이 올바르게 표시되지 않음
* &lbrack;색상 관리&rbrack; 투영 모드에서 사용되는 리소스는 오버레이에서 색상이 관리되지 않습니다
* &lbrack;색상 선택기&rbrack;에서 16진수 필드에 쓸 수 없음

### 7.4.1

*(출시됨: 2021년 12월 14일*)요약: **색상 관리 개선 버그 수정**

**추가됨:**

* &lbrack;색상 관리&rbrack; 내보낸 파일 이름에 데이터 역할 사용
* &lbrack;색상 관리&rbrack; 새 프로젝트 및 프로젝트 설정 창에서 OCIO을 선택한 경우 기본적으로 색상 관리 섹션을 확장합니다
* &lbrack;색상 관리&rbrack; 레거시 모드에서 ACE Tonemaper 추가
* &lbrack;색상 관리&rbrack; 기본 구성 설정 조정
* &lbrack;색상 관리&rbrack;&lbrack;내보내기&rbrack; 데이터 채널의 파일 이름에 $colorSpace 채우기
* &lbrack;내보내기&rbrack; UV 타일 프로젝트를 Stager로 내보내기
* &lbrack;Interoperability&rbrack; Steam 및 Substance 버전에는 사용할 수 없음
* &lbrack;Interoperability&rbrack; Stager에 UV 타일 프로젝트 보내기 허용

**고정:**

* &lbrack;MacOS&rbrack;&lbrack;충돌&rbrack; Painter이 Catalina로 시작되지 않음
* 사용자 채널에서 데이터 유형/색상 관리를 재생할 때 &lbrack;색상 관리&rbrack;&lbrack;충돌&rbrack; 임의 충돌
* &lbrack;색상 관리&rbrack; 마스크 표시 색상 공간 새 메뉴의 회색 음영으로 사용되는 리소스
* &lbrack;색상 관리&rbrack; 사용자 채널이 레거시 모드 + 솔로 보기의 뷰포트에서 더 어둡게 표시됩니다.
* &lbrack;색상 관리&rbrack; Env 맵은 iRay에서 사용될 때 항상 선형입니다.
* &lbrack;색상 관리&rbrack; 색상 피커가 레거시 모드의 데이터 채널에 적합한 값을 선택하지 않습니다
* 레거시 모드에서 색상 피커(&lbrack;Color management&rbrack;)가 Substance 내에서 중단됨
* &lbrack;색상 관리&rbrack; 드롭다운 메뉴를 사용할 때 뷰포트에서 솔로 채널 보기 간에 전환하면 오른쪽 색상 공간으로 표시되지 않습니다
* &lbrack;색상 관리&rbrack; 내보내기가 레거시 모드의 색상 관리 사용자 채널에 잘못된 변환을 적용합니다
* 단독 보기 마스크에서 만든 획은 재질 보기로 다시 전환할 때 표시되지 않습니다
* &lbrack;내보내기&rbrack; 변환된 맵은 색상 관리 채널로 내보내지지 않습니다.
* 이름이 변경된 사용자 채널에서 원래 이름의 &lbrack;텍스처 Set&rbrack; 도구 설명이 누락됨
* &lbrack;Steam&rbrack; Steam을 사용하여 파일 무결성을 확인할 때 파일이 누락됨

**알려진 문제:**

* &lbrack;Mac M1&rbrack; 스마트 재질이 올바르게 표시되지 않음

### 7.4.0

*(릴리스: 2021년 11월 24일*)요약: **주요 릴리스. 색상 관리의 첫 번째 버전 도입, 2D 또는 3D 보기 고정 해제, 긴 아일랜드를 피하기 위한 자동 UV 언래핑 새로운 옵션, Python API에서 JavaScript 함수 호출 및 새 콘텐츠**

**추가됨:**

* &lbrack;색상 관리&rbrack; 색상 관리 OpenColorIO 버전 2 지원
* &lbrack;색상 관리(&amp;r); 색상 관리 설정을 프로젝트 설정에 추가
* 프로젝트를 열 때 색상 관리 구성 변경에 대한 경고 창(&lbrack; Color Management&rbrack;)
* &lbrack;색상 관리&rbrack; 잘못된 OCIO 구성 파일이 선택된 경우 오류 메시지를 표시합니다
* &lbrack;색상 관리&rbrack; OCIO 환경 변수로 구성 재정의 허용
* &lbrack;색상 관리&rbrack; 응용 프로그램과 기본적으로 통합된 여러 OCIO 구성
* &lbrack;색상 관리&rbrack; 가져온 비트맵 파일 이름에서 색상 공간 이름 추출
* &lbrack;색상 관리&rbrack; 속성 창의 구성에서 색상 공간 하나를 사용하여 색상 공간을 재정의할 수 있습니다.
* &lbrack;색상 관리&rbrack; 텍스처 세트 설정에 색상 관리 옵션 추가
* &lbrack;색상 관리&rbrack;&lbrack;뷰포트&rbrack; 2D 및 3D 뷰를 개별적으로 색상 관리할 수 있도록 허용
* &lbrack;색상 관리&rbrack; 환경 맵을 작업 색상 공간으로 로드 및 변환
* &lbrack;색상 관리&rbrack; 현재 색상 공간으로 색상 피커 및 편집기 조정
* &lbrack;색상 관리&rbrack; 뷰포트의 새로운 색상 드롭다운 메뉴를 사용하여 새 색상 변환을 선택할 수 있습니다.
* &amp;lbrack Color Management&R; Apply display brack;변환 렌더링 결과
* &lbrack;색상 관리&rbrack; 다른 색상 공간으로 텍스처 내보내기
* &lbrack;색상 관리&rbrack;&lbrack;Python&rbrack; 환경 변수(OCIO)의 색상 관리 설정을 새 프로젝트에 적용
* &lbrack;Viewport&rbrack; 2D 또는 3D 뷰포트 고정 해제 허용
* &lbrack;자동 줄 바꿈 해제&rbrack; 길쭉한 섬을 피하는 새로운 옵션
* &lbrack;스크립팅 Python&rbrack; Python API에서 JavaScript 함수 호출
* &lbrack;새 프로젝트 창(&amp;r); 가져온 맵 섹션을 축소할 수 있게 만듭니다.
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; 뒤틀기 설정의 옵션으로 표준 숨기기 허용
* &lbrack;Content&rbrack; 11개의 새로운 그런지 맵
* &lbrack;Content&rbrack; 8개의 새로운 도구 사전 설정(지퍼, 조임 코드, 글리터)
* &lbrack;Content&rbrack; 8가지 새로운 재질(반흔, 주머니, ...)
* &lbrack;Content&rbrack; 1개의 새로운 생성기(부풀리기 shrinkwarp)

**알려진 문제:**

* &lbrack;Mac M1&rbrack; 스마트 재질이 올바르게 표시되지 않음
* 사용자 채널에서 데이터 유형/색상 관리를 재생할 때 &lbrack;색상 관리&rbrack;&lbrack;충돌&rbrack; 임의 충돌
* &lbrack;색상 관리&rbrack; 색상 피커가 레거시 모드의 데이터 채널에 적합한 값을 선택하지 않습니다
* &lbrack;색상 관리&rbrack;&lbrack;Iray&rbrack; 색상 관리가 뷰포트에서 활성화된 상태에서 EXR 또는 TIFF에 렌더링을 저장하면 항상 선형으로 저장됩니다
* 마스크에서 회색 음영으로 사용된 &lbrack;색상 관리&rbrack; 리소스에 잘못된 색상 공간 메뉴가 표시됩니다.
* &lbrack;색상 관리&rbrack;&lbrack;Iray&rbrack; Env 맵은 Iray에서 사용될 때 항상 선형입니다.
* &lbrack;색상 관리&rbrack;&lbrack;내보내기&rbrack; 변환된 맵은 색상 관리 채널로 내보내지지 않습니다.
* &lbrack;색상 관리&rbrack;&lbrack;내보내기&rbrack; 내보내기는 사용자 채널이 색상 관리되거나 레거시 모드가 아닌 경우 무시합니다

### 7.3.1

*(릴리스: 2021년 11월 24일*)요약: **버그 수정**

**추가됨:**

* &lbrack;Projection&rbrack; 크기 조절은 개체 공간에서만 작동해야 합니다.

**고정:**

* &lbrack;Mac M1&rbrack; 재료 레이어가 작동하지 않음
* &lbrack;Mac M1&rbrack;&lbrack;투영&rbrack; 뒤틀기가 작동하지 않음
* 세부 정보가 제대로 표시되지 않음
* &lbrack;투영&rbrack;&lbrack;충돌&rbrack; 이전 버전에서 만든 레이어로 뒤틀기 모드로 전환
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; Flip이 월드 공간으로 설정된 경우 작동하지 않습니다.
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; 분할이 완료된 후 분할 옵션이 선택된 상태로 남아 있음
* &lbrack;Projection&rbrack;&lbrack;UV&rbrack; 투영을 뒤집으면 피벗 포인트가 재설정됩니다.
* &lbrack;Filter&rbrack; 매개 변수를 다시 로드하거나 변경할 때 조명 베이크 환경이 변경됩니다.
* &lbrack;Interoperability&rbrack; Steam 및 Substance 버전에는 사용할 수 없음
* &lbrack;Interoperability&rbrack; &quot;Marketplace에서 3D 에셋 찾아보기&quot; 버튼은 항상 Stock 및 Marketplace 3D 탭에서 CCD를 열어야 합니다

**알려진 문제:**

* &lbrack;Mac M1&rbrack; 스마트 재질이 올바르게 표시되지 않음

### 7.3.0

*(릴리스: 2021년 10월 13일*)요약: **주요 릴리스. 여기에는 새로운 3D 뒤틀기 투영, 새로운 원통형 투영, 색상 피커 개선, Python API의 새로운 기능 및 버그 수정**&#x200B;이 포함됩니다.

**추가됨:**

* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; 3D 뒤틀기를 새로운 투영 모드로 노출
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; 뷰포트에서 드래그 앤 드롭으로 Alpha, 텍스처 및 프로시저에 대해 데칼 모드 허용
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; 데칼 단축키에 뒤틀기 투영 사용(ALT)
* &amp;lbrack&amp;projection&rbrack;&lbrack;뒤틀기&rbrack;뒤틀기&lbrack;뒤틀기&rbrack; 전체 또는 정점당 변환 비틀기 도구 모음&rbrack;
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack;&lbrack;Toolbar&rbrack; 뒤틀기 분할, 수평 또는 수직 옵션을 사용하여 격자 점 추가
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack;&lbrack;Toolbar&rbrack; 재설정 작업을 위한 전용 메뉴
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack;&lbrack;Toolbar&rbrack; 포인트를 이동할 때 접선을 자동으로 조정하는 옵션
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack;&lbrack;Toolbar&rbrack; 격자 에디션 전용 메뉴(크기, 재설정, 색상 및 핸들 크기)
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; 전체 정점 뒤틀기 편집 모드(SHIFT+V)를 전환하는 새 키보드 단축키
* &lbrack;투영&rbrack;&lbrack;뒤틀기&rbrack; Click+Ctrl을 사용하면 서피스 도구와 다른 도구 간에 전환할 수 있습니다.
* &lbrack;Projection&rbrack;&lbrack;Cylindrical&rbrack; 원통형 투영 모드 노출
* &lbrack;투영&rbrack;&lbrack;도구 모음&rbrack; 그룹 조작기 설정(크기, 격자 단계, 각도 단계)
* &lbrack;색상 피커&rbrack; 새 색상 피커 UI
* &lbrack;색상 피커&rbrack; 색상 피커 위젯에서 sRGB 값 사용
* &lbrack;색상 피커&rbrack; 색상 견본 저장 및 삭제 허용
* &lbrack;색상 피커&rbrack; 색상 및 일반 슬롯에서 액세스할 수 있는 스포이드
* &lbrack;색상 피커&rbrack; 0~255개 값 사이의 동적 색상 편집 허용
* &lbrack;색상 선택기&rbrack; HSV/RGB 상태를 앱 전체에서 공통적으로 설정
* &lbrack;색상 피커&rbrack; 색상 피커 창이 반영구적입니다.
* &lbrack;색상 피커&rbrack; Esc를 누르면 색상 피커 창이 닫힘
* UI 상호 작용 및 페인팅 중에 성능 개선
* &lbrack;엔진&rbrack; 새 Substance 엔진 버전(8.3.0)으로 업데이트
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 현재 프로젝트의 메시 다시 로드 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 프로젝트의 리소스 업데이트 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; UV 타일 해상도 설정 및 쿼리 허용
* &lbrack;Interoperability&rbrack; Steam 및 Substance 버전에는 사용할 수 없음
* &lbrack;Interoperability&rbrack; Bridge에서 여러 리소스 받기

**고정:**

* 색상 피커에 올바른 색상이 표시되지 않음
* &lbrack;Baking&rbrack; 텍스처 세트 목록이 올바르게 정렬되지 않음
* &lbrack;FBX import&rbrack; 3ds 최대 그룹 피벗 변환 고려 안 함
* &lbrack;손상된 SBSAR 가져오기가 포함된 Substance 엔진&rbrack; 충돌
* 다른 언어로 된 &lbrack;MacOS&rbrack; 프로젝트 구성 옵션이 없습니다.
* 자동 저장은 긴 프로세스 동안 Painter을 고정할 수 있습니다.

**알려진 문제:**

* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; 분할이 완료된 후 분할 옵션이 선택된 상태로 남아 있음
* &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; Flip이 월드 공간으로 설정된 경우 작동하지 않습니다.
* 드물게 &lbrack;Projection&rbrack;&lbrack;Warp&rbrack; 패치 사이의 가공물 선
* &lbrack;Projection&rbrack;&lbrack;UV&rbrack; 투영을 뒤집으면 피벗 포인트가 재설정됩니다.
* &lbrack;Mac M1&rbrack; 스마트 재질이 올바르게 표시되지 않음
* &lbrack;M1&rbrack;&lbrack;Regression&rbrack; 재료 레이어링 작동하지 않음

### 7.2.3

*(릴리스: 2021년 8월 24일*)요약: **부 릴리스, 버그 수정**

**추가됨:**

* &lbrack;Libraries&rbrack; 크롤링 시 원하지 않는 파일을 제외할 수 있는 방법 추가

**고정:**

* &lbrack;Win&rbrack; 다중 화면 및 절전 문제
* &lbrack;MacOS&rbrack;&lbrack;충돌&rbrack; 효과 사용 시 셰이더 전환
* &lbrack;뷰포트&rbrack; 전체 미리 보기 모드에서 더 이상 알파 없이 브러시 커서가 표시되지 않습니다.
* &lbrack;UI&rbrack; 각도 위젯이 잘못된 방향으로 회전함
* &lbrack;레이어 스택&rbrack; 많은 하위 폴더가 매우 긴 고정을 만듭니다.
* &lbrack;Iray&rbrack; Iray 및 OpenGL의 다른 보기: 작동하지 않으면 표시
* &lbrack;Array&rbrack; 굴절률이 고려되지 않으며 mdl 속성에 나타나지 않습니다.
* &lbrack;JavaScript&rbrack; ShowExportDialog()가 true를 반환하지 않음
* Adobe Stock에서 mtl을 읽을 수 없음

### 7.2.2

*(릴리스: 2021년 7월 27일*)요약: **부 릴리스, 버그 수정**

**추가됨:**

* AMD 드라이버 요구 사항 버전 업그레이드

**고정:**

* &lbrack;Mac M1&rbrack; 잘못된 메모리 감지
* &lbrack;내보내기&rbrack; 매우 긴 경로가 제대로 표시되지 않음

**알려진 문제:**

* &lbrack;Content&rbrack; 샘플의 오래된 셰이드

### 7.2.1

*(릴리스: 2021년 7월 2일*)요약: **부 릴리스, 핫픽스**

**추가됨:**

* &lbrack;Interop&rbrack; Stager에 UV 타일 프로젝트를 전송할 수 없음을 알리는 도구 설명을 추가합니다.
* &lbrack;Plugin&rbrack;&lbrack;UI&rbrack; Livelink 아이콘 업데이트

**고정:**

* &lbrack;30으로 시작하는 Nvidia&rbrack; 드라이버 버전은 오래된 것으로 간주됩니다.
* 프로젝트가 열려 있지 않으면 &lbrack;Libraries&rbrack; 에셋 패널 상태가 저장되지 않습니다.
* &lbrack;Libraries&rbrack; 저장된 새 검색은 저장된 이전 검색의 키워드를 유지합니다.
* &lbrack;Bakers&rbrack;&lbrack;UVTiles&rbrack; meshID당 ID 맵도 UV 타일을 고려합니다
* &lbrack;내보내기&rbrack; gLTF 파일이 정점 색상을 가져오지 않음
* &lbrack;Array&rbrack; 일부 도구 설명 누락
* &lbrack;Interop&rbrack; Stager가 감지되지 않을 때 Stager로 전송이 항상 비활성화되는 것은 아닙니다.
* &lbrack;Resource Updater&rbrack; Photoshop brush maker를 업데이트할 수 없음
* &lbrack;Content&rbrack; 섬유 유리 가장자리 마모 생성기가 고장났습니다

### 7.2.0

*(출시됨: 2021년 6월 23일*)요약: **주요 릴리스, 에셋 패널에 대한 업데이트, 새 채널 및 매개 변수에 대한 액세스를 포함하는 새 셰이더, UI의 전체 새로 고침, 일부 많이 요청된 성능 개선, 확장된 언어 지원 등을 제공합니다!**

**추가됨:**

* &lbrack;라이브러리&rbrack; 셸프를 대체할 새로운 에셋 패널
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; 새 에셋 패널 레이아웃
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; 기본 에셋 패널 방향 및 UI 변경
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; 라이브러리에 목록 보기 옵션 소개
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; 에셋 패널의 새로운 탐색 경로 탐색
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; 저장된 검색을 선택할 때 &quot;모든 라이브러리&quot; 선택
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; 모든 폴더를 선택 해제한 경우 &quot;모든 라이브러리&quot; 선택
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; 입자 브러시용 새 태그
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; 앱에서 &#39;shelf&#39;를 &#39;모든 라이브러리&#39;로 대체함
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; 빈 폴더 숨기기 허용
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; 기본 사용자 라이브러리는 비어 있는 경우에도 표시되어야 합니다.
* &lbrack;Libraries&rbrack;&lbrack;UI&rbrack; 에셋 유형 아이콘을 통한 새로운 필터링 방법
* 여러 에셋 유형을 선택하려면 &lbrack;Libraries&rbrack; 단축키 &quot;CTRL&quot;
* &lbrack;Libraries&rbrack; 에셋 미리보기 메모리 예산을 제어하는 새 환경 변수
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack; 새 환경 맵
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack;&lbrack;UI&rbrack; 기본 재질에서 변위 렌더링
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack; 미리 보기 생성을 위한 기본값으로 ASM(Adobe Standard Material) 셰이더 설정
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack;&lbrack;ASM&rbrack; 새 ASM 셰이더에 대한 새 프로젝트 템플릿
* &lbrack;Libraries&rbrack;&lbrack;Thumbnail&rbrack; 새 Studio 6 환경 맵 사용
* &lbrack;Libraries&rbrack;&lbrack;Thumbnail&rbrack; 생성 대신 리소스에서 축소판 읽기
* &lbrack;Libraries&rbrack;&lbrack;Thumbnail&rbrack; 썸네일 생성에 변위 추가
* &lbrack;텍스처 설정(&amp;r)
* &lbrack;텍스처 세트 설정&rbrack;&lbrack;UI&rbrack; 새 Height을 일반 변환 방법에 노출
* &lbrack;텍스처 세트 설정&rbrack;&lbrack;UI&rbrack; 채널의 UI 구성 재작업
* &lbrack;텍스처 설정(&amp;r); 사용자 채널 제한을 16채널로 증가
* &lbrack;텍스처 세트 설정&rbrack;&lbrack;UI&rbrack; 현재 선택한 셰이더와 호환되는 채널을 나타냅니다
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; 새 Adobe Standard Material 셰이더
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; 비등방성, Clear Coat, 서브서피스 스캐터링, Specular edge color 및 광택에 대한 추가 지원
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; 기본 채널의 색상 값 변경
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack;&lbrack;Export&rbrack; 내보내기 템플릿 Adobe Dimension을 Adobe Substance 3D Stager으로 업데이트했습니다.
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; 셰이더 및 MDL 매개변수에 대한 레이블 및 도구 설명을 추가했습니다.
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; SSS가 지원되지 않더라도 2D 보기에 산란 색상이 표시되도록 합니다
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack;&lbrack;Iray&rbrack; 새 MDL을 사용하여 Iray에서 ASM 셰이더 지원
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack;&lbrack;Iray&rbrack; 레거시 PBR spec gloss &amp; coated에서 업데이트된 서브서피스 스캐터링
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack;&lbrack;Content&rbrack; 샘플의 기본 SSS 유형을 변경했습니다.
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; ASM API에 대한 추가 설명서
* &lbrack;Shader&rbrack;&lbrack;ASM&rbrack; 사용하지 않는 채널을 무시하도록 셰이더를 최적화합니다.
* &lbrack;Shader&rbrack; 새 텍스처 세트 채널 노출
* &lbrack;Shader&rbrack; 향상된 서브서피스 분산
* &lbrack;Shader&rbrack; 일부 셰이더에 대한 새 셰이더 매개 변수를 숨겼습니다.
* &lbrack;Shader&rbrack; 셰이더 매개 변수에 대해 표시
* &lbrack;성능&rbrack;
* &lbrack;Libraries&rbrack; 리소스 미리 보기 로딩 시간 및 계산 성능 개선
* &lbrack;엔진&rbrack; 페인팅 성능 개선
* &lbrack;자동 줄 바꿈 해제&rbrack;
* &lbrack;자동 줄 바꿈 해제&rbrack; 패킹 성능 개선
* &lbrack;자동 줄 바꿈 해제&rbrack; UV 타일 워크플로우와 호환되는 자동 줄 바꿈 해제
* &lbrack;자동 언랩&rbrack; 메시 방향에 따라 UV를 배치하는 새로운 옵션
* &lbrack;Other&rbrack;
* &lbrack;설정&rbrack; 변경된 기본 확대/축소 방향
* &lbrack;UI&rbrack; UI의 전체 새로 고침
* 도움말 메뉴의 &lbrack;UI&rbrack; 재작업
* &lbrack;UI&rbrack; 반전 바꾸기 아이콘
* 플러그인 dcc 링크에 대한 &lbrack;UI&rbrack;&lbrack;Plugin&rbrack; 바꾸기 아이콘
* &lbrack;UI&rbrack;&lbrack;AMD&rbrack; 필요한 최소 버전 및 팝업 메시지 업데이트
* &lbrack;레이어 스택&rbrack; 선택한 빈 폴더 내에 새 레이어 만들기
* Python 설명서 업데이트
* &lbrack;브랜딩&rbrack;
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; 응용 프로그램 이름이 Adobe Substance 3D Painter으로 업데이트되었습니다.
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; 독립 실행형 버전을 &#39;Substance 에디션&#39;으로 업데이트함
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; 응용 프로그램 실행 파일 이름, 설치 경로, 패키지 및 아이콘이 업데이트되었습니다.
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack;의 이름이 기본 라이브러리 및 경로로 변경되었습니다.
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; 창 정보 업데이트됨
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; 업데이트된 시작 화면
* &lbrack;Branding&rbrack;&lbrack;UI&rbrack; 제거된 연도 기반 버전 번호
* &lbrack;Localization&rbrack; 독일어, 프랑스어 및 중국어 간체로 된 새로운 번역
* &lbrack;Interoperability&rbrack; Steam 및 Substance 버전에는 사용할 수 없음
* &lbrack;Interoperability&rbrack; Adobe 에코시스템과의 상호 운용성: Designer, Sampler, Stager 및 Bridge
* &lbrack;Interoperability&rbrack;&lbrack;UI&rbrack; Designer에서 에셋 수신 및 업데이트
* &lbrack;Interoperability&rbrack;&lbrack;UI&rbrack; Sampler에서 에셋 받기
* &lbrack;Interoperability&rbrack;&lbrack;UI&rbrack; Stager로 에셋 보내기
* &lbrack;Interoperability&rbrack;&lbrack;UI&rbrack; Adobe Bridge에 표시
* &lbrack;Interoperability&rbrack;&lbrack;UI&rbrack; Adobe 3D 에셋에 빠르게 액세스할 수 있도록 허용
* &lbrack;Interoperability&rbrack; sbsar의 새로운 사용 태그
* &lbrack;Interoperability&rbrack; 수신된 에셋 유형 처리
* Adobe Substance 3D Designer 또는 Adobe Substance 3D Sampler에서 받은 &lbrack;Interoperability&rbrack; 자산은 사용자가 선택한 기본 라이브러리에 저장됩니다
* &lbrack;Interoperability&rbrack;&lbrack;UI&rbrack; Stager 또는 Photoshop으로 보낼 왼쪽 도구 모음의 새 아이콘

**고정:**

* &lbrack;Tablet&rbrack; 압력 페인팅 시 낮은 성능
* &lbrack;Tablet&rbrack; 슬라이더 컨트롤이 있는 태블릿 문제
* &lbrack;충돌&rbrack; 텍스처 세트 목록과 내보내기 도구 이름이 일치하지 않습니다.
* &lbrack;충돌&rbrack;&lbrack;라이브러리&rbrack; 하위 라이브러리를 두 번 클릭합니다.
* &lbrack;Libraries&rbrack; 라이브러리 디렉터리를 크롤링할 때 발생하는 문제
* &lbrack;Libraries&rbrack; 미리 보기 생성 강제 실행 명령줄이 제대로 작동하지 않습니다.
* &lbrack;Libraries&rbrack;&lbrack;Content&rbrack; Baked Light Environment 필터는 기본적으로 검정색입니다
* &lbrack;Linux&rbrack;&lbrack;MacOS&rbrack;&lbrack;Export Mesh&rbrack; Linux/MacOS에서 만든 glTF를 가져올 수 없습니다.
* &lbrack;Linux&rbrack; 파일을 에셋 패널로 드래그하여 놓으면 충돌이 발생할 수 있습니다
* &lbrack;자동 언랩&rbrack; 자동 언랩은 다시 로드하기 위해 메시를 선택하지 않은 경우에도 사용할 수 있습니다
* &lbrack;파티클&rbrack; 중력이 있는 잘못된 파티클 동작
* &lbrack;레이어 스택&rbrack; 레벨 막대 그래프는 일부 채널에서 광도만 사용할 수 있습니다.
* &lbrack;지오메트리 마스크&rbrack; 지오메트리 마스크 편집 시 폴더의 마우스 오른쪽 클릭 메뉴가 작동하지 않습니다
* &lbrack;투영&rbrack; 구형 투영 및 쌍선형 필터링 연결
* &lbrack;UV 타일&rbrack; 파일로 마스크 내보내기 타일 0, 0만 내보내기
* &lbrack;메시 내보내기&rbrack; FBX 메시 내보내기가 비어 있습니다.
* 렌더링할 때 &lbrack;Array&rbrack; 노멀 맵은 새 프로젝트에 고려되지 않습니다.
* &lbrack;저장&rbrack; 공유 드라이브에 저장 문제
* &lbrack;Baking&rbrack; 수정된 매개변수가 있는 메시를 다시 굽으면 경고가 표시됨
* &lbrack;Baking&rbrack;&lbrack;Regression&rbrack; 높은 폴리 메쉬(poly mesh)의 글로벌 경계 상자에 장면 원점이 포함되지 않은 경우 잘못된 결과가 표시됩니다.
* &lbrack;Python&rbrack; 사용자 정의 사용자 라이브러리는 고려하지 않습니다.

**알려진 문제:**

* &lbrack;Libraries&rbrack; 프로젝트를 열지 않은 경우 저장된 검색이 저장되지 않음
* &lbrack;NVIDIA&rbrack; 드라이버가 최신 버전인 경우에도 오래된 드라이버에 대한 메시지

### 7.1.1 (2021.1.1)

*(출시됨: 2021년 3월 23일*)요약: **마이너 릴리스, 색상 피커에 16진수 값을 입력할 가능성이 있는 버그 수정**

**추가됨:**

* &lbrack;Log&rbrack; 호환되지 않는 AMD GPU 드라이버에 대해 사용자에게 경고
* &lbrack;색상 선택기&rbrack; 16진수 값 입력 허용

**고정:**

* &lbrack;Baker&rbrack; 성능 저하
* &lbrack;형상 마스크&rbrack; 메시 이름을 Alt를 클릭하면 충돌이 발생할 수 있습니다.
* &lbrack;엔진&rbrack; 페인팅이 필요할 때 전체 보기를 새로 고치지 않음
* &lbrack;레이어 스택&rbrack; 셰이더를 변경한 후 선택이 중단됨
* &lbrack;MacOS&rbrack;&lbrack;색상 피커&rbrack; 색상이 선택한 색상과 약간 다릅니다.
* &lbrack;내보내기&rbrack; PSD 파일 형식을 사용하면 UV 타일 당 하나의 파일이 생성되지 않습니다.
* &lbrack;Scripting&rbrack;&lbrack;Javascript&rbrack; alg.mapexport.getPathsExportDocumentMaps() 가 모든 값을 반환하지 않음
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Painter을 다시 열 때 비활성화된 플러그인이 다시 활성화됩니다

### 7.1.0 (2021.1.0)

*(출시됨: 2021년 1월 28일*)요약: **주요 릴리스, 형상의 일부를 선택하고 페인트, 레이어 스택의 효과를 복사/붙여넣기, UV 타일 워크플로 개선, Iray, 베이커, Substance 엔진 및 새 콘텐츠 업데이트**&#x200B;를 수행할 수 있는 새로운 지오메트리 마스크

**추가됨:**

* 새 지오메트리 마스크 및 지오메트리 선택 부분 페인트
* &lbrack;지오메트리 마스크&rbrack; 선택한 지오메트리 부분을 메쉬 이름으로 페인트 허용
* &lbrack;형상 마스크&rbrack; 두 뷰포트의 사각형 선택
* &lbrack;지오메트리 마스크&rbrack; 레이어에서 제외된 지오메트리를 숨기거나 무시하도록 허용
* &lbrack;지오메트리 마스크&rbrack;&lbrack;등록 정보&rbrack; 클릭 및 드래그로 확인란에 대한 빠른 선택
* &lbrack;지오메트리 마스크&rbrack;&lbrack;등록 정보&rbrack;&lbrack;UI&rbrack; 등록 정보 창의 드롭다운이 있는 모두 포함/제외
* &lbrack;지오메트리 마스크&rbrack;&lbrack;등록 정보&rbrack; Alt+왼쪽 클릭으로 목록의 항목 하나를 빠르게 선택할 수 있습니다.
* &lbrack;형상 마스크&rbrack;&lbrack;등록 정보&rbrack; 등록 정보 창에서 메시 이름/UV 타일을 가리킬 때 뷰포트에 오버레이
* &lbrack;지오메트리 마스크&rbrack;&lbrack;레이어 스택&rbrack; 지오메트리 마스크에 복사/붙여넣기 옵션 추가
* &lbrack;지오메트리 마스크&rbrack; 제외된 지오메트리 숨기기/무시의 새 아이콘
* &lbrack;형상 마스크&rbrack; 제외된 형상 숨기기/무시를 위한 새로운 도구 설명
* &lbrack;지오메트리 마스크&rbrack; 키보드 단축키 ALT+H - &quot;제외된 지오메트리 무시&quot; 버튼을 켜거나 끕니다
* &lbrack;UV 타일&rbrack;&lbrack;레이어 스택&rbrack; UV 타일 및 단순화 모드에 대한 새 칠 레이어 구 미리 보기 축소판
* &lbrack;UV 타일&rbrack;&lbrack;레이어 스택&rbrack; UV 타일 마스크를 쉽게 종료할 수 있도록 허용
* &lbrack;UV 타일&rbrack;&lbrack;텍스처 집합 목록&rbrack; UV 타일 당 설명 허용
* &lbrack;Users&rbrack;&lbrack;Texture Set Settings&rbrack;&lbrack;UI&rbrack; 드롭다운 메뉴의 두 개의 새 섹션 제목으로 UV 타일 해상도를 변경합니다.
* &lbrack;UV 타일&rbrack;&lbrack;뷰포트&rbrack; 재질을 뷰포트로 드래그할 때 UV 타일 마스크 종료
* &lbrack;레이어 스택&rbrack; 효과에 대한 복사/붙여넣기 옵션 추가
* &lbrack;레이어 스택&rbrack; 한 텍스처 세트에서 다른 텍스처 세트로 효과 복사/붙여넣기 허용
* &lbrack;레이어 스택&rbrack; 다중 효과 선택 허용
* &lbrack;레이어 스택&rbrack; 레이어 효과에 대한 단축키로 복사/붙여넣기 옵션 추가
* 효과를 다른 레이어로 드래그할 때 마스크와 내용 간을 자동으로 전환하는 &lbrack;레이어 스택&rbrack;
* &lbrack;레이어 스택&rbrack; 다른 레이어에서 마스크를 붙여넣을 때 자동으로 마스크 만들기
* &lbrack;레이어 스택&rbrack; 효과의 문맥상 오른쪽 클릭 메뉴 내에 이동 효과 동작 추가
* &lbrack;레이어 스택&rbrack; 한 레이어에서 다른 레이어로 효과를 드래그하여 놓을 수 있음
* &lbrack;레이어 스택&rbrack; 항목을 폴더로 드래그하면 폴더 맨 위에 항목이 놓입니다
* Iray를 버전 2020.1.0으로 업데이트
* &lbrack;Bakers&rbrack; Bakers를 버전 2.5.4로 업데이트
* &lbrack;Bakers&rbrack; 굽기 진행 창에 개별 UV 타일 표시
* &lbrack;Bakers&rbrack;&lbrack;UI&rbrack; 새 버튼으로 현재 텍스처 세트를 빠르게 굽도록 허용
* &lbrack;Bakers&rbrack; 사용자가 Alt+왼쪽 클릭으로 베이커 중 하나를 빠르게 선택할 수 있도록 허용
* 버전 8.0.8로 Substance 엔진 업데이트
* &lbrack;Substance 엔진&rbrack; 새 .sbsar 파일의 기본 색상 지원
* &lbrack;자동 줄 바꿈 해제&rbrack; 성능 향상
* &lbrack;내보내기&rbrack; 프로젝트의 기본값과 다른 UV 타일의 해상도를 나타내는 시각적 피드백을 추가합니다.
* &lbrack;Export&rbrack; 내보낸 셰이더 json 파일에 장면 크기 계수 추가
* &lbrack;언어&rbrack; 일본어 번역 추가
* &lbrack;UI&rbrack; 내부 종속성 버전 관리를 사용하는 정보 창 업데이트
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 쉘프 리소스 관리 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 프로젝트를 굽고 내보낼 준비가 되면 알 수 있도록 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 셸프가 디스크의 리소스 크롤링을 완료한 시기를 알 수 있도록 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 텍스처 세트당 UV 타일 목록 쿼리 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 사용자 정의 미리 보기를 쉘프 리소스에 할당할 수 있도록 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 사용자 정의 셸프 관리 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 설명서의 각 하위 모듈에 메서드 인덱스를 추가합니다
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 설명서의 새로운 스타일
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 리소스 및 쉘프 설명서 개선
* &lbrack;내용&rbrack; 스티치를 만드는 세 가지 새로운 도구 사전 설정
* &lbrack;Shelf&rbrack; 새 Substance share 플랫폼으로 전환하는 동안 &quot;Substance share으로 내보내기&quot;를 일시적으로 제거

**고정:**

* 해상도가 다른 모니터를 사용할 때 충돌
* 몇 가지 드문 프로젝트와 Substance 엔진 충돌
* 레이어를 전환할 때 제외된 형상 숨기기/무시로 뷰포트 새로 고침이 실패함
* 일부 프로젝트에서 &lbrack;2D 보기&rbrack; 2D 뷰포트가 누락될 수 있습니다.
* &lbrack;Baking&rbrack; &quot;메쉬 이름으로 일치&quot;는 개체의 일부를 무시합니다.
* &lbrack;레이어 스택&rbrack; 레이어 효과를 클릭하면 폴더가 열립니다.
* &lbrack;Geometry Mask&rbrack; UV 타일은 메쉬를 다시 가져올 때도 마스크에서 계산됩니다.
* &lbrack;형상 마스크&rbrack; 뷰포트의 마우스 오른쪽 버튼 클릭 메뉴가 올바른 도구를 제공하지 않습니다.
* 특정 프로젝트에 대한 &lbrack;엔진&rbrack; 대용량 지연
* &lbrack;Scripting&rbrack; Windows에서 원격 JSON POST 요청에 대해 높은 대기 시간
* 특정 통합 GPU에서 &lbrack;Linux&rbrack; Vram 양이 제대로 감지되지 않음
* &lbrack;자동 줄 바꿈 해제&rbrack; 충돌 또는 일부 프로젝트에서 긴 줄 바꿈 해제

## 버전 6

### 6.2.2 (2020.2.2)

*(릴리스: 2020년 9월 28일*)요약: **마이너 릴리스, Python API의 일부 함수가 있는 버그 수정**

**추가됨:**

* &lbrack;성능&rbrack; 색상 ID 선택을 사용할 때 모든 UV 타일을 계산하지 않음
* &lbrack;베이커&rbrack;&lbrack;UI&rbrack; 텍스처 세트 표시 설명
* &lbrack;베이커&rbrack; 베이크 설정 저장 허용
* &lbrack;Bakers&rbrack; [선택] 탭에 [모두 축소/모든 옵션 확장] 추가
* &lbrack;텍스처 세트 목록&rbrack; 비어 있을 때 설명 숨기기
* &lbrack;UV 타일&rbrack;&lbrack;텍스처 집합 목록&rbrack; UV 타일을 클릭하면 목록이 확장/축소됨
* &lbrack;내보내기&rbrack;&lbrack;UI&rbrack; 텍스처 세트 목록 패널의 크기를 가로로 조정할 수 있도록 허용
* &lbrack;Export&rbrack;&lbrack;UI&rbrack; 선택되지 않은 텍스처가 있는 UV 타일 및 텍스처 세트 워크플로우에 대한 일관된 도구 설명 텍스트
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 내보내기 사전 설정을 사용하여 텍스처 내보내기 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 설명서에 변경 로그 추가
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 지정된 스택에서 사용 가능한 모든 채널을 쿼리할 수 있도록 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 콘솔 UI 개선

**고정:**

* &lbrack;AMD&rbrack; 오래된 드라이버 버전의 잘못된 감지
* 경우에 따라 UV 타일 레이아웃이 다른 메시를 다시 가져올 때 충돌 발생
* 매우 무거운 메쉬에서 UDIM이 있는 입자를 사용할 때 충돌
* 경우에 따라 변위 정보가 있는 메시를 내보낼 때 &lbrack;UV 타일&rbrack; 충돌
* &lbrack;내보내기&rbrack;&lbrack;충돌&rbrack; psd 형식으로 2D 보기를 내보내면 충돌이 발생할 수 있습니다.
* 프로젝트를 만들 때 이미지를 시퀀스로 가져오는 기능이 작동하지 않음
* 엔진이 무한 루프에 갇혔다
* 스냅 모드 단축키를 변경할 때 &lbrack;단축키&rbrack; 카메라는 항상 스냅 모드에서 회전합니다.
* 옵션을 해제한 경우에도 다시 가져올 때 메쉬의 래핑이 자동으로 해제됩니다
* &lbrack;텍스처 세트 목록&rbrack; 설명 텍스트 필드가 편집 중에 완전히 표시되지 않는 경우가 있습니다.
* 텍스처 세트 숨기기/숨김 해제를 위한 &lbrack;텍스처 세트 목록&rbrack; 드롭다운 메뉴가 완전히 표시되지 않습니다.
* &lbrack;텍스처 세트 목록&rbrack; 눈 아이콘을 클릭하면 &quot;텍스처 세트 이름 편집&quot;을 입력할 수 없습니다.
* &lbrack;텍스처 세트 설정&rbrack; 채널을 제거하면 아래의 채널도 제거됩니다.
* &lbrack;내보내기&rbrack; 모두 포함 및 모두 재설정 은 UV 타일을 고려하지 않습니다
* &lbrack;Bakers&rbrack; 굽는 동안 선택 해제된 베이커가 나타납니다.
* 입력으로 사용된 베이킹된 맵에 대한 해결 업데이트가 고려되지 않습니다.
* &lbrack;UV 타일&rbrack;&lbrack;뷰포트&rbrack; 3D 뷰포트가 UV 타일 마스크가 선택된 폴더 뒤에 스마트 재질을 추가할 때 멈춤
* &lbrack;Users&rbrack;&lbrack;Viewport&rbrack; UV 타일 통과 모드의 숨겨진 타일에 대해 와이어프레임이 계속 표시됩니다.
* &lbrack;Export&rbrack;&lbrack;Sketchfab&rbrack; &quot;plus&quot; 구독 유형 관련 문제
* 계정 전환 후 &lbrack;Sketchfab&rbrack; &quot;이 자산은 비공개입니다&quot; 확인란이 표시되지 않음
* &lbrack;내보내기&rbrack;&lbrack;내용&rbrack; &quot;흔들기&quot; 브러시 사전 설정으로 인해 성능 문제가 발생할 수 있습니다.
* &lbrack;플러그인 Photoshop&rbrack; 로그 메시지: UV 타일 워크플로우와 호환되지 않음
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; PYTHONPATH env var로 인해 응용 프로그램이 시작되지 않습니다.
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; Typo in Python documentation

### 6.2.1 (2020.2.1)

*(릴리스: 2020년 7월 29일*)요약: **부 릴리스, 핫픽스**

**추가됨:**

* 환경 변수 &quot;SUBSTANCE_PAINTER_VRAM_BUDGET&quot;을 추가하여 GPU VRam 금액을 재정의합니다.
* &lbrack;UV 타일&rbrack;&lbrack;성능&rbrack; 다각형 채우기 도구를 사용할 때 모든 UV 타일을 계산하지 않음

**고정:**

* &lbrack;Iray&rbrack; 저장 렌더링에서 검은색 이미지의 오류 결과를 반환합니다.
* &lbrack;Linux&rbrack; CentOS 7.3의 시작 화면 뒤에 충돌
* &lbrack;Linux&rbrack; 특정 구성에서 Vram 양이 제대로 감지되지 않음
* &lbrack;충돌&rbrack; 중복 텍스처 세트의 이름이 있는 프로젝트 열기
* 마스크를 수정할 때 &lbrack;Engine&rbrack; 캐시 무효화 문제
* &lbrack;텍스처 세트 목록&rbrack; 텍스처 세트가 비활성화되었을 때 잘못된 글꼴 효과 발생

**알려진 문제:**

* &lbrack;텍스처 세트 목록&rbrack; 설명을 숨길 수 없음
* &lbrack;텍스처 세트 목록&rbrack; UI 문제
* &lbrack;Array&rbrack; PSD 렌더링이 열리지 않음
* &lbrack; 플러그인 Photoshop&rbrack; UV 타일 워크플로우와 호환되지 않음

### 6.2.0 (2020.2.0)

*(릴리스: 2020년 7월 23일*)요약: **새로운 UV 타일 워크플로, UV 타일 간 페인트 및 성능 개선이 포함된 주요 릴리스**

**추가됨:**

* UV 타일(UDIM)
* UV 타일 간 &lbrack;UV 타일&rbrack; 페인트
* &lbrack;UV 타일&rbrack; UV 타일에 대한 새 워크플로우 및 기존 워크플로우 중에서 선택할 수 있도록 허용
* &lbrack;UV 타일&rbrack; UDIM/UV 타일 이미지 시퀀스를 리소스로 가져오기
* &lbrack;UV 타일&rbrack; 텍스처 세트 목록 창에서 텍스처 세트당 UV 타일 목록 추가
* &lbrack;UV 타일&rbrack; 텍스처 세트 설정에서 한 번에 여러 UV 타일의 해상도를 편집할 수 있도록 허용
* &lbrack;UV 타일&rbrack;&lbrack;2D 보기&rbrack; UV 타일을 그리드로 표시
* &lbrack;UV 타일&rbrack;&lbrack;2D 보기&rbrack; UV 타일 정보를 표시하거나 숨기는 새 뷰포트 단추
* &lbrack;UV 타일&rbrack; UV 타일 프로젝트에 대해 페인팅 도구를 기본적으로 단일 채널로 전환
* 페인팅 중에 마스킹된 UV 타일을 무시하는 컨텍스트 UV 타일 모음의 &lbrack;Users&rbrack; New 단추
* &lbrack;UV 타일&rbrack;&lbrack;레이어 스택&rbrack; 성능 향상을 위한 새로운 레이어 스택 아이콘
* &lbrack;UV 타일&rbrack;&lbrack;레이어 스택&rbrack; 도구 모음의 페인트 및 채우기 아이콘 개선
* &lbrack;UV 타일 마스크&rbrack;&lbrack;2D 보기&rbrack; 한 번에 여러 UV 타일 포함 또는 제외 허용(왼쪽 클릭, CTRL+왼쪽 클릭)
* &lbrack;UV 타일 마스크&rbrack; 새 아이콘이 있는 레이어당 타일을 포함하거나 제외하는 새로운 UV 타일 마스크
* &lbrack;UV 타일 마스크&rbrack;&lbrack;레이어 스택&rbrack; 모두가 포함되지 않은 경우 UV 타일 마스크 아이콘의 UV 타일 수를 표시합니다
* &lbrack;UV 타일 마스크&rbrack;&lbrack;2D/3D 보기&rbrack; 커서 아래에 UV 타일을 시각화하기 위한 호버 효과 추가
* &lbrack;UV 타일&rbrack;&lbrack;베이커&rbrack; 특정 UV 타일 선택 및 굽기 허용
* &lbrack;UV 타일&rbrack;&lbrack;베이커&rbrack; 텍스처 세트/UV 타일에 대한 선택 옵션 추가
* &lbrack;UV 타일&rbrack;&lbrack;베이커&rbrack; 텍스처 세트 내의 UV 타일을 선택하려면 마우스 오른쪽 버튼을 클릭합니다.
* &lbrack;UV 타일&rbrack;&lbrack;베이커&rbrack; 드래그하여 텍스처 세트/UV 타일에서 빠른 선택을 허용합니다.
* &lbrack;UV 타일&rbrack;&lbrack;베이커&rbrack; 메시 맵에서 &quot;모두&quot; 및 &quot;없음&quot; 단추를 더 명확한 선택 옵션으로 바꾸기
* &lbrack;Users&rbrack;&lbrack;Bakers&rbrack; 구울 UV 타일의 수 표시
* &lbrack;UV 타일&rbrack;&lbrack;내보내기&rbrack; 특정 UV 타일 선택 및 내보내기 허용
* &lbrack;UV 타일&rbrack;&lbrack;내보내기&rbrack; 드래그하여 UV 타일 빠른 선택 허용
* &lbrack;UV 타일&rbrack;&lbrack;내보내기&rbrack; UV 타일에 대한 드롭다운 메뉴 옵션 추가
* &lbrack;Users&rbrack;&lbrack;Export&rbrack; UV 타일에서 작동하지 않는 경우 일부 내보내기 사전 설정을 사용할 수 없도록 설정(Adobe Dimension, Sketchfab, glTF, USD)
* &lbrack;UV 타일&rbrack;&lbrack;내용&rbrack; 새 $udim 태그를 사용하도록 내보내기 사전 설정 업데이트
* &lbrack;UV 타일&rbrack; UV 섬이 겹치는 메시를 가져올 때 오류 보고 개선
* Iray에서 호환되는 &lbrack;UV 타일&rbrack; UV 타일
* &lbrack;Scripting&rbrack;&lbrack;Scripting&rbrack; Python 문서에 UV 타일 내보내기 설명서 추가
* 성능
* 작업 시 엔진 계산을 일시 중지하는 컨텍스트 도구 모음의 새 버튼(&lbrack;Performance&rbrack; New button)(SHIFT+ESC)
* &lbrack;성능&rbrack; 텍스처 세트 캐시 계산을 지연하여 프로젝트를 더 빨리 열기
* &lbrack;성능&rbrack; 프로젝트를 열 때 메시 맵이 로드될 때까지 기다리지 않음
* &lbrack;Performance&rbrack;&lbrack;2D/3D 보기&rbrack; 마스크 채널을 사용하지 않을 때 뷰포트에서 계산하지 않음
* &lbrack;성능&rbrack; 뷰포트에 표시된 메시 맵을 로드할 때 애플리케이션을 차단하지 마십시오.
* &lbrack;성능&rbrack; 프로젝트 저장 시 증분 저장 속도 향상
* &lbrack;Performance&rbrack;&lbrack;Bakers&rbrack; 시간 절약 및 프로젝트 크기 개선을 위해 기본 확장 설정을 변경합니다.
* &lbrack;Performance&rbrack;&lbrack;Bakers&rbrack; 특정 베이커의 회색 음영으로 전환하여 시간 및 프로젝트 크기 절약
* &lbrack;Performance&rbrack;&lbrack;Export&rbrack; 텍스처를 더 빠르게 내보낼 수 있도록 엔진 성능을 개선합니다
* &lbrack;Performance&rbrack;&lbrack;Export&rbrack; 텍스처 세트가 많은 내보내기 대화 상자를 열 때 응답성 향상
* &lbrack;Performance&rbrack;&lbrack;Export&rbrack; &quot;List of Exports&quot; 탭으로 전환할 때 성능 향상
* &lbrack;성능&rbrack;&lbrack;Iray&rbrack; Iray 시작 시간 단축
* 기타
* &lbrack;베이커&rbrack; 텍스처 세트의 선택 옵션 추가
* 셰이더 인스턴스 관리를 텍스처 집합 설정으로 이동
* &lbrack;2D/3D 보기&rbrack; 뷰 포트 하단에 편집된 마스크 유형을 나타내는 메시지 추가
* 기존 축소판과 새 축소판 사이를 전환하는 설정의 새로운 옵션(&lbrack;레이어 스택&rbrack;)
* &lbrack;레이어 스택&rbrack; 축소판의 로딩 상태를 나타내는 시각적 피드백을 추가합니다.
* &lbrack;Proj&rbrack; 이미지 시퀀스를 로드하는 새로운 투영 모드 &quot;칠(UV-타일에 따라 일치)&quot;
* &lbrack;Proj&rbrack; 특정 경우 칠 레이어 투영 모드를 &quot;칠(UV-타일에 따라 일치)&quot;로 변경
* &lbrack;내용&rbrack; 성능 향상을 위한 목탄 브러시 사전 설정 최적화
* Iray를 버전 2020.0.0으로 업데이트
* &lbrack;내보내기&rbrack; 아무것도 선택되지 않은 경우 내보내기 목록 비활성화 탭
* 자동 줄 바꿈 해제
* &lbrack;자동 줄 바꿈 해제&rbrack; 자동 줄 바꿈 해제 프로세스의 성공률 향상
* &lbrack;자동 줄 바꿈 해제&rbrack; 속도와 안정성을 높이기 위한 개선된 매개 변수화

**고정:**

* &lbrack;Alembic&rbrack; 파일을 가져올 때 얼굴 세트가 무시됩니다.
* &lbrack;Alembic&rbrack; 특정 파일의 무한 로드 시간
* &lbrack;Import&rbrack; 파일 확장자만 다른 경우 잘못된 UDIM 이미지 시퀀스를 가져옵니다
* &lbrack;충돌&rbrack; 다른 프로세스에 의해 잠긴 프로젝트를 열려고 하면 충돌이 발생합니다.
* &lbrack;Projection&rbrack; 삼면형 투영을 사용할 때 복제된 메쉬의 가공물
* &lbrack;Export&rbrack; 방출 채널을 USD 포맷으로 내보낼 수 없습니다.
* &lbrack;Content&rbrack; 스마트 재질 &quot;Charcoal&quot;에 페인트 선 포함

**알려진 문제:**

* &lbrack;텍스처 세트 목록&rbrack; 설명을 숨길 수 없음
* &lbrack;텍스처 세트 목록&rbrack; UI 문제

### 6.1.3 (2020.1.3)

*(릴리스: 2020년 6월 16일*)요약: **버그 수정**

**추가됨:**

* &lbrack;Export&rbrack; 셰이더 매개 변수 json 파일에 변위 설정 추가

**고정:**

* 기존 충돌을 지우고 바꾸려고 할 때 &lbrack;channel&rbrack;&lbrack;Engine&rbrack; 충돌
* &lbrack;충돌&rbrack; 재료 레이어링 시 마스크를 페인트한 후 셰이더를 변경하는 중
* 대용량 프로젝트가 포함된 &lbrack;충돌&rbrack;&lbrack;엔진&rbrack; 충돌
* &lbrack;Bakers&rbrack; 이름별 일치 기능이 zBrush에서 내보낸 OBJ에서 작동하지 않음
* &lbrack;변위&rbrack;&lbrack;SVT&rbrack; 텍스처가 켜져 있을 때 프로젝트 열림 시 변위가 표시되지 않습니다
* &lbrack;내보내기&rbrack; 일부 텍스처는 균일 회색으로 내보내집니다.
* &lbrack;Export&rbrack; 비활성화된 텍스처 세트는 Dimension 및 Sketchfab 내보내기 사전 설정에 대해 내보내서는 안 됩니다.
* JavaScript API를 사용하여 onProjectOpened 이벤트의 내보내기 구성에 액세스하는 동안 &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; 충돌
* &lbrack;Scripting&rbrack;&lbrack;Javascript&rbrack; onExportFinished()가 내보내기 후 호출되지 않습니다.

### 6.1.2 (2020.1.2)

*(릴리스됨: 2020년 5월 28일*)요약: **Substance 엔진 및 베이커 업데이트가 포함된 버그 수정**

**추가됨:**

* &lbrack;Bakers&rbrack; 최신 버전으로 업데이트
* &lbrack;Bakers&rbrack; 앰비언트 오클루전, 곡률, Thickness 베이커의 새로운 샘플링 방법
* 최신 버전의 Substance 엔진으로 업데이트
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 프로젝트 리소스에 대한 ResourceID 생성 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 채널 정보 쿼리 허용
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; 텍스처 내보내기를 시뮬레이션하는 dryrun 및 콜백 함수 추가

**고정:**

* &lbrack;Bakers&rbrack; 특정 경우에 탄젠트 노멀 맵을 사용하는 월드 스페이스 표준 베이커의 표준이 잘못되었습니다.
* &lbrack;Bakers&rbrack; 높은 폴리가 없을 때 Optix에서 앰비언트 오클루전 베이킹 오류
* 특정 텍스처 세트를 로드할 때 &lbrack;역동적인 획&rbrack; 지연
* &lbrack;Export&rbrack;에서는 USD, glTF에 대해 비활성화된 텍스처 세트를 내보내지 않아야 합니다.
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; 새 Curvature baker 설정을 편집할 수 없습니다.
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; alg.texturesets.addChannel() 이 오류를 반환하지 않는 경우가 있습니다.
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; setProjectExportOptions()에 대한 Javascript API 설명서의 Typo
* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; 항상 모든 텍스처 세트 내보내기
* &lbrack;Scripting&rbrack;&lbrack;Python&rbrack; sys.executable이 Substance Painter 대신 python.exe에 대한 경로를 반환합니다.
* Mac OS 및 Windows/Linux에서 텍스처 캐시가 호환되지 않음
* &lbrack;Livelink UE4&rbrack; 조합 메쉬의 모든 텍스처 세트에는 마지막 재질만 사용됩니다.

**알려진 문제:**

* &lbrack;Export&rbrack;&lbrack;Dimension&rbrack;&lbrack;Skecthfab&rbrack; 비활성화된 텍스처 세트를 내보내면 안 됩니다.
* &lbrack;충돌&rbrack; 재질 레이어링 시 마스크를 페인트한 후 셰이더를 변경합니다

### 6.1.1 (2020.1.1)

*(릴리스: 2020년 5월 5일*)요약: **핫픽스**

**추가됨:**

* &lbrack;Export&rbrack; TextureSet에서 재정의된 상태 시각적 피드백

**고정:**

* &lbrack;내보내기&rbrack; 내보내기 도구 창 크기가 특수 해상도 모니터에서 너무 커서 크기를 조정할 수 없습니다.
* &lbrack;내보내기&rbrack; 옵션이 내보내기 후 저장되지 않음
* &lbrack;Export&rbrack; 충돌 또는 &quot;캐시에서&quot; 내보내기 사전 설정으로 내보낼 수 없음
* &lbrack;Export&rbrack; 내보내기를 취소하면 예기치 않은 추가 빈 맵이 생성됩니다
* &lbrack;내보내기&rbrack; 가상 내보내기 사전 설정 수정
* &lbrack;Python&rbrack; PYTHONPATH env var은 고려되지 않습니다.
* &lbrack;Python&rbrack;&lbrack;Export&rbrack; Python을 통해 내보내기를 취소하면 예외 오류가 반환됩니다.
* &lbrack;Python&rbrack;&lbrack;Export&rbrack; export_project_users psd 파일 형식의 잘못된 결과
* &lbrack;Bakers&rbrack; GPU 광선 추적 포함 Linux 충돌

**알려진 문제:**

* &lbrack;JavaScript&rbrack;에서 새 곡률 베이커 설정을 편집할 수 없음
* &lbrack;JavaScript&rbrack;&lbrack;Export&rbrack; 항상 모든 텍스처 세트 내보내기
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; 비활성화된 텍스처 세트를 내보내서는 안 됩니다.
* &lbrack;충돌&rbrack; 재질 레이어링 시 마스크를 페인트한 후 셰이더를 변경합니다

### 6.1.0 (2020.1.0)

*(출시됨: 2020년 4월 22일*)요약: **새로운 텍스처 및 메시 내보내기 도구(변위 및 테셀레이션 포함)과 함께 주요 릴리스, 더 많은 컨트롤로 UV 언래핑 업데이트, 새로운 베이커, 새로운 스크립팅 python API, 데칼 프로젝션 및 새로운 콘텐츠에 대한 더 나은 UX**

**추가됨:**

* 새로운 텍스처 및 메시 내보내기 도구
* &lbrack;내보내기&rbrack; 새 내보내기 도구 인터페이스
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; 텍스처 세트당 내보낼 맵 채널을 선택할 수 있습니다.
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; 한 번의 작업으로 모든 텍스처 세트의 텍스처 세트 크기를 수정할 수 있습니다
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; 텍스처 세트별로 다른 템플릿 허용(USD, glTF, Sketchfab 및 Dimension 제외)
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; 지도 및 텍스처 세트의 빠른 활성화 및 비활성화
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; 내보내기 해상도 8192x8192 더 이상 실험적이지 않음
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; 맵당 파일 형식 및 비트 심도 수정 허용
* &lbrack;Export&rbrack;&lbrack;Export tab&rbrack; 기본 매개변수 값으로 재설정 허용
* &lbrack;내보내기&rbrack;&lbrack;내보내기 탭&rbrack; 내보내기 없이 설정 저장 허용
* &lbrack;내보내기&rbrack;&lbrack;출력 템플릿 탭&rbrack; &quot;구성&quot; 탭의 이름을 &quot;출력 템플릿&quot; 탭으로 변경
* &lbrack;내보내기&rbrack;&lbrack;출력 템플릿 탭&rbrack; 사전 설정 맵당 파일 형식 및 비트 심도 정의 허용
* &lbrack;Export&rbrack;&lbrack;내보내기 목록 탭&rbrack; 내보내기 프로세스를 요약하고 보는 새 미리 보기 탭
* &lbrack;메시 가져오기/내보내기&rbrack; 가져오기/내보내기 시간 성능 최적화
* &lbrack;메시 내보내기&rbrack; FBX에서 메시 내보내기
* &lbrack;메시 내보내기&rbrack; 변위 및 테셀레이션을 사용한 메시 내보내기
* &lbrack;메시 내보내기&rbrack;&lbrack;UI&rbrack; 일반 정점을 다시 계산하기 위한 새로운 설정, 삼각 측량 적용
* &lbrack;메시 내보내기&rbrack; 자동 래핑 해제로 생성된 새 UV로 원래 메시 토폴로지를 내보냅니다
* 더 많은 컨트롤로 업데이트된 자동 UV 감싸기
* &lbrack;UV Unwrapping&rbrack;&lbrack;UI&rbrack; 새 프로젝트 창에서 자동 UV Unwrapping을 활성화하는 설정 추가
* &lbrack;UV Unwrapping&rbrack;&lbrack;UI&rbrack; 감싸기 해제 단계(이음새, 감싸기 해제, 패킹)를 제어하는 새로운 옵션
* &lbrack;UV 언랩&rbrack;&lbrack;UI&rbrack; 기존 언랩/언랩/패킹 보존 허용
* &lbrack;UV Unwrapping&rbrack;&lbrack;UI&rbrack; 감싸지 않은 단계를 완전히 다시 계산하는 새로운 옵션
* &lbrack;UV Unwrapping&rbrack;&lbrack;UI&rbrack; 여백 크기(없음, 소, 중 및 대)를 제어하는 새 옵션
* 뉴베이커
* &lbrack;Bakers&rbrack; 이전 곡률을 메쉬의 새 곡률로 바꾸기
* &lbrack;Bakers&rbrack; &quot;앰비언트 오클루전&quot; baker에서 백페이스를 무시하려면 이름순으로 일치 옵션 추가
* &lbrack;Bakers&rbrack; &quot;앰비언트 오클루전&quot; baker에 접지면 추가 옵션
* 새로운 스크립팅 Python API(3.7.6)
* &lbrack;Python&rbrack;&lbrack;UI&rbrack; Python에 대한 새로운 스크립팅 메뉴
* 도움말 메뉴의 &lbrack;Python&rbrack;&lbrack;UI&rbrack; 새로운 Python 설명서
* &lbrack;Python&rbrack; Substance Painter python 모듈 노출: substance_painter, alg, display, project.setting, project, texturesets, ui
* &lbrack;Python&rbrack; 새로운 &quot;substance_painter&quot; Python 모듈 노출
* &lbrack;Python&rbrack; 새로운 Python 하위 모듈 노출: alg, display, log, project, resource, texturesets, ui
* 프로젝트 변경 사항에 대한 &lbrack;Python&rbrack; 수신기
* &lbrack;Python&rbrack; Python 설명서의 새로운 예
* &lbrack;JavaScript&rbrack;&lbrack;UI&rbrack; 플러그인 메뉴가 JavaScript로 대체됨
* &lbrack;Viewport&rbrack; 선반에서 리소스를 &quot;드래그/드롭 + ALT&quot;하여 데칼 투영을 만들 수 있습니다.
* 새 콘텐츠
* &lbrack;Content&rbrack; Substance Source의 5가지 새로운 데칼 재질
* &lbrack;Content&rbrack; 새 프로젝트 템플릿 추가 및 Maxwell 렌더러용 내보내기 사전 설정
* &lbrack;Content&rbrack; Keyshot 9 내보내기용 프로젝트 템플릿 추가
* &lbrack;Content&rbrack; 변위 및 방출을 지원하도록 Keyshot 9 내보내기 사전 설정 업데이트
* &lbrack;Content&rbrack;&lbrack;내보내기 도구&rbrack; 게임 엔진 및 렌더러의 최신 버전과 일치하도록 모든 내보내기 사전 설정 업데이트
* &lbrack;Content&rbrack;&lbrack;Content&rbrack; 내보내기 도구&rbrack; 내보내기 사전 설정 파일을 업데이트하여 새로운 형식 및 디더링 설정을 사용합니다.
* &lbrack;Content&rbrack; VRay 재질(VRayMtl)을 지원하는 새로운 템플릿 및 셰이더들
* &lbrack;레이어 스택&rbrack; 휴지통 아이콘 또는 키보드 단축키 삭제를 사용하여 레이어 효과 삭제 허용
* 플러그인 제거 Substance Source(&quot;보내기&quot; 기능과 함께 시작 프로그램 사용)
* &lbrack;Windows&rbrack; 고급 GPU에 TDR 경고를 표시하지 않음

**고정:**

* 새 프로젝트 파일 대화 상자의 번역 문제
* &lbrack;Bakers&rbrack; &quot;사전 처리된 장면 파일 저장&quot; 설정이 더 이상 작동하지 않음
* &lbrack;평면 투영&rbrack; 투영이 반복 UV가 있는 메시에서 작동하지 않음
* &lbrack;Decal&rbrack; 다른 칠 레이어 투영 모드를 사용하는 경우 일반 채널에서 동작 차이
* &lbrack;Smudge&rbrack;&lbrack;복제&rbrack; 가공물(Artifact)이 마스크에 페인팅할 때 나타날 수 있음
* 특정 레이어 콘텐츠가 있는 &lbrack;Engine&rbrack; 충돌
* 경우에 따라 페인팅할 때 &lbrack;Engine&rbrack; Random 충돌
* &lbrack;고정점&rbrack; 빈 마스크에 대한 참조는 항상 흰색을 반환합니다.
* &lbrack;Export&rbrack; 특정 스택 구성에서 고려하지 않은 레이어
* &lbrack;Export mesh&rbrack; 특수 문자가 포함된 경로와 함께 내보낼 수 없습니다.
* &lbrack;Export Mesh&rbrack; Linux 또는 MacOS에서 내보낼 때 glTF 파일을 읽을 수 없음
* &lbrack;메시 가져오기&rbrack; DAE, PLY 또는 glTF 다시 가져오기가 의도한 대로 작동하지 않음

**알려진 문제:**

* &lbrack;Scripting&rbrack;&lbrack;JavaScript&rbrack; 새 Curvature baker 설정을 편집할 수 없습니다.
* &lbrack;Bakers&rbrack; GPU 광선 추적 포함 Linux 충돌
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; 비활성화된 텍스처 세트를 내보내서는 안 됩니다.
* &lbrack;충돌&rbrack; 재질 레이어링 시 마스크를 페인트한 후 셰이더를 변경합니다

## 버전 5

### 5.3.3 (2019.3.3)

*(릴리스: 2020년 2월 6일*)요약: **Iray 2019.3**&#x200B;으로 업그레이드한 버그 수정

**추가됨:**

* Iray 2019.3으로 업그레이드
* &lbrack;Log&rbrack; 굽는 동안 충돌으로 이어지는 Ryzen CPU에 대한 오래된 bios를 나타냅니다.
* &lbrack;ABR&rbrack; 셸프에 ABR 알파 추출

**고정:**

* &lbrack;Baker&rbrack; 하이 폴리 메쉬에 UV가 없으면 굽기 실패
* &lbrack;Linux&rbrack; 사용자 정의 마우스 단축키가 저장되지 않음
* 일부 알파 모양과 함께 &lbrack;Brush&rbrack; 윤곽선이 사라짐
* &lbrack;Tablet&rbrack; 슬라이더를 이동할 때 잘못된 감지
* &lbrack;단축키&rbrack;에서는 &quot;Ctrl+Alt+MouseClick&quot;을 사용하여 단축키를 설정할 수 없습니다.
* &lbrack;Shelf&rbrack; 펜 타블렛을 사용할 때 리소스 도구 설명이 표시되지 않음
* &lbrack;2D 보기&rbrack;&lbrack;내보내기&rbrack; 2D 보기 사전 설정은 일반 정보를 고려하지 않습니다
* 특정 브러시를 사용하여 UV 정렬로 페인팅할 때 고정
* 필터 아래에 페인팅하면 진행 중인 획에 가공물이 만들어집니다
* &lbrack;Viewport&rbrack; 메시를 다시 가져온 후 뷰포트에 텍스처 캐시가 잘못됨
* &lbrack;충돌&rbrack; Photoshop으로 내보낸 후 저장하는 동안 오류가 발생했습니다.
* &lbrack;충돌&rbrack; 리소스를 가져올 때 접두어에 특수 기호 작성
* &lbrack;충돌&rbrack; 기준점 속성에서 참조를 클릭합니다.
* 앵커 포인트와 참조 사이에 필터가 있는 경우 &lbrack;앵커 포인트 &rbrack; 채널이 업데이트되지 않음
* 도움말 메뉴의 URL 링크가 작동하지 않습니다.

**알려진 문제:**

* &lbrack;UV Unwrapping&rbrack; 높은 폴리 메쉬 처리에 시간이 오래 걸릴 수 있습니다.
* 같은 좌표의 &lbrack;UV Unwrapping&rbrack; 정점이 병합됩니다.
* 드물게 일부 메시 부분에서 UV 생성이 실패할 수 있는 &lbrack;UV 언래핑&rbrack;
* &lbrack;UV Unwrapping&rbrack; 경우에 따라 단일 UV 섬에서 균일하지 않거나 매우 왜곡된 텍셀 비율
* &lbrack;UV Unwrapping&rbrack; 텍스처 세트 간의 균일하지 않은 텍스처 비율
* 생성된 &lbrack;UV Unwrapping&rbrack; UV 섬은 매우 길어질 수 있으며 경우에 따라 UV 공간에 맞지 않을 수 있습니다
* &lbrack;UV Unwrapping&rbrack; 가장자리가 작거나 겹친 역생성 면이나 비삼각형 메시 면은 UV Unwrapped가 되지 않을 수 있습니다

### 5.3.2 (2019.3.2)

*(릴리스: 2020년 1월 21일*)요약: **버그 수정**

**고정:**

* 단독 채널 모드로 저장된 프로젝트를 열면 메쉬가 표시되지 않습니다
* 복제 도구를 사용하여 레이어 아래에 페인팅할 때 뷰포트가 업데이트되지 않는 경우가 있음

**알려진 문제:**

* &lbrack;Ryzen CPU의 다중 스레딩과 관련된 Bakers&rbrack; 충돌
* &lbrack;UV Unwrapping&rbrack; 높은 폴리 메쉬 처리에 시간이 오래 걸릴 수 있습니다.
* 같은 좌표의 &lbrack;UV Unwrapping&rbrack; 정점이 병합됩니다.
* 드물게 일부 메시 부분에서 UV 생성이 실패할 수 있는 &lbrack;UV 언래핑&rbrack;
* &lbrack;UV Unwrapping&rbrack; 경우에 따라 단일 UV 섬에서 균일하지 않거나 매우 왜곡된 텍셀 비율
* &lbrack;UV Unwrapping&rbrack; 텍스처 세트 간의 균일하지 않은 텍스처 비율
* 생성된 &lbrack;UV Unwrapping&rbrack; UV 섬은 매우 길어질 수 있으며 경우에 따라 UV 공간에 맞지 않을 수 있습니다
* &lbrack;UV Unwrapping&rbrack; 가장자리가 작거나 겹친 역생성 면이나 비삼각형 메시 면은 UV Unwrapped가 되지 않을 수 있습니다

### 5.3.1 (2019.3.1)

*(릴리스: 2019년 12월 20일*)요약: **핫픽스**

**고정:**

* 특정 UV 투영이 있는 메시에서 작업할 때 충돌
* Photoshop 사전 설정 간 전환 시 &lbrack;ABR&rbrack; 충돌
* &lbrack;Linux&rbrack;libGLX 종속성 문제로 인해 CentOS 7.4에서 Substance Painter을 시작할 수 없습니다.
* 파일 > 지우기를 사용한 후 굽는 동안 &lbrack;Bakers&rbrack; 충돌
* &lbrack;Bakers&rbrack; 취소 후 베이킹 진행 대화 상자가 멈춤
* &lbrack;Bakers&rbrack; 텍스처 내보내기 후 베이킹 메시가 작동하지 않음
* &lbrack;Bakers&rbrack; &quot;이름별 일치&quot;를 사용하면 검은색 메시 맵이 결과로 표시됨
* &lbrack;Bakers&rbrack; Cage는 고려되지 않음
* &lbrack;Shelf&rbrack; PSD 파일을 가져오면 이미지가 손상됨
* &lbrack;Sample&rbrack; &quot;Mat&quot; 샘플 프로젝트에 끊어진 카메라와 잘못된 내보내기 사전 설정이 있음

**알려진 문제:**

* &lbrack;Ryzen CPU의 다중 스레딩과 관련된 Bakers&rbrack; 충돌
* &lbrack;UV Unwrapping&rbrack; 높은 폴리 메쉬 처리에 시간이 오래 걸릴 수 있습니다.
* 같은 좌표의 &lbrack;UV Unwrapping&rbrack; 정점이 병합됩니다.
* 드물게 일부 메시 부분에서 UV 생성이 실패할 수 있는 &lbrack;UV 언래핑&rbrack;
* &lbrack;UV Unwrapping&rbrack; 경우에 따라 단일 UV 섬에서 균일하지 않거나 매우 왜곡된 텍셀 비율
* &lbrack;UV Unwrapping&rbrack; 텍스처 세트 간의 균일하지 않은 텍스처 비율
* 생성된 &lbrack;UV Unwrapping&rbrack; UV 섬은 매우 길어질 수 있으며 경우에 따라 UV 공간에 맞지 않을 수 있습니다
* &lbrack;UV Unwrapping&rbrack; 가장자리가 작거나 겹친 역생성 면이나 비삼각형 메시 면은 UV Unwrapped가 되지 않을 수 있습니다

### 5.3.0 (2019.3.0)

*(출시됨: 2019년 12월 17일*)요약: **핸드페인팅 사용자 경험 개선, 태블릿 작업, 베타(0.3.0)의 자동 UV 언래핑 및 핸드페인팅을 위한 다양한 새로운 콘텐츠**&#x200B;가 포함된 주요 릴리스

**추가됨:**

* Substance Painter에 자동 UV 언래핑 0.3.0 버전 통합
* &lbrack;UV 언랩&rbrack; UV가 없거나 부분 UV가 없는 경우 Substance Painter에서 자동 UV 언랩
* &lbrack;UV unwrapping&rbrack; 이를 활성화 및 비활성화하는 하나의 전역 설정
* &lbrack;UV unwrapping&rbrack; 버전이 로그 파일에 보고됨
* &lbrack;UV 언래핑&rbrack;&lbrack;UI&rbrack; UV 언래핑 진행률을 나타냅니다.
* &lbrack;UI&rbrack; 브러시 미리보기를 선택할 수 있는 컨텍스트 도구 모음의 새 설정(전체 미리보기, 브러시 윤곽선 및 십자)
* &lbrack;도구&rbrack; 알파 섹션의 새로운 고급 혼합 모드: 일반 외에 밝게(최대)
* 알파 또는 마스크의 레이어당 &lbrack;레이어 스택&rbrack; 감마 교정 옵션(마우스 오른쪽 단추 클릭 메뉴)
* &lbrack;레이어 스택&rbrack;&lbrack;UI&rbrack; 레이어 알파가 감마 수정된 경우 &#39;i&#39; 아이콘 추가
* &lbrack;Tablet&rbrack;&lbrack;Tool&rbrack; 크기 및 플로우에 대한 최소 압력 노출
* &lbrack;Tablet&rbrack;&lbrack;UI&rbrack; 곡선 압력을 선택하기 위한 컨텍스트 도구 모음의 새로운 설정: 선형, 손쉬운 입력, 손쉬운 출력
* &lbrack;Tablet&rbrack;&lbrack;UX&rbrack; 추가 Ctrl+Alt+클릭하여 스크롤
* Photoshop 브러시 사전 설정 가져오기(ABR 형식)
* &lbrack;ABR&rbrack; 모양 매개 변수 지원
* &lbrack;ABR&rbrack; 모양 다이내믹 매개 변수 지원
* &lbrack;ABR&rbrack; 지원 전송 매개변수
* &lbrack;ABR&rbrack; 분산 매개변수 지원
* &lbrack;ABR&rbrack;&lbrack;역동적인 획&rbrack; 원형율 및 뒤집기 지원
* &lbrack;ABR&rbrack;&lbrack;Shelf&rbrack; 필터 편집기에서 브러시 폴더 구조 노출
* &lbrack;ABR&rbrack;&lbrack;Shelf&rbrack; 축소판에 Photoshop 아이콘 추가
* &lbrack;ABR&rbrack;&lbrack;Shelf&rbrack; ABR 상세 썸네일에 지원되지 않는 매개변수 목록 추가
* &lbrack;Tool&rbrack;&lbrack;Tools&rbrack; 생성할 임의 시드 수를 제어하는 새로운 동적 선 설정
* &lbrack;도구&rbrack;&lbrack;UI&rbrack; 분산 지터에 대한 새 분포 및 축 설정 추가
* &lbrack;단축키&rbrack; Ctrl+Shift+B를 추가하여 베이킹 창 열기
* &lbrack;UI&rbrack;&lbrack;Menu&rbrack; &#39;편집&#39; 메뉴에 항목을 추가하여 베이킹 창 열기
* &lbrack;UI&rbrack;&lbrack;Settings&rbrack; 단축키 목록의 개선 정렬
* &lbrack;UI&rbrack; 압력 컨트롤(크기 및 플로우) 아이콘을 켜기/끄기 단추로 바꾸기
* &lbrack;Viewport&rbrack; 2D 및 3D 뷰포트에 각각 포커스를 두도록 허용
* QT 5.12.5로 업데이트
* &lbrack;UI&rbrack; 메시 로드 진행률을 나타냅니다.
* &lbrack;Substance&rbrack; 슬라이더로 고정되지 않은 소프트 범위에 대한 지원 추가
* &lbrack;Substance&rbrack; Substance 매개 변수 정밀도를 최대 6소수까지 증가
* &lbrack;Substance&rbrack; 매개변수로 정의된 단계를 고려합니다.
* &lbrack;user&rbrack; Substance 데이터의 조건을 지원하여 동적 획 생성 최적화
* &lbrack;user&rbrack; Substance 데이터를 통해 그래프 출력을 모든 채널에 대한 마스크로 지정할 수 있습니다.
* &lbrack;Content&rbrack; 변위 친화적인 토폴로지, 새 ID 맵 및 새 카메라를 사용하여 &#39;Mat&#39; 샘플 프로젝트 업데이트
* &lbrack;Content&rbrack; 3가지 새로운 필터 통합(MatFx): 만화책, 수채화, 오일 페인트(Emrecan Cubukcu 작업에서 영감)
* &lbrack;Content&rbrack; Kyle T. Webster 팩의 102개 Photoshop 브러시 사전 설정 통합
* &lbrack;Content&rbrack; 18개의 새로운 브러시 사전 설정 통합: 페인트 롤러 화살표, 페인트 롤러 경고 텍스트, 목탄 미세 등
* &lbrack;Content&rbrack; 9개의 새로운 알파 통합: 브러시 메이커 페인트 롤러, 브러시 메이커 Photoshop, 브러시 패턴 등
* &lbrack;Content&rbrack; 2개의 새로운 도구 사전 설정 통합: Gouache Dense 및 Gouache Faded
* &lbrack;Content&rbrack; 1개의 새로운 생성기 통합 : UV 검사기(밝은 영역 UV 섬 및 이음새)
* &lbrack;Content&rbrack; 2개의 새로운 내보내기 사전 설정 통합: Keyshot 9+ 및 Spark AR Studio
* &lbrack;Content&rbrack; 1개의 새 프로젝트 템플릿 통합 : Spark AR Studio(Facebook)

**고정:**

* &lbrack;Tablet&rbrack; 스타일러스 선 실행 취소(Ctrl+Z)가 마우스 선 실행 취소보다 더 지연됨
* 직선을 그릴 때 시작 및 끝 압력이 고려되지 않은 &lbrack;Tablet&rbrack;
* 직선을 사용할 때 첫 번째 스탬프가 두 번 그려지는 &lbrack;Tablet&rbrack;
* &lbrack;Tablet&rbrack; Huion 태블릿 바로 가기 지원 개선
* &lbrack;Tablet&rbrack; Huion 펜 버튼에 대한 지원 개선
* 브러시 미리 보기와 그려진 스탬프 사이의 &lbrack;Tablet&rbrack; 오프셋
* &lbrack;Tablet&rbrack; 펜으로 브러시를 수정하는 단축키로 인해 가끔 성능이 저하됩니다
* 특정 레이어에 페인트할 때 &lbrack;Tablet&rbrack; Lag
* 드문 경우지만 뷰포트를 전환할 때 흐린 텍스처가 발생할 수 있습니다.
* &lbrack;UI&rbrack;&lbrack;Substance&rbrack; 이미지 입력이 항상 표시되는 것은 아닙니다
* 정리하면 프로젝트에서 가져온 셸프에서 사전 설정이 제거되지 않음
* &lbrack;Tool&rbrack;&lbrack;Dynamic Stroke&rbrack; 스탬프 사이클 수 수정 시 성능 문제
* 드문 경우지만 3D/2D 뷰포트 모드에서 페인팅하는 동안 새로 고침 문제
* 매우 긴 획 하나를 페인트하면 얼음이 발생할 수 있습니다
* &lbrack;Tool&rbrack; 특정 도구를 사용하여 페인팅할 때 성능 문제
* &lbrack;UI&rbrack; 컨텍스트 도구 모음은 폴더를 선택할 때 브러시 속성을 표시합니다.
* 대칭 축 값이 재설정되지 않음
* 부동 소수점 값이 있는 EXR 텍스처 가져오기가 완전히 검정색입니다
* Alt 키를 누른 채 격리할 채널을 클릭하는 기능은 필터 및 생성기에서 작동하지 않습니다
* &lbrack;내보내기&rbrack; 내보내기 시 특정 프로젝트 충돌
* &lbrack;Substance&rbrack; 매개 변수가 Visible If에 의해 숨겨진 경우 드롭다운의 기본값이 잘못되었습니다.
* 재질 레이어를 통해 정의된 &lbrack;Shader&rbrack; 채널은 UI에서 동일한 방식으로 정렬되지 않습니다
* &lbrack;Shelf&rbrack; 사전 설정 메타데이터가 디스크에 저장되지 않음

**알려진 문제:**

* &lbrack;UV Unwrapping&rbrack; 높은 폴리 메쉬 처리에 시간이 오래 걸릴 수 있습니다.
* 같은 좌표의 &lbrack;UV Unwrapping&rbrack; 정점이 병합됩니다.
* 드물게 일부 메시 부분에서 UV 생성이 실패할 수 있는 &lbrack;UV 언래핑&rbrack;
* &lbrack;UV Unwrapping&rbrack; 경우에 따라 단일 UV 섬에서 균일하지 않거나 매우 왜곡된 텍셀 비율
* &lbrack;UV Unwrapping&rbrack; 텍스처 세트 간의 균일하지 않은 텍스처 비율
* 생성된 &lbrack;UV Unwrapping&rbrack; UV 섬은 매우 길어질 수 있으며 경우에 따라 UV 공간에 맞지 않을 수 있습니다
* &lbrack;UV Unwrapping&rbrack; 가장자리가 작거나 겹친 역생성 면이나 비삼각형 메시 면은 UV Unwrapped가 되지 않을 수 있습니다
* Meetmat 샘플에서 가져온 카메라에 몇 가지 문제가 있습니다

### 5.2.3 (2019.2.3)

*(릴리스: 2019년 10월 23일*)요약: **버그 수정 릴리스**

**추가됨:**

* &lbrack;텍스처 세트 목록&rbrack; 초점 모드를 빠르게 활성화/비활성화하는 [추가] 단추
* &lbrack;Log&rbrack; 로그 파일에 Windows 10 버전 번호 추가
* 최신 버전의 Substance 엔진으로 업데이트
* &lbrack;MacOS&rbrack; 새 MacOS Catalina 배포 요구 사항을 따르도록 소프트웨어를 공증함

**고정:**

* &lbrack;Plugin&rbrack; Plugin Source가 작동하지 않음
* &lbrack;MacOS&rbrack;&lbrack;Shader&rbrack; Mac OS 10.14.5 및 AMD: 재질 레이링이 의도한 대로 작동하지 않습니다.

**알려진 문제:**

* 하위 구분이 있는 알렘빅 파일은 가져올 수 없습니다.
* 일부 Alembic 파일을 가져올 때 드문 충돌 발생
* Pascal GPU에서 DXR을 사용하여 굽기 시 UI가 일시적으로 응답하지 않습니다

### 5.2.2 (2019.2.2)

*(릴리스: 2019년 9월 20일*)요약: **버그 수정 릴리스**

**고정:**

* 스크립팅으로 리소스를 가져오면 충돌 발생
* &lbrack;Plugin&rbrack; 소스에서 재질을 다운로드하면 충돌이 발생할 수 있습니다.

**알려진 문제:**

* 하위 구분이 있는 알렘빅 파일은 가져올 수 없습니다.
* 일부 Alembic 파일을 가져올 때 드문 충돌 발생
* Pascal GPU에서 DXR을 사용하여 굽기 시 UI가 일시적으로 응답하지 않습니다

### 5.2.1 (2019.2.1)

*(릴리스: 2019년 9월 17일*)요약: **버그 수정 릴리스**

**고정:**

* &lbrack;Mac&rbrack;&lbrack;USD&rbrack; MacOS에서 내보낸 USDZ 파일을 열 수 없습니다
* &lbrack; 텍스처 세트&rbrack; ALT 수정자를 사용하여 텍스처 세트를 분리할 수 없음
* &lbrack;Shelf&rbrack; 사전 설정, 스마트 재질 및 스마트 마스크는 애플리케이션을 종료할 때 항상 수정됩니다.
* &lbrack;레이어 스택&rbrack; 다른 효과를 삭제한 후 효과를 선택할 수 없습니다.
* 도구 속성 패널 내에서 슬라이더를 사용할 때 깜박임
* 사전 설정을 선반으로 내보낼 때 충돌
* 공간이 부족한 사전 설정을 내보낼 때 충돌 발생
* 공간이 부족한 사전 설정을 만들 때 충돌 발생

**알려진 문제:**

* 하위 구분이 있는 알렘빅 파일은 가져올 수 없습니다.
* 일부 Alembic 파일을 가져올 때 드문 충돌 발생
* Pascal GPU에서 DXR을 사용하여 굽기 시 UI가 일시적으로 응답하지 않습니다

### 5.2.0 (2019.2.0)

*(릴리스: 2019년 7월 25일*)요약: **성능 및 새로운 사전 시각화 모드의 베이커 업데이트가 포함된 주요 릴리스 + 새 콘텐츠**

**추가됨:**

* &lbrack;Bakers&rbrack; DXR 및 OptiX 포함 GPU 광선 추적(앰비언트 오클루전, Thickness)에 대한 추가 지원
* &lbrack;Bakers&rbrack; CPU 광선 추적에 대한 최적화 및 가속
* &lbrack;Bakers&rbrack;&lbrack;Vis mode&rbrack;&lbrack;UI&rbrack; 뷰포트의 새로운 베이킹 시각화 모드
* &lbrack;Bakers&rbrack;&lbrack;Preferences&rbrack;&lbrack;UI&rbrack; GPU 광선 추적 활성화-비활성화에 대한 새로운 베이킹 옵션
* &lbrack;Bakers&rbrack;&lbrack;UI&rbrack; 진행률 표시줄 대화 상자 재작업
* &lbrack;Bakers&rbrack; 경고 및 오류 메시지 개선
* &lbrack;Bakers&rbrack; 더 반응형 제빵 프로세스 취소 허용
* &lbrack;Bakers&rbrack; 취소를 클릭한 후 베이크 창 다시 열기
* &lbrack;Proj&rbrack;&lbrack;UX&rbrack; 회전 조작기 사용성 개선
* &lbrack;Settings&rbrack; HDPI 화면에 대한 뷰포트 해상도를 줄여 성능을 개선하는 옵션
* &lbrack;스크립팅&rbrack; 텍스처 세트 해상도 변경
* &lbrack;스크립팅&rbrack; 선택한 텍스처 세트 가져오기
* &lbrack;스크립팅&rbrack; 사용자가 텍스처 세트를 선택할 수 있도록 허용
* &lbrack;Scripting&rbrack; 텍스처 세트 선택이 변경된 시기를 아는 함수
* &lbrack;Shelf&rbrack; 40개의 새 스마트 재질 추가됨
* &lbrack;Shelf&rbrack; 20개의 새 스마트 마스크 추가됨

**고정:**

* &lbrack;레이어 스택&rbrack; 다중 선택 시 UI 고정
* &lbrack;레이어 스택&rbrack; 많은 레이어를 그룹화하면 UI가 평소보다 오래 고정됨
* &lbrack;레이어 스택&rbrack; 경우에 따라 레이어와 효과를 동시에 선택할 수 있습니다
* 페인팅 도구 내에 사용된 Substance 그래프가 적절한 해상도로 생성되지 않습니다
* &lbrack;Baker&rbrack; &quot;모든 텍스처 세트 굽기&quot; 버튼은 베이커를 선택하지 않으면 비활성화되지 않습니다.
* &lbrack;MacOS&rbrack; 쪽맞춤에 대한 경고 메시지 비활성화
* 마스크와 함께 사용할 때 투영 도구에 미리보기가 없음
* 디스크 공간이 부족하여 저장하려고 할 때 충돌 및 프로젝트 손상
* 공간이 부족한 셸프를 통해 디스크의 리소스를 가져올 때 &lbrack;Shelf&rbrack; 충돌
* 세션 사전 설정을 복원할 때 &lbrack;Shelf&rbrack; 충돌
* &lbrack;Shelf&rbrack; 공백으로 끝나는 이름을 가진 사전 설정을 가져오면 충돌이 발생합니다
* &lbrack;Shelf&rbrack; 접두어가 빈 공간으로 끝나는 리소스를 가져오면 충돌이 발생합니다

**알려진 문제:**

* 하위 구분이 있는 알렘빅 파일은 가져올 수 없습니다.
* 일부 Alembic 파일을 가져올 때 드문 충돌 발생
* Pascal GPU에서 DXR을 사용하여 굽기 시 UI가 일시적으로 응답하지 않습니다

### 5.1.3 (2019.1.3)

*(출시됨: 2019년 7월 1일*)요약: **두 가지 새로운 기능이 포함된 버그 수정**

**추가됨:**

* 명령줄에서 VRam 예산을 지정할 수 있습니다(예: —vram-budget 4096).
* &lbrack;QML&rbrack; QML 단추 및 확인란의 흐름 모드 및 지우기 속성 노출

**고정:**

* &quot;패스 따르기&quot;가 항상 작동하지 않음
* 단일 채널 슬롯에 사용된 SBSAR에서 채널 매핑이 작동하지 않음
* &lbrack;레이어 스택&rbrack; 숨겨진 레이어로 스크롤할 때 낮은 성능
* 마스크 사이를 클릭할 때 &lbrack;TextureSet&rbrack; 충돌
* &lbrack;SVT&rbrack; 변위가 제대로 표시되지 않고 일부 경우 깜박임
* 꼭지점 수직 대신 점 수직을 사용하는 메쉬가 있는 &lbrack;Alembic&rbrack; 충돌
* &lbrack;Alembic&rbrack;&lbrack;Log&rbrack; 가져오기 중 Alembic 파일이 지원되지 않는 경우 로그에 오류를 보고합니다

**알려진 문제:**

* 하위 구분이 있는 알렘빅 파일은 가져올 수 없습니다.
* 일부 Alembic 파일을 가져올 때 드문 충돌 발생

### 5.1.2 (2019.1.2)

*(릴리스: 2019년 5월 21일*)요약: **핫픽스**

**고정:**

* 이미지 입력이 있는 두 개의 리소스를 선택할 때 충돌

### 5.1.1 (2019.1.1)

*(릴리스: 2019년 5월 20일*)요약: **핫픽스**

**추가됨:**

* Substance Designer 2019.1의 마지막 릴리스를 사용하여 최신 버전의 Substance 엔진으로 업데이트

**고정:**

* &lbrack;Substance&rbrack; 보이는 경우 입력 이미지에 대해 고려하지 않음
* &lbrack;SVT&rbrack;&lbrack;Engine&rbrack; 텍스처 세트 해상도를 변경하면 경우에 따라 충돌이 발생합니다
* 경우에 따라 &lbrack;Engine&rbrack; Random Black 텍스처가 나타납니다
* &lbrack;레이어 스택&rbrack;&lbrack;UI&rbrack; SHIFT로 마스크를 전환하면 여러 레이어를 동시에 선택할 수 있습니다
* &lbrack;레이어 스택&rbrack; 불투명도는 통과 혼합 모드의 페인트 효과에 영향을 주지 않습니다.
* &lbrack;레이어 스택&rbrack; Height-일반 필터 입력이 지우개 브러시 획으로 제대로 업데이트되지 않음
* 스마트 마스크 드롭을 실행 취소할 때 &lbrack;LayersStack&rbrack; 충돌
* 어두운 영역과 시간 앤티 앨리어싱이 활성화된 와이어프레임 깜박임
* &lbrack;변위&rbrack; 일부 강한 메시가 있는 AMD에서 지연됨
* 파일 탐색기를 통해 일부 프로젝트를 열 때 &lbrack;Windows&rbrack; 충돌
* 경우에 따라 고정점이 있는 마스크를 제거할 때 &lbrack;Histogram&rbrack; 충돌
* 드문 경우지만 미리 보기 생성 시 충돌 발생
* &lbrack;충돌&rbrack; 너무 많은 복제 및 손가락 도구를 사용하여 프로젝트를 다시 열 수 없음
* 경우에 따라 저장한 후 재질 모드에서 메쉬가 표시되지 않습니다
* &lbrack;Scripting&rbrack; alg.mapexport.documentStructure()가 폴더에 대해 잘못된 값을 반환합니다.

**알려진 문제:**

* 텍스처 세트 이름을 두 번 클릭하면 이름 바꾸기 모드로 들어가기 전에 해당 이름이 선택됩니다.

### 5.1.0 (2019.1.0)

*(출시됨: 2019년 4월 23일*)요약: **새로운 전용 콘텐츠, 실시간 및 Iray의 변위 및 테셀레이션, 마스크 비교 효과, 방사형 대칭, 평면 및 구형 투영이 포함된 동적 획**

**추가됨:**

* &lbrack;Tool&rbrack; 동적 획: 브러시 획과 함께 Substance 변형
* &lbrack;동적 선&rbrack; 옵션과 함께 새 스탬프 인덱스 매개 변수를 표시합니다.
* &lbrack;동적 획&rbrack; 고려사항 $time 매개 변수
* &lbrack;동적 선&rbrack; 선 및 스탬프당 새 $randomseed 매개 변수 생성
* &lbrack;동적 선&rbrack; 난수에서 동적 선 색인 시작
* &lbrack;Dynamic stroke&rbrack;&lbrack;Shelf&rbrack; 전용 새 아이콘이 있는 동적 획 리소스 찾기 도움말
* 실시간 뷰포트에서 변위 및 쪽맞춤
* Iray의 변위 및 테셀레이션
* &lbrack;Shader settings&rbrack;&lbrack;UI&rbrack; 변위 및 테셀레이션 제어를 위한 새 탭
* &lbrack;레이어 스택&rbrack; 새로운 비교 마스크 효과: 두 채널을 비교하여 마스크 생성
* &lbrack;레이어 스택&rbrack;&lbrack;UI&rbrack; 마우스 오른쪽 버튼 클릭 메뉴 &quot;Height 조합으로 마스크 추가&quot;에 CompareMask 효과를 삽입하는 새 항목
* &lbrack;대칭&rbrack; 새로운 대칭 모드: 방사형 페인팅
* &lbrack;대칭 설정&rbrack; &quot;설정&quot; 및 &quot;표시&quot; 섹션을 모두 확장합니다.
* &lbrack;대칭 설정&rbrack;&lbrack;UI&rbrack; 방사형 페인팅을 위한 미리 보기
* 두 가지 새로운 투영 모드, 즉 평면 및 구형 노출
* &lbrack;Proj&rbrack; 모든 투영에 대한 새로운 모양 자르기 모드
* &lbrack;Proj&rbrack; 평면 모드 및 새로운 조작기: 표면 도구
* &lbrack;Proj&rbrack;&lbrack;단축키&rbrack; 단축키 SHIFT+W for Surface tool
* &lbrack;Proj&rbrack; 깊이 컬링 및 백페이스 컬링이 포함된 평면 투영 마스킹
* &lbrack;조작기&rbrack; 삼면체의 세 축 모두에 대한 회전 조작기 개선
* &lbrack;Tool&rbrack;&lbrack;UX&rbrack; Alt 키를 누른 채 채널을 클릭하면 채널에 초점이 맞춰집니다(활성화하거나 다른 채널을 비활성화함).
* &lbrack;엔진&rbrack; 최신 버전의 Substance 엔진으로 업데이트
* &lbrack;텍스처 설정&rbrack; 다중 선택 및 해상도 변경
* &lbrack;텍스처 세트&rbrack; 텍스처 세트의 빠른 활성화 및 비활성화
* &lbrack;텍스처 세트&rbrack; 솔로 및 모든 옵션을 새 메뉴에 결합
* &lbrack;텍스처 set&rbrack;&lbrack;활성화 및 비활성화에 대한 레이어 스택&rbrack; 새 아이콘
* &lbrack;레이어 스택&rbrack;&lbrack;UX&rbrack; 이미 선택한 효과 위에 효과 삽입
* &lbrack;레이어 스택&rbrack;&lbrack;UI&rbrack; 레이어 스택 보기 선택 스타일 다시 작업
* 인스턴스 레이어의 [통과] 모드가 기본적으로 &lbrack;레이어 스택&rbrack; 혼합 모드입니다.
* &lbrack;내보내기&rbrack; 디더링 활성화 및 비활성화 옵션
* &lbrack;Plugin&rbrack; 슬라이더용 정밀도 수정자 지원(SHIFT)
* &lbrack;Plugin&rbrack;&lbrack;UI&rbrack; 자동 저장의 새 아이콘
* &lbrack;스크립팅&rbrack; 폴더의 내용을 나열합니다.
* &lbrack;스크립팅&rbrack; 파일 삭제 허용
* &lbrack;Scripting&rbrack; 사용된 리소스를 포함한 모든 스택 정보 읽기
* &lbrack;Content&rbrack;&lbrack;Dynamic stroke&rbrack; 새로운 도구 및 브러시 사전 설정
* &lbrack;Content&rbrack;&lbrack;Dynamic stroke&rbrack; 두 개의 새로운 프로시저 그레이디언트: 그레이디언트 색조 및 그레이디언트 빌더
* &lbrack;Content&rbrack; 11가지 새로운 필터: MatFx 필링 페인트, MatFx 물방울 등
* &lbrack;Content&rbrack; 7개의 새로운 생성기: 자동 스티처, UV 랜덤 색상, UV 텍셀 밀도 등
* &lbrack;Content&rbrack; 93개의 새로운 알파: 새로운 텍스트, 화살표 및 다양한 모양
* &lbrack;Content&rbrack; 2개의 새로운 절차: 그레이디언트 색조, 그레이디언트 빌더 등
* &lbrack;내용&rbrack; 역동적인 획에 대한 21개의 새로운 도구 및 브러시 사전 설정 : 자갈, 발자국, 스프레이 등
* &lbrack;Content&rbrack; 2개의 새로운 HDRis: Canopus Ground 및 Autumn Forest
* &lbrack;Content&rbrack; 쉘프의 무작위 시드 큐레이션으로 콘텐츠 업데이트
* &lbrack;Content&rbrack; 셸프에 노출된 무작위 시드 매개 변수가 있는 새 아이콘

**고정:**

* &lbrack;레이어 스택&rbrack; 레이어 스택이 계속 드래그됨
* &lbrack;Mac&rbrack; &quot;Show in Finder&quot;로 인해 작동이 중단될 수 있음
* 셰이더 파일이 이동하면 사용자 지정 UI를 통해 저장된 &lbrack;Scripting&rbrack; 설정이 손실됩니다.
* &lbrack;스크립팅&rbrack; API 버전 번호가 잘못되었으며 최신 버전이 아닙니다.
* &lbrack;효과&rbrack; 막대 그래프 콘텐츠가 올바르게 표시되지 않음
* &lbrack;효과&rbrack; 막대 그래프 효과가 업데이트되지 않는 경우가 있습니다.
* &lbrack;Shelf&rbrack; Stitches가 &quot;플라스틱 직물 피라미드&quot; 재료에 제대로 정렬되지 않음

**알려진 문제:**

* 텍스처 세트 이름을 두 번 클릭하면 이름 바꾸기 모드로 들어가기 전에 해당 이름이 선택됩니다.
* &lbrack;레이어 스택&rbrack;&lbrack;UI&rbrack; SHIFT로 마스크를 전환하면 여러 레이어를 동시에 선택할 수 있습니다

## 버전 4

### 4.3.3 (2018.3.3)

*(출시됨: 2019년 3월 7일*)요약: **버그 수정**

**추가됨:**

* &lbrack;Content&rbrack; 새 프로젝트 템플릿 통합: &quot;PBR - 금속 거칠기 Alpha-blend&quot;
* Linux 동적 라이브러리 검색 순서가 시스템에 설치된 라이브러리보다 설치 디렉토리의 라이브러리에 우선 순위를 지정하도록 변경되었습니다.

**고정:**

* 3D 뷰포트에서 가끔씩 메시가 사라집니다(카메라를 재설정하려면 F 키 누름).
* 새 Sketchfab 라이선스 유형으로 Substance Painter Sketchfab 업로더 업데이트
* &lbrack;Import&rbrack;&lbrack;glTF&rbrack; glTF 파일에 정의된 입력 텍스처 변조를 잘못 처리함
* &lbrack;Import&rbrack;&lbrack;glTF&rbrack; 지표 평면이 glTF 가져오기와 함께 잘못 표시되는 경우가 있습니다
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; Opacity가 Arkit에서 작동하지 않습니다
* 경우에 따라 &lbrack;Export&rbrack;&lbrack;USD&rbrack; USDz 내보내기 충돌
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; 충돌에 대한 리드를 저장하지 않고 USD으로 내보내기
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; 텍스처에 대한 잘못된 타일링 모드, 메시에 대한 하위 분할 모드 및 셰이더에 대한 출력 유형
* &lbrack;Export&rbrack;&lbrack;USD&rbrack; 모든 형상이 있는 일부 텍스처 세트만 스파스 내보내기로 내보내기
* 끊어진 인스턴스 레이어를 삭제하려고 할 때 &lbrack;Instance&rbrack; 충돌
* &lbrack;Regression&rbrack;&lbrack;Export&rbrack; 일부 맵이 선택한 비트 심도에서 내보내지지 않음
* &lbrack;Linux&rbrack; 라이브러리 libtbb.so.2 문제

**알려진 문제:**

* 경우에 따라 AMD VEGA GPU에서 계산 중단
* Windows OS의 단축키와 관련된 Huion 태블릿 문제

### 4.3.2 (2018.3.2)

*(릴리스: 2019년 1월 24일*)요약: **새로운 기능이 포함된 핫픽스(뷰포트에서 USDZ 내보내기 및 텍스처 필터링)**

**추가됨:**

* &lbrack;내보내기&rbrack; USDZ로 내보내기 허용
* &lbrack;뷰포트(&amp;r); 디스플레이 설정에서 텍스처 품질을 제어할 수 있도록 허용
* &lbrack;Viewport&rbrack; 표시 설정에 mip 편향 설정 추가됨
* &lbrack;Viewport&rbrack; 디스플레이 설정에 비등방성 필터링 추가
* &lbrack;plugins&rbrack; Substance Painter 2018 스타일을 사용하도록 공식 플러그인 업데이트
* &lbrack;License&rbrack; 기본적으로 사용자 폴더에 라이선스 설치

**고정:**

* 압축 해제에 연결된 충돌
* 솔로 재질에 TAA 추가
* 그림자가 있는 노이즈, 디더링이 있는 TAA 및 알파 테스트 셰이더
* 모든 클래식 PBR 셰이더에 대한 Specular 디더링 제거
* 경우에 따라 셰이더 설정의 충돌
* OpenGL과 Iray 렌더링 간에 분산 활성화가 동기화되지 않음
* 손가락 및 복제 도구가 특정 메시에서 더 이상 작동하지 않습니다
* 일부 텍스처 세트가 Ray 렌더링에 나타나지 않습니다.
* 프로젝트를 닫은 후 이름이 바뀐 텍스처 세트가 저장되지 않음
* ID 맵에서 재질을 드래그 앤 드롭할 때 가공물 와이어프레임
* 프로젝트를 저장할 때 &lbrack;Scripting&rbrack; 파일 경로 생성이 강제되지 않음
* &lbrack;Scripting&rbrack; 콜백 &quot;onProjectAboutToSave()&quot; 기능이 더 이상 작동하지 않음
* 버그 보고 창에서 포럼 링크가 끊어짐

**알려진 문제:**

* 경우에 따라 AMD VEGA GPU에서 계산 중단
* Windows OS의 단축키와 관련된 Huion 태블릿 문제

### 4.3.1 (2018.3.1)

*(릴리스: 2018년 12월 6일*)요약: **핫픽스**

**추가됨:**

* &lbrack;대칭&rbrack;&lbrack;뷰포트&rbrack; 2D 보기에서 페인팅한 대칭이 다시 돌아왔으며 이제 복제 브러시 미리 보기가 수정되었습니다.

**고정:**

* &lbrack;Export&rbrack; 2D 보기 내보내기에서 경우에 따라 검은색 텍스처가 출력됩니다
* 재질 레이어를 인스턴스화한 후 Iray에서 &lbrack;Iray&rbrack; 일반 정보가 올바르지 않게 됩니다.
* 정사각형이 아닌 텍스처 세트를 사용하면 경우에 따라 충돌이 발생할 수 있습니다
* &lbrack;Undo&rbrack; 몇몇 Ctrl+Z는 경우에 따라 무작위로 충돌으로 이어질 수 있습니다.
* &lbrack;QML&rbrack; AlgScrollView는 경우에 따라 로그에 경고를 생성할 수 있습니다(바인딩 루프)

**알려진 문제:**

* 경우에 따라 AMD VEGA GPU에서 계산 중단
* Windows OS의 단축키와 관련된 Huion 태블릿 문제
* 앤티 앨리어싱과 그림자를 함께 활성화하면 예기치 않은 결과가 발생할 수 있습니다

### 4.3.0 (2018.3.0)

*(출시됨: 2018년 11월 20일*)요약: **뷰포트 업그레이드, 적절한 2D 보기 내보내기, 새로운 UI 도우미, 향상된 대칭 도구, 새로운 콘텐츠 및 큰 성능 향상**

**추가됨:**

* &lbrack;앤티 앨리어싱&rbrack;&lbrack;뷰포트&rbrack; 3D 뷰포트에 대한 새로운 임시 안티앨리어싱 필터링(디스플레이 설정을 통해)
* &lbrack;내보내기&rbrack; 2D 뷰포트의 내용을 단일 텍스처로 내보냅니다
* &lbrack;Export&rbrack;&lbrack;Dithering&rbrack; 내보내기 시 디더링 표시
* 레이어 및 폴더의 &lbrack;레이어 스택&rbrack; 색상
* &lbrack;레이어 스택&rbrack; 다중 레이어 및 효과의 빠른 활성화 및 비활성화
* &lbrack;레이어 스택&rbrack; 위/아래 키 및 마우스 스크롤로 혼합 모드를 쉽게 탐색
* &lbrack;Proj&rbrack;&lbrack;UI&rbrack; 삼평면의 세 축 모두에 추가 회전 조작기
* &lbrack;Proj&rbrack;&lbrack;Shorcuts&rbrack; - 및 + - UV 투영 조작기 크기 변경
* &lbrack;Shader&rbrack; PBR-coated 셰이더의 채널이 있는 코팅된 레이어 매개 변수를 제어합니다
* &lbrack;Substance&rbrack; 필터 및 생성기에 대한 새로운 메시 기반 텍스처 입력 노출
* &lbrack;대칭&rbrack;&lbrack;뷰포트&rbrack;&lbrack;UI&rbrack; 조작기가 있는 컨트롤 대칭 오프셋
* &lbrack;대칭&rbrack;&lbrack;상황별 도구 모음&rbrack;&lbrack;UI&rbrack; 옵션이 있는 새 대칭 패널
* &lbrack;대칭&rbrack; 새 대칭 라인 교차 모드
* &lbrack;대칭&rbrack; 새 대칭 복제 커서
* &lbrack;대칭&rbrack;&lbrack;단축키&rbrack; Q: 숨기기 및 -, +: 크기 변경 및 shift: 스냅
* &lbrack;Log&rbrack; 텍스처를 내보낼 수 없을 때 오류 메시지 개선
* &lbrack;스크립팅&rbrack; 표시 설정에서 리소스 변경 또는 업데이트 허용
* &lbrack;스크립팅&rbrack; 텍스처 세트에서 채널 만들기 또는 제거 허용
* &lbrack;Content&rbrack;&lbrack;Shaders&rbrack; 전용 셰이더(pbr-metal-rough-비등방성-angle)가 있는 비등방성에 대한 지원 추가
* &lbrack;내용&rbrack; 비등방성 및 수정된 각도로 미리 보기 구 업데이트
* &lbrack;Content&rbrack; 업데이트된 matFx 셔터
* &lbrack;Content&rbrack; 새로운 Texturing.XYZ 원활한 얼굴 스캔
* &lbrack;Content&rbrack; 새로운 비등방성 절차
* &lbrack;Content&rbrack; 새 필터: 베이크된 조명 환경
* &lbrack;Content&rbrack; 새로운 환경 맵: 스튜디오 자동차 중립
* &lbrack;Content&rbrack; 새 프로젝트 템플릿: PBR - 금속 거칠기 비등방성 각도(비등방성 채널 포함)
* &lbrack;Content&rbrack; 새 프로젝트 템플릿: PBR - 금속 거칠기 코팅
* &lbrack;SVT&rbrack;&lbrack;Engine&rbrack; SVT(Sparse Virtual Textures)
* &lbrack;SVT&rbrack;&lbrack;Preferences&rbrack;&lbrack;UI&rbrack; SVT 하드웨어 지원 가속 옵션
* &lbrack;SVT&rbrack;&lbrack;Log&rbrack; 스파스 가상 텍스처링 기능(예: 디스크 크기)에 대한 추가 정보
* 디스크의 크기가 캐시에 비해 너무 낮은 경우 &lbrack;SVT&rbrack;&lbrack;UI&rbrack; 시작 시 메시지 창
* &lbrack;SVT&rbrack;&lbrack;Preferences&rbrack;&lbrack;UI&rbrack; Substance Painter 글로벌 캐시 위치
* &lbrack;SVT&rbrack; Substance Painter 캐시의 경로를 지정하는 새 환경 변수
* &lbrack;SVT&rbrack; SVT 하드웨어 지원 가속을 활성화하는 새로운 환경 변수
* &lbrack;SVT&rbrack; 하드웨어별 스파스 지원 검색
* &lbrack;SVT&rbrack;&lbrack;하드웨어 스파스&rbrack; Nvidia GPU용 최소 드라이버 버전 올리기
* &lbrack;SVT&rbrack;&lbrack;Shader&rbrack;&lbrack;Viewport&rbrack;&lbrack;UI&rbrack; 프로젝트를 열 때 스파스 가상 텍스처링(Sparse Virtual Texturing)이 있는 아티팩트가 있으면 사용자에게 경고합니다

**고정:**

* &lbrack;색상 피커&rbrack; 색상을 선택하려고 할 때 페인팅 커서가 나타남
* 특정 순서로 레이어를 선택하거나 선택 취소하여 충돌을 수행하면 충돌이 발생할 수 있습니다
* 마스크가 있는 레이어를 인스턴스로 붙여넣을 때 충돌
* 사용자 채널 이름을 바꿀 때 &lbrack;사용자 채널&rbrack;&lbrack;회귀&rbrack; 충돌
* &lbrack;사용자 채널(&amp;r); 회색 브러시 미리 보기
* &lbrack;Alembic&rbrack; 가져오기 후 여러 재질에서 하나의 텍스처만 설정됨
* &lbrack;Engine&rbrack; 내보낸 텍스처가 브러시 스탬프에 대한 뷰포트와 다름
* &lbrack;Engine&rbrack; 레벨 효과를 사용한 반전은 텍스처에 완전히 영향을 주지 않습니다.
* 재료 선택기가 선택하는 동안 브러시 획을 적용하고 있음
* 해상도를 128x128px로 전환하면 충돌이 발생합니다
* 레이어를 다시 굽거나 인스턴스화할 때 메시 맵 링크가 제대로 업데이트되지 않음
* &lbrack;user&rbrack; UserData ColorSpace가 [굽은 메시 표준] 입력 시 작동하지 않음
* 여러 셰이더스 인스턴스를 사용할 때 MDL 연결 불일치
* &lbrack;대칭&rbrack;&lbrack;칠 레이어&rbrack; 대칭 평면과 칠 레이어에서 활성화된 해당 조작기
* &lbrack;Viewport&rbrack; 클릭 후 번역을 위한 피벗 포인트가 업데이트되지 않음
* &lbrack;UI&rbrack; HDPI 모니터용 고정 아이콘 및 자리 표시자 제거

**알려진 문제:**

* 경우에 따라 AMD VEGA GPU에서 계산 중단
* Windows OS의 단축키와 관련된 Huion 태블릿 문제
* 앤티 앨리어싱과 그림자를 함께 활성화하면 예기치 않은 결과가 발생할 수 있습니다

### 4.2.3 (2018.2.3)

*(릴리스: 2018년 9월 25일)*

**고정:**

* 새 프로젝트를 만들 때 일부 메시로 인해 &lbrack;2D 보기&rbrack; 2D 보기가 끊김
* &lbrack;충돌&rbrack; UV 투영에서 평면 투영으로 전환하면 충돌이 표시됩니다.
* &lbrack;RayCollider&rbrack; &quot;RayCollider&quot;로 인한 다중 충돌
* &lbrack;도구&rbrack; 레이어 전환 시 수정된 브러시 속성이 손실됩니다.
* 지우개로 전환할 때 브러시 설정이 재설정됨

**알려진 문제:**

* AMD VEGA GPU에서 계산 중단
* Windows OS의 단축키와 관련된 Huion 태블릿 문제

### 4.2.2 (2018.2.2)

*(릴리스: 2018년 9월 11일*)요약: **콘텐츠 업데이트, 새로운 스크립팅 기능 및 자동 업데이트를 비활성화할 수 있는 핫픽스**

**추가됨:**

* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; 스킨 셸프 사전 설정 추가
* &lbrack;Content&rbrack;&lbrack;shelf&rbrack; 19개의 피부 표준을 표면 아래 산란용 재료로 변환
* &lbrack;스크립팅&rbrack; 열려 있는 프로젝트에서 프로젝트 템플릿 만들기
* &lbrack;스크립팅&rbrack; 열린 프로젝트의 내보내기 설정 가져오기/설정
* &lbrack;Updates&rbrack; 설정 및 환경 변수에서 자동 업데이트 팝업을 비활성화할 수 있습니다
* &lbrack;Updates&rbrack; 유지 관리 기한이 지난 팝업에서 다음 버전까지 표시되지 않습니다.

**고정:**

* &lbrack;Camera&rbrack; 직교에서 원근감으로 전환하여 잘못된 확대/축소
* &lbrack;Display&rbrack; 일부 맵이 sRGB 대신 선형으로 표시됨
* &lbrack;Viewports&rbrack; 메시 포커스가 제대로 작동하지 않음
* &lbrack;2D 보기&rbrack; 끊어진 카메라가 있는 프로젝트의 UV 쉘이 사라짐
* &lbrack;SSS&rbrack;&lbrack;Tooltip&rbrack; 서브서피스 분산 도구 설명이 로그에 나타납니다
* 일부 프로젝트는 2018.2에서 열 수 없으며 오류 메시지는 null substance 패키지를 저장할 수 없습니다.
* 마스크에서 작업할 때 경우에 따라 &lbrack;Mask&rbrack; 페인트 도구 색상이 중단될 수 있습니다
* &lbrack;재료&rbrack; 특정 상황에서 표시되지 않는 맵
* 생성기를 사용하여 활성화된 &lbrack;Proj&rbrack;&lbrack;Tools&rbrack; 조작기
* &lbrack;Substance&rbrack; 매개 변수의 Substance 그룹이 누락되었습니다.
* &lbrack;스크립팅&rbrack; 설명서의 소프트웨어 이름이 잘못됨
* &lbrack;UDIM&rbrack; 여러 UV 타일의 UV 쉘에 대한 로그의 정보 없음

**알려진 문제:**

* AMD VEGA GPU에서 계산 중단
* Windows OS의 단축키와 관련된 Huion 태블릿 문제

### 4.2.1 (2018.2.1)

*(릴리스: 2018년 8월 3일)*

**고정:**

* 업그레이드 프로젝트에서 하위 표면 분산 셰이더 매개 변수가 누락되었습니다.

**알려진 문제:**

* AMD VEGA GPU에서 계산 중단
* Windows OS의 단축키와 관련된 Huion 태블릿 문제

### 4.2.0 (2018.2.0)

*(릴리스: 2018년 8월 2일*)요약: **여름 릴리스, 서브서피스 분산 지원, 투영 및 채우기 개선, 카메라 가져오기 및 선택, Alembic 및 glTF 지원, ID 맵에 대한 드래그 앤 드롭, 개선된 Substance 형식 지원 및 새 콘텐츠**

**추가됨:**

* &lbrack;SSS&rbrack;&lbrack;Viewport&rbrack;&lbrack;Iray&rbrack; 일반 서브서피스 분산
* &lbrack;SSS&rbrack; 동기화 MDL 및 서브서피스 스캐터링 매개변수
* &lbrack;SSS&rbrack;에 [분산]이라는 새 회색 음영 채널이 추가되었습니다.
* &lbrack;SSS&rbrack;&lbrack;Shader Settings&rbrack; 서브서피스 스캐터링(스킨 또는 반투명)을 위한 스캐터링 유형 매개 변수
* &lbrack;SSS&rbrack;&lbrack;Shader Settings&rbrack; 서브서피스 스캐터링을 위한 스캐터링 비율 매개 변수
* &lbrack;SSS&rbrack;&lbrack;Shader Settings&rbrack; 서브서피스 스캐터링을 위한 스캐터링 색상 매개 변수
* &lbrack;SSS&rbrack;&lbrack;Display Settings&rbrack; 서브서피스 스캐터링을 위한 스캐터링 샘플 수
* &lbrack;Shader&rbrack;&lbrack;Iray&rbrack; Iray에 대한 서브서피스 스캐터링 MDL 통합
* &lbrack;Shader&rbrack; 리소스 업데이터를 통한 셰이더 업데이트
* &lbrack;Shader&rbrack; 변경 로그 API 및 설명서 업데이트
* &lbrack;도구 등록 정보&rbrack;&lbrack;프로젝트&rbrack; 삼면 투영의 새 매개변수
* &lbrack;Viewport&rbrack;&lbrack;Proj&rbrack; 조작기로 직접 3D 보기에서 레이어 채우기 속성 제어(삼평면 투영)
* &lbrack;Shortcuts&rbrack;&lbrack;Proj&rbrack; 삼면형 투영 조작기에 대한 새 단축키 Q, W, E, R, T
* &lbrack;Viewport&rbrack;&lbrack;Proj&rbrack; 조작기(UV 투영)를 사용하여 직접 2D 보기에서 레이어 속성 채우기 제어
* &lbrack;Shortcuts&rbrack;&lbrack;Proj&rbrack; UV 투영 조작기를 위한 새로운 단축키 Q
* &lbrack;Contextual Toolbar&rbrack;&lbrack;Proj&rbrack; Control triplanar 투영 조작기
* &lbrack;상황별 도구 모음&rbrack;&lbrack;프로젝트&rbrack; 제어 UV 투영 조작기
* &lbrack;도구 속성&rbrack; 투영 및 스텐실 도구로 텍스처 타일링 비활성화
* &lbrack;Stencil&rbrack; 투영 도구/스텐실과 함께 사각형이 아닌 이미지 사용
* &lbrack;Stencil&rbrack; 속성 창에서 타일링 모드 제어 허용
* &lbrack;Stencil&rbrack; 확대/축소가 타일링하지 않은 스텐실의 중심에 있지 않음
* &lbrack;Cameras&rbrack; Maya, Max, Blender, Modo, DAE에서 카메라 가져오기
* &lbrack;Cameras&rbrack;&lbrack;Viewport&rbrack; 가져온 카메라를 뷰포트에서 선택 및 제어
* &lbrack;Cameras&rbrack;&lbrack;Iray&rbrack; Iray에서 가져온 카메라 선택 및 제어
* &lbrack;Cameras&rbrack;&lbrack;UI&rbrack;&lbrack;New project&rbrack;&lbrack;Project configuration&rbrack; 카메라 가져오기가 기본적으로 선택되어 있습니다.
* &lbrack;Cameras&rbrack;&lbrack;Shortcuts&rbrack; 카메라 간 전환에 대한 단축키 추가
* &lbrack;Cameras&rbrack;&lbrack;Viewport&rbrack; 뷰포트에 프레임 추가
* &lbrack;Cameras&rbrack;&lbrack;Viewport Settings&rbrack; 프레임 불투명도 제어
* &lbrack;Cameras&rbrack;&lbrack;Camera Settings&rbrack; 최대 초점 거리(500mm)
* &lbrack;Cameras&rbrack;&lbrack;Camera Settings&rbrack; 노출 비율
* &lbrack;Cameras&rbrack;&lbrack;Camera Settings&rbrack; 잠금 옵션 추가
* &lbrack;Cameras&rbrack;&lbrack;Camera Settings&rbrack; 복원 옵션 추가
* &lbrack;Cameras&rbrack;&lbrack;Camera Settings&rbrack; Add focus distance attribute
* &lbrack;glTF&rbrack; glTF 파일 가져오기
* &lbrack;glTF&rbrack; 가져오기 앰비언트 오클루전 맵
* &lbrack;Alembic&rbrack; 정적 형상이 있는 Alembic 1 프레임 가져오기
* &lbrack;Shelf&rbrack; 수정자(CTRL/Command)와 함께 ID 맵을 사용하여 재료를 메시로 직접 드래그하여 놓기
* &lbrack;레이어 스택&rbrack; ID 맵이 있는 메시의 재료 드래그 앤 드롭으로 자동 ID 마스크 만들기
* &lbrack;레이어 스택&rbrack; 레이어 스택을 가로질러 드래그하여 놓아 레이어의 자동 스크롤
* &lbrack;UI&rbrack;&lbrack;도구 속성&rbrack; Substance 사전 설정 노출
* &lbrack;UI&rbrack;&lbrack;도움말 메뉴&rbrack; 도움말 메뉴 개선
* &lbrack;UI&rbrack;&lbrack;새 프로젝트&rbrack;&lbrack;프로젝트 구성&rbrack; 창 재구성
* &lbrack;UI&rbrack;&lbrack;새 프로젝트&rbrack;&lbrack;프로젝트 구성&rbrack; 메시 용어를 파일로 바꾸기
* &lbrack;UI&rbrack;&lbrack;Substance&rbrack; UI에서 Substance 속성 표시
* &lbrack;Shortcuts&rbrack; 2D와 3D 보기 간 F4 스위치
* &lbrack;단축키&rbrack; 전환 스텐실 N 및 빠른 마스크 U에 대한 새로운 단축키
* &lbrack;Substance 통합&rbrack; Substance 매개변수의 &#39;visible if&#39; 문을 고려합니다.
* &lbrack;뷰포트&rbrack; 카메라 이동 후 그림자를 강제로 계산하지 않음
* &lbrack;Content&rbrack; 가져온 카메라로 MeetMat 업데이트
* &lbrack;Content&rbrack; 서브서피스 스캐터링이 활성화된 샘플 추가 - JadeToad
* &lbrack;Content&rbrack; 서브서피스 스캐터링이 활성화된 새 PBR 프로젝트 템플릿 추가
* &lbrack;Content&rbrack; 새 분산 채널을 추가하도록 내보내기 사전 설정을 업데이트했습니다.
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; pbr-metal-rough-alpha-test, pbr-coated, pbr-spec-gloss에 대한 서브서피스 스캐터링 지원 추가
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; 5개의 스마트 재질(마블 및 스킨)에 분산 채널 추가
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; 1개의 새로운 옥 재질
* &lbrack;Content&rbrack;&lbrack;Shelf&rbrack; 1개의 새로운 왁스 재질

**고정:**

* &lbrack;CMD&rbrack; 다른 버전에서 동일한 명령줄을 사용하는 다른 결과
* &lbrack;TDR&rbrack; TdrLevel이 설정된 경우 로그에 오류가 없습니다
* &lbrack;Baker&rbrack; 앰비언트 오클루전 맵이 뒤집힘
* 0-1 범위 밖에서 선택할 때 &lbrack;ID Map&rbrack;이 충돌합니다.
* 텍스처 설정을 전환하고 페인트 모드로 돌아갈 때 &lbrack;Array&rbrack; 충돌
* &lbrack;뷰포트(&amp;r); 드래그 앤 드롭을 위한 뷰포트 간 드롭 영역 동기화
* &lbrack;Engine&rbrack; 칠 레이어를 타일링하거나 작은 브러시를 칠할 때 아티팩트 수정
* &lbrack;License&rbrack; 라이선스 서비스 잘못된 소프트웨어 버전 확인
* &lbrack;License&rbrack; 인증 처리 방식 재작업
* &lbrack;API&rbrack; 템플릿으로 작성하는 경우에도 onNewProjectCreated 스크립팅 API 이벤트를 호출합니다.
* &lbrack;Shader&rbrack; 컴파일된 셰이더는 셰이더 파일이 컴파일되지 않을 때 캐시에서 로드되지 않습니다.
* &lbrack;Shelf&rbrack; 셸프에서 HDR 파일을 내보내면 고정된 값이 있는 파일이 출력됩니다.
* &lbrack;Export&rbrack; EXR export clamps RGB 색상 값(0-1 사이)
* &lbrack;Content&rbrack; 프로시저 노이즈 3D Perlin 노이즈 프랙탈이 픽셀화됨

**알려진 문제:**

* AMD VEGA GPU에서 계산 중단
* Windows OS의 단축키와 관련된 Huion 태블릿 문제

### 4.1.3 (2018.1.3)

*(릴리스: 2018년 6월 28일)*

**추가됨:**

* &lbrack;Preferences&rbrack; Painter이 다시 시작될 때 프로젝트 저장 제안

**고정:**

* &lbrack;Plugin&rbrack; 검색 Substance Source이 작동하지 않음
* &lbrack;스마트 재질&rbrack; 스마트 재질을 가져오면 경우에 따라 충돌이 발생합니다
* &lbrack;스마트 재질&rbrack; 스마트 재질을 삭제하면 경우에 따라 충돌이 발생합니다.
* &lbrack;Save&rbrack; 저장하기 위해 충돌이 발생하는 경우가 있습니다.
* &lbrack;Shelf&rbrack; Invert가 셀 2 및 셀 3에서 작동하지 않음
* 일부 Alpha에서 &lbrack;Shelf&rbrack; Typo
* &lbrack;Shelf&rbrack; 일부 Substance 재질이 제대로 렌더링되지 않음

**알려진 문제:**

* AMD VEGA GPU에서 계산 중단

### 4.1.2 (2018.1.2)

*(릴리스: 2018년 6월 12일*)요약: **개선된 굽기 속도, 개선된 저장 시스템, 업데이트된 슬라이더, 업데이트된 플러그인 API, 중국어 번역, 개선된 패딩 지금 선택 사항**

**추가됨:**

* &lbrack;Bakers&rbrack; 새로운 베이커 버전으로 성능 향상
* 호환되지 않는 GPU가 있는 강제 표시 대화 상자
* &lbrack;Save&rbrack; 새로운 압축 프로젝트 기능(전체/압축 저장 모드) 노출
* &lbrack;저장&rbrack; 저장 오류 시 사용자에게 알리기
* &lbrack;Clean&rbrack; 전체/압축 모드에서 다음 저장
* &lbrack;슬라이더&rbrack; 색상/회색 음영 막대 및 슬라이더의 정밀도 향상
* &lbrack;슬라이더&rbrack; 위쪽/아래쪽 화살표 컨트롤 추가
* &lbrack;슬라이더&rbrack; 색상 및 회색 음영 막대 슬라이더의 동일한 감지 영역
* &lbrack;Plugin&rbrack; 항상 증분 모드에서 자동 저장
* &lbrack;Plugin&rbrack; 플러그인을 새 인터페이스 스타일로 전환하는 옵션
* &lbrack;언어&rbrack; 중국어 번체 추가
* &lbrack;Padding&rbrack; 텍스처 세트 설정에서 텍스처당 UV 및 3D 공간 인접 패딩 사이를 전환하는 옵션
* &lbrack;스크립트&rbrack; 저장 모드 노출: 전체/압축 또는 증분
* &lbrack;스크립트&rbrack; 스크립팅/QML 설명서 업데이트
* &lbrack;Log&rbrack; 로그에서 저장 모드(전체/압축 또는 증분) 표시

**고정:**

* &lbrack;도구&rbrack;채널 슬롯 변환을 단일 채널 채우기의 재료 슬롯으로 연결
* 특정 면이 재질에 의해 할당되지 않은 메시(FBX)를 로드할 때 충돌 발생
* 가상 시스템에서 NVIDIA GRID 5.2를 사용하여 Iray의 충돌
* 재질 사전 설정 삭제를 실행 취소할 때 충돌
* 일부 프로젝트 로드 시 충돌
* &lbrack;명령줄&rbrack; udim별로 분할된 UDIM 메시에 대한 새 명령줄
* &lbrack;도구 모음&rbrack; 도구 모음 축소
* &lbrack;Instanceing&rbrack;에서는 여러 텍스처 세트에서 비트맵을 인스턴스화할 수 없습니다.
* 타일 UV로 메시를 페인트할 때 &lbrack;Viewport&rbrack; 새로 고침이 완료되지 않음
* &lbrack;Iray&rbrack; 노멀 맵이 유전체에 대해 두 번 적용됨
* &lbrack;Shelf&rbrack; 일부 Substance 매개 변수의 오타(alphas, procedurals 및 matfx)
* &lbrack;Shelf&rbrack; 비트맵 &quot;Authorized Personnel Only&quot;에 대한 오타
* &lbrack;Script&rbrack; 함수 alg.shaders.materials()가 더 이상 작동하지 않습니다

**알려진 문제:**

* AMD VEGA GPU에서 계산 중단

### 4.1.1 (2018.1.1)

*(릴리스: 2018년 4월 3일)*

**고정:**

* &lbrack;Tablet&rbrack; 기본 상호 작용 선택 변경 시 문제
* &lbrack;Bakers&rbrack; 라이브러리 연결 충돌
* &lbrack;Bakers&rbrack; A.O. 맵으로 성능 회귀
* &lbrack;Iray&rbrack; 렌즈 왜곡이 알파 채널에 적용되지 않습니다.
* &lbrack;드라이버&rbrack; 최소 드라이버 요구 사항 업데이트
* &lbrack;3Dview&rbrack; 정규식 정보가 없는 UDIM 메시에서 정규식이 올바르게 생성되지 않습니다.
* &lbrack;Intel&rbrack; 충돌(Substance Painter 2018.1.0 포함)
* &lbrack;Intel&rbrack;&lbrack;Viewport&rbrack; 패딩 문제(검은색 아티팩트)

**알려진 문제:**

* AMD VEGA GPU에서 계산 중단

### 4.1.0 (2018.1.0)

*(릴리스: 2018년 3월 15일)*

**추가됨:**

* 새로운 전체 스타일(아이콘, 색상, 비헤이비어)
* 새 기본 레이아웃
* &lbrack;Tablet&rbrack; 페인팅 중 사용자 환경 개선
* &lbrack;기본 메뉴&rbrack; 뷰 및 도구 모음의 기본 항목을 먼저 정렬합니다.
* &lbrack;기본 메뉴&rbrack; 뷰포트 섹션에서 빠른 마스크 이동 작업
* &lbrack;기본 메뉴&rbrack; 마우스 오른쪽 버튼 클릭 동작을 뷰포트 섹션으로 이동
* &lbrack;기본 메뉴&rbrack; &quot;보기&quot; 메뉴의 이름을 &quot;창&quot;으로 바꾸기
* &lbrack;빠른 메뉴&rbrack; 뷰포트에서 마우스 오른쪽 버튼으로 클릭하는 새 도구 속성
* &lbrack;Dock widget&rbrack; 빠른 감소/회수를 위한 새로운 Dock 도구 모음
* &lbrack;디스플레이 설정&rbrack; 카메라 및 뷰어 설정 창 병합
* &lbrack;레이어 스택&rbrack; 상황에 맞는 오른쪽 클릭 메뉴
* &lbrack;레이어 스택&rbrack; 드래그 앤 드롭하여 동일한 레이어 내에서 효과를 이동합니다
* &lbrack;도구 모음&rbrack; 도구 모음 및 새로운 상황별 도구 모음 재구성
* &lbrack;도구 도구 도구 모음&rbrack; 복제 도구를 두 개의 개별 도구로 분할
* 미리 보기에서 배경 회색 음영 값이 더 밝게 표시되는 &lbrack;도구 속성&rbrack;
* &lbrack;도구 등록 정보&rbrack; 탭 구성(채우기 및 도구)
* &lbrack;도구&rbrack; 페인팅 결과가 스텐실과 일치함
* &lbrack;뷰포트&rbrack; 칠 레이어용 새 커서
* &lbrack;뷰포트&rbrack; 더 매끄러운 탐색 및 페인팅(더 높은 프레임 속도)
* &lbrack;뷰포트&rbrack; 재료/채널/맵 선택 콤보 상자(뷰포트)
* &lbrack;뷰포트&rbrack; 회전하는 동안 깜박임 감소(그림자 표시)
* &lbrack;Shelf&rbrack; Painter을 열 때 기본적으로 재질 표시
* &lbrack;Shelf&rbrack; Substance 텍스처 및 재료의 로드 시간 개선(2~6배 더 빠름)
* &lbrack;Shelf&rbrack; Substance Source 구조에 맞게 재질 폴더 재구성
* &lbrack;Shelf&rbrack; 재질을 뷰포트의 메시에 직접 끌어다 놓습니다
* &lbrack;Shelf&rbrack; 새로운 3D 노이즈(Perlin, Perlin Fractal, Simplex 및 Worley)
* &lbrack;Shelf&rbrack; 메쉬 위치를 사용하는 새 3D Linear gradient 마스크 생성기
* &lbrack;Shelf&rbrack; 비정사각형 확장 지원을 위한 기본 노이즈 업데이트
* &lbrack;Shelf&rbrack; Lens Studio(스냅 응용 프로그램)에 대한 새 템플릿 및 내보내기 사전 설정을 추가했습니다.
* &lbrack;Shelf&rbrack; 최신 버전의 마스크 편집기(마이크로 디테일)를 사용하도록 스마트 재질 및 스마트 마스크를 업데이트했습니다.
* &lbrack;Shelf&rbrack; 매끄러운 타일링 재료를 만들기 위한 새로운 샘플 프로젝트 &quot;TilingMaterial&quot;
* &lbrack;Shelf&rbrack; 새 브러시 사전 설정(캘리그래피, 젖은 색상, 해칭 등)
* &lbrack;슬라이더&rbrack; 새로운 슬라이더 및 회색 음영/색상 막대 스타일 및 비헤이비어
* &lbrack;Bakers&rbrack; 전체 장면 경계 상자를 사용하여 위치 맵 계산 허용
* &lbrack;Shader&rbrack; 기본 셰이더 매개 변수에서 Height 강제 매개 변수를 제거합니다.
* &lbrack;엔진&rbrack; Substance 엔진 업데이트됨
* &lbrack;엔진&rbrack; UV 청크에 걸쳐 불연속성이 없거나 적음
* &lbrack;Plugins&rbrack; Substance Source에서 다운로드한 자료를 더 빠르게 가져오기
* &lbrack;Plugins&rbrack; 새로운 전체 스타일에 맞게 모든 플러그인 업데이트
* &lbrack;환경 설정&rbrack; 미리 보기 배경색이 자동으로 변경됨
* &lbrack;Clean&rbrack; 프로젝트 손상 위험 감소
* &lbrack;Open&rbrack; 프로젝트 시간 개선 열기
* &lbrack;새 프로젝트&rbrack; 새 프로젝트 - 메시 업데이트 시간 개선
* &lbrack;저장&rbrack; 저장 프로젝트 시간 개선
* &lbrack;Log&rbrack; 라이센스 유형이 로그에 보고됨
* &lbrack;TextureSet&rbrack; &quot;베이크 텍스처&quot; 단추의 이름을 &quot;베이크 메시 맵&quot;으로 바꾸기
* &quot;추가 맵&quot;의 이름을 &quot;망 맵&quot;으로 바꾸기

**고정:**

* &lbrack;Viewport&rbrack; 하위 개체가 많이 포함된 메시의 성능 저하
* 이미지를 질감 슬롯으로 드래그하여 놓을 때 &lbrack;도구 등록 정보&rbrack; 채널이 비활성화됨
* &lbrack;도구 속성&rbrack; 브러시 미리 보기가 손가락 및 복제 도구로 끊김
* 템플릿을 사용할 때 &lbrack;텍스처 set&rbrack; 채널 순서가 잘못됨
* &lbrack;Shelf&rbrack; 회색 음영 전환 생성기의 누락 아이콘
* &lbrack;Shelf&rbrack; Sign Circle Number 알파가 끊김(누락된 글꼴)
* 실행 시 통합 GPU가 잘못 감지됩니다.
* &lbrack;충돌&rbrack; # 문자가 있는 이름의 가져온 리소스를 드래그 앤 드롭합니다
* 통합 GPU에서 &lbrack;엔진&rbrack; Vram 감지 문제
* &lbrack;Engine&rbrack; Substance 엔진 링커의 수많은 충돌 수정
* 해상도 변경 시 &lbrack;Engine&rbrack; Square 아티팩트
* 포스트 효과가 켜져 있을 때 &lbrack;포스트 효과&rbrack; 인터페이스 크기 조정이 느려짐
* &lbrack;Bakers&rbrack; 장면 단위가 광선 거리 값에 대해 올바르게 적용되지 않습니다.
* &lbrack;Bakers&rbrack; 메시 오클루더 거리의 AO는 입력 값에 관계없이 1로 클램핑됩니다.
* &lbrack;Bakers&rbrack; 이름별 일치는 특정 이름의 일부 메시를 무시함
* &lbrack;Bakers&rbrack; 메시 폴리그룹 및 서브메시 ID 설정의 색상이 항상 검은색 이미지를 반환합니다.
* &lbrack;Bakers&rbrack; Blender에서 이진 FBX 메시로 ID 굽기가 실패합니다
* &lbrack;Shader&rbrack; dota-2 및 비 pbr-spec-gloss가 있는 2D 보기의 노이즈
* &lbrack;Linux&rbrack; 굽기 시 하나의 CPU 스레드만 사용됨
* 브러시 커서가 뷰포트 위로 이동하는 &lbrack;MacOS&rbrack; 충돌

**알려진 문제:**

* AMD VEGA GPU에서 계산 중단
* IRay(알파)에서 내보내는 동안 왜곡 후 프로세스가 고려되지 않음

## 버전 3

### 3.4.2 (2017.4.2)

*(릴리스: 2018년 1월 24일)*

**추가됨:**

* &lbrack;Export&rbrack; 단계 진행과 함께 내보내기 상태 가져오기
* &lbrack;내보내기&rbrack; 내보내기 취소 허용
* &lbrack;Export&rbrack; 노멀 맵 품질 손실 없이 Sketchfab으로 텍스처 내보내기
* &lbrack;Export&rbrack; glTF 이진 형식(glb)으로 내보내기
* &lbrack;내보내기&rbrack; 내보내기 창의 구성 탭에서 열 크기 조정 허용
* &lbrack;Shader&rbrack; 셰이더 API 변경 로그 추가
* &lbrack;Scripting&rbrack; 텍스처 내보내기 시 이전 및 이후 콜백 함수 추가
* &lbrack;Iray&rbrack; SDK 2017.1로 업그레이드(Volta GPU 지원)

**고정:**

* 주 창이 표시되기 전에 응용 프로그램을 종료할 때 충돌
* IRAY를 사용하여 회색 음영 맵을 로드할 때 &lbrack;MAC&rbrack; 충돌
* &lbrack;MAC&rbrack; VRAM 감지가 새로운 High Sierra OS에서 올바르지 않음
* &lbrack;Plugin&rbrack; Substance Source에서 에셋 다운로드가 더 이상 작동하지 않음
* &lbrack;스크립팅&rbrack; 잘못된 최소 플러그인 버전 감지
* &lbrack;Export&rbrack; 텍스처 내보내기 후 내보내기 사전 설정 저장 실패
* 추가 맵이 없는 TextureSet에서 인스턴스화된 생성기에서 &lbrack;Instanceing&rbrack; 문제
* &lbrack;Viewport&rbrack; 디더링이 4k 이상의 해상도에서 작동하지 않습니다.
* &lbrack;뷰포트&rbrack; 2D 보기 재료 디스플레이가 노이즈로 덮여 있음
* &lbrack;Shelf&rbrack; 선반 사전 설정의 로드 시간 개선
* &lbrack;Engine&rbrack; 색상 선택 영역 아래에 페인팅할 때 잘못된 혼합

### 3.4.1 (2017.4.1)

*(릴리스: 2017년 12월 15일)*

**추가됨:**

* &lbrack;스크립팅&rbrack; 스크립팅 API를 통해 메시 내보내기
* &lbrack;Import&rbrack; 지원되지 않는 메시 파일 형식(obj, fbx, dae, ply만 허용)의 가져오기 비활성화
* &lbrack;Log&rbrack; 로그 파일에서 TDR 문제를 더 정확하게 표시

**고정:**

* 리소스 탐색이 완료되기 전에 응용 프로그램이 닫혀 있는 경우 충돌
* 손가락/복제 도구로 프로젝트를 열 때 충돌
* 뷰어 설정에서 셰이더 변경 실행 취소 후 다시 실행을 사용할 때 충돌 발생
* &lbrack;Engine&rbrack; Texturing은 Painter 2017.2와 2017.4에서 서로 다릅니다.
* &lbrack;Viewport&rbrack; 인스턴스에서 ID 맵을 선택하면 잘못된 색상이 샘플링됩니다.
* 잘못된 일반 또는 오클루전 텍스처를 내보낼 때 &lbrack;Export&rbrack; 충돌
* &lbrack;내보내기&rbrack; PSD 파일을 Photoshop CS6에서 열 때 해당 그룹이 잠김
* &lbrack;Plugin&rbrack; Photoshop 플러그인은 채널 선택을 무시하고 항상 모든 것을 내보냅니다.
* 텍스처 세트 간에 복사/붙여넣을 때 &lbrack;레이어&rbrack; 고정점 나누기
* &lbrack;Layers&rbrack; 일부 앵커 참조가 손상된 경우 복원할 수 없습니다.
* &lbrack;Shader&rbrack; pbr-coated secondary roughness 매개변수가 끊어짐
* 시작 시 &lbrack;Steam&rbrack; 버전 검사기 팝업이 표시되지 않아야 합니다.

**알려진 문제:**

* &lbrack;AMD&rbrack; 충돌/메시에서 페인트를 시도할 때 멈춤 GPU 드라이버 업데이트로 수정할 수 있습니다.

### 3.4.0 (2017.4.0)

*(릴리스: 2017년 11월 23일)*

**추가됨:**

* &lbrack;인스턴스화(&amp;r); 레이어 간에 매개 변수를 인스턴스화할 수 있습니다.
* &lbrack;인스턴스 지정&rbrack; 소스 레이어와 인스턴스 간 이동 허용
* &lbrack;인스턴스화(&amp;r); &quot;텍스처 세트 간 인스턴스화&quot; 작업 추가
* &lbrack;Instancing&rbrack; 레이어 스택 재진입 인스턴스(주기)를 나타냅니다.
* &lbrack;인스턴스(&amp;r); 소스가 제거되면 인스턴스 삭제
* &lbrack; 인스턴스화(&amp;r); 인스턴스화된 폴더 외부로부터의 앵커 참조 허용 안 함
* &lbrack;UI&rbrack; 실행 취소 스택을 &quot;기록&quot;이라는 이름의 자체 창으로 이동합니다.
* &lbrack;Plugin&rbrack; DCC 라이브 링크 플러그인 통합
* &lbrack;엔진&rbrack; 스파스 페인팅으로 페인팅 성능 향상
* &lbrack;내보내기&rbrack; Sketchfab 내보내기 도구에 초안 추가 및 재내보내기 옵션
* &lbrack;Shelf&rbrack; 글꼴 재질에 대한 &quot;뒤집기&quot; 컨트롤 추가
* &lbrack;Shelf&rbrack; 20개의 새로운 절차 자료 추가
* &lbrack;Shelf&rbrack; 40개의 새로운 그런지 맵 추가(비트맵 기반 및 프로시저)
* &lbrack;뷰포트(&amp;r); 표시되는 다른 텍스처 세트에서 브러시 미리 보기 충돌 활성화
* AMD GPU 드라이버 최소 요구 사항 업데이트

**고정:**

* 충돌 너무 큰 해상도에서 Substance을 계산할 때
* 입자를 사용하여 과하게 페인팅할 때 충돌
* &lbrack;Viewport&rbrack; 특정 메시가 있는 2D 보기에서 Specular 반사가 잘못됨
* &lbrack;UI&rbrack; 일부 원치 않는 작업이 작업 내역 창에 나타납니다.

**알려진 문제:**

* &lbrack;Layers&rbrack; 일부 앵커 참조가 손상된 경우 복원할 수 없습니다.
* 뷰어 설정에서 셰이더 변경 실행 취소 후 다시 실행을 사용할 때 충돌 발생

### 3.3.3 (2017.3.3)

*(릴리스: 2017년 12월 1일)*

**고정:**

* 시작 시 &lbrack;Steam&rbrack; 버전 검사기 팝업이 표시되지 않아야 합니다.
* &lbrack;내보내기&rbrack; PSD 파일을 Photoshop CS6에서 열 때 해당 그룹이 잠김

### 3.3.2 (2017.3.2)

*(릴리스: 2017년 11월 20일)*

**추가됨:**

* &lbrack;UI&rbrack; 새 버전 대화 상자 개선 및 변경 로그 추가
* &lbrack;UI&rbrack; 새 버전 대화 상자에서 유지 관리가 만료되었는지 여부를 나타냅니다.
* &lbrack;License&rbrack; 유지 관리 날짜를 처리하도록 라이선스 시스템 업데이트
* &lbrack;내보내기&rbrack; Adobe Standard Material 이름을 Adobe Dimension으로 바꾸기

**고정:**

* &lbrack;Mac&rbrack; 페인팅은 검은색 사각형과 텍스처 손상을 유발합니다
* &lbrack;엔진&rbrack; 캐시가 뷰포트에서 사라질 수 있습니다.
* &lbrack;엔진&rbrack; 메모리 압축 트리거 시 블록 가공물이 나타납니다.
* &lbrack;Baking&rbrack; 특정 망을 굽을 때 이상한 오류 메시지
* &lbrack;Export&rbrack; PSD이 잘못 작성되어 Photoshop에서 제대로 인식되지 않습니다
* &lbrack;Layers&rbrack; 여러 프로젝트에 레이어를 복사/붙여넣을 수 없습니다.
* 일반 입력에 대한 &lbrack;Substance&rbrack; 사용자 데이터 색상 공간이 뒤집어진 경우가 있습니다.
* &lbrack;Shelf&rbrack; Micro-normal in generators 반전 곡률을 출력함
* &lbrack;Shelf&rbrack; HSL 필터도 알파 채널에 영향을 줍니다.
* 종속성 누락으로 인해 Centos에서 &lbrack;Linux&rbrack; 설치가 실패합니다.
* 특정 경우 설치 관리자가 이전 설치에서 모든 리소스를 제거하지 않음

### 3.3.1 (2017.3.1)

*(릴리스: 2017년 10월 26일)*

**추가됨:**

* &lbrack;내보내기&rbrack; 프로젝트에서 메시 내보내기 허용
* &lbrack;Shelf&rbrack; 탭 제목에서 &quot;Sub-Shelf&quot;를 제거합니다.
* 템플릿에서 사후 프로세스 설정 저장
* TDR 메시지를 더 이해하기 쉽게 만듭니다.
* 오류를 보고하도록 설정 창 개선

**고정:**

* 여러 개의 하위 셸프를 삭제할 때 충돌 발생
* 엔진 계산 중에 레벨에서 다른 레벨로 전환할 때의 충돌
* 엔진 계산 중 Intel GPU의 &lbrack;Mac&rbrack; 충돌
* &lbrack;Mac&rbrack;&lbrack;Viewport&rbrack; 디더링이 활성화되어 있을 때 잘못된 성능
* &lbrack;Mac&rbrack; MacOS 10.13은 로그 파일에서 &quot;알 수 없는 버전&quot;으로 인식됩니다.
* &lbrack;Baker&rbrack; 케이지로 굽는 것은 더 이상 작동하지 않습니다
* &lbrack;레이어&rbrack; Ctrl + C 단축키(복사 작업)가 더 이상 작동하지 않음
* &lbrack;Layers&rbrack; 레이어를 붙여넣어도 앵커 참조가 있는 UI가 새로 고쳐지지 않음
* &lbrack;앵커&rbrack; 참조가 있는 레이어 복제 또는 복사/붙여넣기 시 링크가 끊어집니다.
* &lbrack;Export&rbrack; 8K 내보내기는 경우에 따라 응용 프로그램을 충돌 또는 교착 상태로 만들 수 있습니다.
* &lbrack;내보내기&rbrack; 생성된 glTF 파일 형식의 다중 문제
* &lbrack;가져오기&rbrack; 같은 파일 이름의 메시 다시 가져오기가 더 이상 작동하지 않습니다
* &lbrack;Plugin&rbrack; 자동 저장 창은 항상 모든 것 위에 나타납니다.
* tdr 대화 상자에서 &quot;Escape&quot;를 누를 때 &lbrack;UI&rbrack; 무한 루프
* &lbrack;UI&rbrack; 재설정 UI는 선반 창의 두 번째 제목 표시줄을 표시합니다.

### 3.3.0 (2017.3.0)

*(릴리스: 2017년 9월 28일)*

**추가됨:**

* &lbrack;Export&rbrack; Adobe 프로젝트 Felix에 대한 메시 및 텍스처 내보내기 허용
* &lbrack;내보내기&rbrack; glTF 파일 형식으로 내보내기 허용
* &lbrack;엔진&rbrack; 블록 압축을 사용하여 VRAM에서 텍스처 크기 최적화
* &lbrack;Viewport&rbrack; 메쉬 또는 프로젝트를 뷰포트에 끌어다 놓을 수 있습니다.
* &lbrack;UI&rbrack; TDR에 대한 경고 메시지 개선
* &lbrack;UI&rbrack; 로그는 요청 시에만 표시되어야 합니다.
* &lbrack;UI&rbrack; 로그 창의 내용을 지울 수 있도록 허용
* &lbrack;UI&rbrack; 상태 표시줄에 경고 및 오류 표시
* &lbrack;UI&rbrack; 웹 브라우저에서와 마찬가지로 탭을 맨 위에 표시
* &lbrack;UI&rbrack; &quot;채색 가능 사용 안 함&quot; 컨텍스트 및 메시지 개선
* &lbrack;UI&rbrack; 파일 메뉴에서 &quot;사본으로 저장&quot; 동작을 추가합니다.
* &lbrack;레이어&rbrack; 기본 타일링 설정을 1로 기본적으로 설정
* &lbrack;Shelf&rbrack; 10가지 동적 색상을 지원하도록 그레이디언트 필터를 개선했습니다.
* &lbrack;Shelf&rbrack; 미니 셸프의 기본 쿼리에 공백을 추가합니다.
* &lbrack;Shelf&rbrack; 셸프의 로컬 리소스에 대해 &quot;탐색기에서 열기&quot; 동작을 추가합니다.
* &lbrack;Shelf&rbrack; Adobe Material Standard에 대한 템플릿 및 셰이더 추가(Project Felix)
* &lbrack;Shelf&rbrack; 재질 레이어 음영에서 최대 타일링을 128까지 증가
* &lbrack;Shelf&rbrack; 마스크 생성기의 마이크로 세부 사항에 대한 소벨 곡률 추가
* &lbrack;Plugin&rbrack; 사용자 정의 가능한 시간 간격을 가진 자동 저장 플러그인 추가
* &lbrack;스크립팅&rbrack; &quot;사본으로 저장&quot; 함수 추가

**고정:**

* 첫 번째 실행 시 &lbrack;UI&rbrack; 레이아웃이 중단됨
* &lbrack;내보낼 때 생성된 내보내기&rbrack; PSD에 형식 오류가 있음
* &lbrack;Export&rbrack; EXR은 항상 8비트 높이 맵을 내보냅니다.
* &lbrack;손상된 추가 맵을 내보낼 때 내보내기&rbrack; 충돌
* &lbrack;가져오기&rbrack; 하드 가장자리가 낮은 폴리 메쉬에서 보존되지 않는 경우가 있습니다
* &lbrack;가져오기&rbrack; 문제가 있는 메시를 가져올 때 오류 메시지가 개선되었습니다.
* &lbrack;Bakers&rbrack; ID 맵 굽기가 이름별로 일치 사용 가능으로 실패함
* &lbrack;뷰포트&rbrack; 탄젠트 공간이 베이커와 동기화되지 않음
* &lbrack;효과&rbrack; 레이어를 다시 이동하면 앵커 참조가 복원되지 않습니다
* &lbrack;Effect&rbrack; 고정점이 있는 두 마스크 간에 링크를 만들 때 새로 고침 문제
* &lbrack;효과&rbrack; 마스크 위의 마스크 고정점은 나열할 수 없습니다.
* &lbrack;효과&rbrack; 고정점에서 Alpha 추출 설정이 작동하지 않음
* &lbrack;엔진&rbrack; 첫 번째 브러시 획 후 마스크가 자체적으로 반전됨
* 특정 프로젝트에서 [텍스처 설정]을 전환할 때 &lbrack;Engine&rbrack; 충돌
* 프로젝트에 있는 사전 설정을 삭제할 때 &lbrack;Shelf&rbrack; 충돌
* &lbrack;Shelf&rbrack; Typo in advanced Tri-평면 filter
* &lbrack;Shelf&rbrack; MG 마스크 빌더 AO 노이즈 비율이 제대로 작동하지 않음
* &lbrack;Shelf&rbrack; MG Mask Builder에 반전된 곡률 매개 변수가 있음
* &lbrack;Shelf&rbrack; 가져온 알파에서 평면 구 미리 보기 대신 재질 구 미리 보기가 생성됩니다

### 3.2.0 (2017.2.0)

*(릴리스: 2017년 7월 27일)*

**추가됨:**

* 기준점 - 레이어 및 마스크 참조 시스템
* &lbrack;Layers&rbrack; 채우기 및 페인트 효과의 이름을 바꾸는 기능
* &lbrack;Plugin&rbrack; 업데이트된 Substance Source 플러그인
* &lbrack;스크립팅&rbrack; 텍스처 집합 해상도 쿼리 허용
* &lbrack;Scripting&rbrack; 페인팅 엔진의 상태를 가져올 수 있습니다.
* &lbrack;Performance&rbrack; 향상된 프로젝트 로드 및 브러시 스탬핑 최적화

**고정:**

* 재질 매개변수를 조정할 때 &lbrack;Tool&rbrack; 성능 문제가 발생합니다.
* &lbrack;엔진&rbrack; 해상도 변경 시 브러시 획 사라짐(4K>2K)
* &lbrack;3D 보기&rbrack; 탄젠트 공간이 베이커와 동기화되지 않음
* &lbrack;Shelf&rbrack; 사용자 문서의 Shelf 경로는 자동으로 생성되지 않습니다.
* &lbrack;Shelf&rbrack; 업데이트 후 사전 설정을 이전 버전과 호환되게 만듭니다.
* &lbrack;Shader&rbrack; 비PBR 셰이더가 더 이상 작동하지 않습니다.
* &lbrack;Bakers&rbrack; ID 맵 굽기가 이름별로 일치 사용 가능으로 실패함
* &lbrack;Sample&rbrack; Met Mat 샘플 프로젝트 텍스처 세트 이름이 올바르지 않음
* 템플릿을 만들기 전에 프로젝트를 저장하면 쓰기 권한 오류가 반환됩니다.

### 3.1.0 (2017.1.0)

*(릴리스: 2017년 6월 20일)*

**추가됨:**

* &lbrack;Plugin&rbrack; 새 Substance Source 플러그인(쉘프에 에셋 다운로드 허용)
* &lbrack;Shelf&rbrack; 4개의 새로운 글꼴(일본어 + 중국어 간체, 타자기, 세그먼트)
* &lbrack;Shelf&rbrack; 230개의 새로운 Alpha(패턴, 브러시 및 지문 스캔의 혼합)
* &lbrack;Shelf&rbrack; 50 New Procedurals(중세 및 현대 의류의 직물 패턴)
* &lbrack;Shelf&rbrack; 2개의 새로운 환경 지도(Mondarrain and Villa Nova Street)
* &lbrack;Shelf&rbrack; 9 새로운 필터 (MatFx 세부 정보 Edge Wear, 클램프, HBAO 등)
* &lbrack;Shelf&rbrack; 향상된 기본 파노라마 환경 맵
* &lbrack;Shelf&rbrack; 새로운 아놀드 5 내보내기 사전 설정
* &lbrack;스크립팅&rbrack; 셸프로 리소스 가져오기 허용

**알려진 문제:**

* &lbrack;내보내기&rbrack; 내보내기 사전 설정 편집이 매우 느립니다

## 버전 2

### 2.6.2

*(릴리스: 2017년 10월 20일)*

**추가됨:**

* &lbrack;텍스처 세트&rbrack; 비활성화된 텍스처 세트 삭제 허용
* &lbrack;Shelf&rbrack; 여러 사용자가 동일한 shelf 폴더에 쓸 수 있도록 허용
* &lbrack;스크립팅&rbrack; 플러그인 폴더를 다시 로드할 수 있음
* &lbrack;스크립팅&rbrack; 호환성을 보장하기 위해 플러그인 메타데이터에 필요한 최소 API 버전을 추가합니다
* &lbrack;IRay&rbrack; 이미지 내보내기 대화 상자 개선

**고정:**

* &lbrack;엔진&rbrack; 해상도 변경 시 획이 사라지는 문제(4K>2K)
* &lbrack;Bakers&rbrack; ID 맵 굽기가 이름별로 일치 사용 가능으로 실패함
* &lbrack;Bakers&rbrack; 오류 메시지가 충분히 명시적이지 않음
* &lbrack;3D 보기&rbrack; 탄젠트 공간이 베이커와 동기화되지 않음
* &lbrack;Tool&rbrack; 손가락 도구를 사용할 때 검은색 가공물
* &lbrack;Shader&rbrack; 비PBR 셰이더가 더 이상 작동하지 않습니다.
* &lbrack;Shader&rbrack; &quot;pbr-coated&quot;가 끊어짐
* &lbrack;Shader&rbrack; &quot;pbr-coated&quot; 셰이더의 코팅 거칠기는 더 이상 영향을 주지 않습니다
* &lbrack;Shader&rbrack; Spec gloss 셰이더가 Iray 및 SD와 일치하지 않습니다.
* 이름은 같지만 확장명이 다른 두 파일을 로드할 때 &lbrack;Shelf&rbrack; 충돌
* &lbrack;Shelf&rbrack; 선반에서 더 이상 사전 설정을 편집할 수 없음
* &lbrack;Shelf&rbrack; 셸프에 가져온 자산에 대한 사용자 정의 미리 보기를 설정할 수 없음
* 캐시에서 로드된 리소스는 사용을 잃게 됩니다.
* 템플릿을 만들기 전에 프로젝트를 저장하면 쓰기 권한 오류가 반환됩니다.
* 파일 이름에 마침표가 두 개 포함된 경우 잘못된 프로젝트 저장
* 여러 개의 점(.)이 있는 파일 가져오기 파일 이름에 문제가 있음

### 2.6.1

*(릴리스: 2017년 5월 12일)*

**추가됨:**

* &lbrack;TextureSet&rbrack; 메시 재질을 아무 것도 재할당하지 않음

**고정:**

* 베이킹된 맵을 교체한 후 TextureSet를 전환할 때 충돌 발생
* 레이어의 혼합 모드를 변경한 후 &quot;실행 취소 및 재실행&quot;을 수행할 때 충돌 발생
* big ID 맵에서 &quot;색상 선택&quot; 효과를 사용할 때 충돌 또는 고정
* 내보내기 창에서 이름이 변경된 &lbrack; 내보내기&rbrack; 텍스처 세트가 알파벳순으로 정렬되지 않음
* &lbrack;TextureSet&rbrack; 기본 이름으로 재설정 시 유니크성이 확인되지 않습니다.
* 프로젝트를 다시 열면 &lbrack;TextureSet&rbrack; 이름이 바뀐 텍스처 세트가 비활성화됩니다.
* &lbrack;Shelf&rbrack; 기본 템플릿 내용 누락
* &lbrack;Shelf&rbrack; 정사각형이 아닌 텍스처는 정사각형으로 표시됩니다.
* &lbrack;Shader&rbrack; 텍스처 세트가 비활성화되면 연관된 셰이더가 제거됩니다
* &lbrack;Scripting&rbrack; alg.baking.setTextureSetBakingParameters()가 더 이상 작동하지 않음
* &lbrack;Scripting&rbrack; Typo in websocket 튜토리얼
* &lbrack;Scripting&rbrack; AlgWidgets의 다양한 문제
* &lbrack;Log&rbrack; 경우에 따라 사용 가능한 가상 메모리를 잘못 감지합니다.

### 2.6.0

*(릴리스: 2017년 4월 27일)*

**추가됨:**

* 새 샘플 프로젝트 &quot;Meet Mat&quot; 추가
* &lbrack;Plugin&rbrack; 새로운 &quot;Resources Updater&quot; 플러그인
* &lbrack;TextureSet&rbrack; 텍스처 세트의 이름을 바꾸고 설명을 추가할 수 있도록 허용
* &lbrack;TextureSet&rbrack; 재료 재할당 허용
* &lbrack;TextureSet&rbrack; 텍스처 세트 목록 창에 설정 버튼 추가
* &lbrack;TextureSet&rbrack; 목록 맨 아래에 &quot;사용 안 함&quot; 텍스처 세트 표시
* &lbrack;Substance&rbrack; 현재 텍스처 집합 해상도에서 추가 맵을 사용하여 성능 향상
* &lbrack;Scripting&rbrack; 프로젝트에 사용되는 리소스(재료, 생성기 등)를 업데이트할 수 있습니다.
* &lbrack;스크립팅&rbrack; 쉘프를 추가/제거하는 방법 추가
* &lbrack;스크립팅&rbrack; 프로젝트의 자원에서 정보 쿼리 허용
* &lbrack;스크립팅&rbrack; 사용 가능한 셸 목록 검색 허용
* &lbrack;스크립팅&rbrack; AlgWidget 축소판 자습서 개선
* &lbrack;내보내기&rbrack; 파일 형식 지원에 따라 비트 심도 비활성화/활성화
* &lbrack;Log&rbrack; 콘솔에서 인쇄할 플러그인 이름 추가
* &lbrack;Log&rbrack; 숨겨진 텍스처 세트에 대한 제거 오류
* 샘플에 대한 새 아이콘 및 텍스트로 &quot;시작 화면&quot; 업데이트

**고정:**

* 특정 프로젝트에서 메시를 업데이트할 때 충돌 발생
* &lbrack;뷰포트(&rBrack; 대칭 평면 내부 색상이 더 이상 표시되지 않음
* &lbrack;Viewport&rbrack; 단독 보기를 사용할 때 일부 후처리 효과가 활성화됩니다.
* &lbrack;Shaders&rbrack; &quot;over_premult&quot; 혼합이 제대로 작동하지 않음
* &lbrack;Shaders&rbrack; 기본 셰이더를 사용하는 알파 테스트에 대한 경고
* &lbrack;Shelf&rbrack; Substance에서 태그 구문 분석이 잘못됨
* &lbrack;Shelf&rbrack; MatFX 녹 풍화 기능이 제대로 작동하지 않음
* &lbrack;Shelf&rbrack; HSL 필터는 기본적으로 잘못된 채널에서 활성화됩니다.
* &lbrack;Shelf&rbrack; Sharpen은 기본적으로 Height/표준 채널에서 활성화됩니다.
* &lbrack;Export&rbrack; Vray 내보내기 사전 설정이 OpenGL 노멀 맵을 사용하지 않음
* &lbrack;Tool&rbrack; 복제/손가락 도구의 부정확성 문제 가공물 만들기

### 2.5.3

*(릴리스: 2017년 3월 15일)*

**고정:**

* 특정 메쉬로 굽는 경우 &lbrack;Baker&rbrack; 충돌

**알려진 문제:**

* &lbrack;Mac&rbrack; 파티클이 텍스처 손상을 일으킬 수 있습니다

### 2.5.2

*(릴리스: 2017년 3월 14일)*

**고정:**

* &lbrack;도구&rbrack; Wacom 태블릿이 Linux에서 작동하지 않음
* &lbrack;Tool&rbrack; 손가락 도구를 사용할 때 검은색 가공물
* &lbrack;Bakers&rbrack; 케이지에 [이름별 일치]를 사용하는 경우 베이킹 실패
* 노멀 맵 전용으로 베이킹 시 &lbrack;Bakers&rbrack; 앰비언트 오클루전이 끊김
* &lbrack;Shelf&rbrack; 일반 필터가 알파를 제대로 처리하지 않습니다(대비/광도, 하이패스 등).
* &lbrack;뷰포트&rbrack; 그림자가 활성화된 프로젝트를 로드할 때 성능 문제
* macOS의 3D 보기에서 &lbrack;뷰포트&rbrack; 디더링 문제
* 색상 프로필을 활성화하면 &lbrack;뷰포트&rbrack; 입자 미리 보기가 잘못 표시됨
* Iray를 초기화하지 못한 경우 프로젝트를 다시 OpenGL로 전환할 때 &lbrack;Iray&rbrack; 충돌
* &lbrack;IRay&rbrack; 광택도는 SpecGloss 셰이더/mdl 렌더링 시 무시됩니다.
* &lbrack;Shader&rbrack; Spec/Gloss 셰이더가 Iray 및 SD와 일치하지 않습니다.
* &lbrack;Shader&rbrack; sRGB 변환이 linear to sRGB LUT 변환과 다름
* &lbrack;Shader&rbrack; 오래된 셰이더가 있는 프로젝트를 로드할 때 렌더링이 잘못됨
* &lbrack;Shader&rbrack; &quot;pbr-coated&quot; 셰이더가 더 이상 작동하지 않습니다
* &lbrack;내보내기&rbrack; 일부 채널은 텍스처 세트에 없는 경우에도 계속 내보내집니다.
* &lbrack;Layers&rbrack; 혼합 모드 &quot;노멀 맵 역디테일&quot;이 회색 음영 채널에서 작동하지 않습니다
* &lbrack;UI&rbrack; HDPI 모니터 및 디스플레이 확대/축소 시 &quot;색상 선택 창&quot;에 대한 문제

**알려진 문제:**

* &lbrack;Mac&rbrack; 파티클이 텍스처 손상을 일으킬 수 있습니다

### 2.5.1

*(릴리스: 2017년 2월 27일)*

**고정:**

* &lbrack;Mac&rbrack; Wacom 태블릿 입력이 3D 및 2D 보기에서 깨짐
* &lbrack;Bakers&rbrack; 이름별 일치가 더 이상 작동하지 않음
* &lbrack;Bakers&rbrack; &quot;평균 표준&quot; 설정이 더 이상 작동하지 않음
* &lbrack;Iray&rbrack; 구워진 노멀 맵이 누락된 잘못된 렌더링
* &lbrack;Array&rbrack; 색상 프로필은 OpenGL 렌더러와는 다르게 작동합니다.
* &lbrack;Array&rbrack; 렌더링을 비트맵으로 내보내는 경우 색상 프로파일 교정이 포함되지 않음
* &lbrack;Substance&rbrack; 재질 필터가 더 이상 작동하지 않음
* &lbrack;도구(&amp;r); 획 불투명도가 브러시 사전 설정에 저장되지 않음
* &lbrack;도구(&rbrack; 복제 브러시 UV 정렬이 더 이상 작동하지 않음
* &lbrack;Export&rbrack; 변위 채널은 정수로 내보낼 때 0.5의 가운데에 있어야 합니다.
* &lbrack;Template&rbrack; 절대 경로는 템플릿에 저장됩니다.
* &lbrack;TextureSet&rbrack; 텍스처 제거 후 채널 채널이 유지됩니다

**알려진 문제:**

* &lbrack;Linux&rbrack; Wacom 태블릿 입력이 3D 및 2D 보기에서 작동하지 않음
* &lbrack;Mac&rbrack; 파티클이 텍스처 손상을 일으킬 수 있습니다
* &lbrack;Export&rbrack; 매우 드문 경우지만 검은색 사각형이 AMD GPU에 나타날 수 있습니다

### 2.5.0

*(릴리스: 2017년 2월 21일)*

**추가됨:**

* AMD Radeon Pro 및 AMD FirePro GPU에 대한 지원 추가
* &lbrack;도구(&amp;r); 획 불투명도 지원 추가
* &lbrack;도구&rbrack; 마지막 브러시 획을 계속할 수 있도록 하는 수정자를 추가합니다
* &lbrack;Pascal GPU를 지원하는 Illustrator&rbrack; 업데이트
* &lbrack;뷰포트(&amp;r); 색상 프로파일(LUT)에 대한 지원 추가
* &lbrack;Substance&rbrack; 새 프레임워크(SD6 엔진) 통합
* &lbrack;UI&rbrack; 파일 메뉴에서 &quot;최근 파일&quot; 크기 목록 늘리기
* &lbrack;Import&rbrack; substance에서 범주를 사용하여 가져오기 대화 상자에서 접두어를 채웁니다
* &lbrack;베이커&rbrack; 8K 텍스처 굽기 허용
* &lbrack;Bakers&rbrack; 정사각형이 아닌 해상도를 굽도록 허용
* &lbrack;Bakers&rbrack; 두꺼운 하이 폴리 메쉬를 굽을 때 메모리 소비 개선
* &lbrack;Shelf&rbrack; 선반(및 프로젝트)을 잠가 동시 편집을 금지하고 손상을 방지합니다.
* &lbrack;Shelf&rbrack; 필터링에 사용할 물질에서 범주 및 키워드 읽기
* &lbrack;Shelf&rbrack; 검색 쿼리 결과에서 리소스를 제외하도록 허용
* &lbrack;Shelf&rbrack; 축소판 시간 계산 개선
* &lbrack;Shelf&rbrack; 프로젝트에 사전 설정 포함 허용
* &lbrack;Shelf&rbrack; Shift를 사용하여 트리 보기를 빠르게 축소/확장할 수 있습니다.
* &lbrack;Shelf&rbrack; 에셋이 읽기 전용일 때 축소판 저장 허용(로컬 캐시)
* &lbrack;Shelf&rbrack; 새로운 콘텐츠 : 새로운 필터(변환,, tri-평면 등)
* &lbrack;Shelf&rbrack; 새로운 콘텐츠 : 새로운 LUT 프로필(필름 느와르, 빈티지 등의 클래식 및 예술적)
* &lbrack;Shelf&rbrack; 새로운 내용 : 사용자 정의 텍스트를 빠르게 생성하기 위한 10개의 새로운 글꼴 Substance
* &lbrack;Shelf&rbrack; 새 템플릿 : 유니티 5 및 언리얼 엔진 4
* &lbrack;Shelf&rbrack; 아티스트 친화적으로 개선된 HSL 필터
* &lbrack;Shader&rbrack; PBR 셰이더의 Specular level 채널에 대한 지원 추가
* &lbrack;Shader&rbrack; Alpha 테스트 셰이더의 디더링 지원 추가
* &lbrack;Shader&rbrack; PBR 셰이더의 시차 오클루전 매핑에 대한 지원 추가
* &lbrack;Shader&rbrack; 셰이더 매개 변수에 대한 사용자 정의 UI를 정의할 수 있습니다.
* &lbrack;MatLayering&rbrack; 재질 레이어 작업 과정을 위한 새 마스크 채널 만들기
* &lbrack;스크립팅&rbrack; SP 프로젝트에 메타데이터 쓰기 허용
* &lbrack;스크립팅&rbrack; 특정 내보내기 사전 설정으로 내보내기 허용
* &lbrack;Scripting&rbrack; 셰이더 매개 변수를 JSON으로 검색할 수 있도록 허용
* &lbrack;스크립팅&rbrack; WebSocket 연결 지원 추가
* &lbrack;Scripting&rbrack; 셰이더 인스턴스를 로드할 수 있는 가능성을 추가합니다
* &lbrack;스크립팅&rbrack; 새 프로젝트를 만들 가능성을 추가합니다.
* &lbrack;Scripting&rbrack; 프로젝트에 가져온 메시의 url을 검색할 수 있도록 허용합니다.
* &lbrack;스크립팅&rbrack; 정사각형이 아닌 베이킹 허용
* &lbrack;Scripting&rbrack; 스크립팅 API를 통해 데이터를 설정할 때 오류를 보고합니다.
* &lbrack;users&rbrack; Substance을 지정할 표준 맵 포맷-데이터 태그 추가

**고정:**

* 물질을 사용하여 색상을 선택할 때 충돌
* 비 RGBA32f 이미지를 환경 맵으로 로드할 때 충돌
* AMD GPU 페인팅과 관련된 충돌
* &lbrack;Mesh&rbrack; OBJ 가져오기에서 mtl 파일이 없는 재질을 인식하지 못합니다
* &lbrack;메시&rbrack; UDIM 텍스처 세트 이름 생성이 일부 메시에서 잘못될 수 있습니다.
* &lbrack;UI&rbrack; 뷰어의 실행 취소/다시 실행 버튼 스틸 포커스 설정 및 마우스 스크롤 중지
* &lbrack;UI&rbrack; 일부 레이블이 높은 DPI에서 잘못 잘립니다.
* &lbrack; 페인트 효과의 [레이어] (&amp;r) [대체] 모드가 [마스크]에서 잘못된 동작을 가지고 있음
* &lbrack; Layer&rbrack; 빼기 혼합 모드가 알파에 잘못된 동작을 가지고 있음
* &lbrack;Tool&rbrack; 브러시 크기가 UV 테두리에 페인팅할 때 2D 보기에서 커짐
* &lbrack;Tool&rbrack; 물린 직선이 높은 DPI에서 불규칙한 동작을 합니다.
* &lbrack;도구&rbrack; 스텐실 해상도가 잘못된 경우가 있습니다.
* &lbrack;Bakers&rbrack; &quot;테두리 상자를 기준으로&quot;가 &quot;해제&quot;이면 &quot;최대 폐색기 거리&quot; 값이 고정되어 있습니다.
* &lbrack;Shader&rbrack; 스택 및 자동 매개 변수 채널 정의가 일치하지 않습니다.
* &lbrack;3D 보기&rbrack; 프로젝트 설정에 따라 일반 채널의 표시가 일치하지 않습니다.
* &lbrack;Viewport&rbrack; 일부 노멀 맵은 고정된 값을 가지며 가공물로 나타납니다
* &lbrack;뷰 포트(&amp;r); 사후 효과는 기본적으로 항상 비활성화되어 있습니다.
* 표준 채널이 없는 경우 &lbrack;내보내기&rbrack; 표준 혼합 설정이 잘못됨
* &lbrack;Export&rbrack; 경우에 따라 AMD GPU에서 잘못된 텍스처 생성이 발생합니다.
* &lbrack;Export&rbrack; Shader 매개변수가 그룹 내에 있는 경우 제대로 내보내지지 않습니다
* &lbrack;내보내기&rbrack; 사용자 정의 셸프에서 내보내기 사전 설정을 편집하면 로그 오류가 출력됨
* &lbrack;Shelf&rbrack; 트리 보기 필터링이 폴더 이름과 정확하게 일치하지 않음
* &lbrack;Shelf&rbrack; 선반 사전 설정의 이름을 바꾸는 것은 읽기 어렵습니다.
* &lbrack;Shelf&rbrack; 셸프에 가져온 셰이더 리소스는 다시 실행 후 보존되지 않습니다.
* &lbrack;Shelf&rbrack; 내용 : 용접 도구 사전 설정이 누락됨
* &lbrack;Shelf&rbrack; 내용 : Tile Generator이 제대로 작동하지 않음
* &lbrack;Shelf&rbrack; 내용 : 고무 타이어 더티 스마트 재질의 잘못된 마스크 수정
* &lbrack;Shelf&rbrack; 콘텐츠 : 가죽 가방 자재에 잘못된 그룹 이름이 수정되었습니다.
* &lbrack;Iray&rbrack; Iray에서 메시 절반이 누락됨
* 리소스를 3D 보기 위로 드래그할 때 &lbrack;Linux&rbrack; 충돌
* &lbrack;Mac&rbrack; 환경 설정은 Sierra에서 실행할 때마다 재설정됩니다

**알려진 문제:**

* &lbrack;Export&rbrack; 매우 드문 경우지만 검은색 사각형이 AMD GPU에 나타날 수 있습니다
* &lbrack;Array&rbrack; 색상 프로필이 때때로 이상하게 작동할 수 있습니다.

### 2.4.1

*(릴리스: 2016년 10월 28일)*

**고정:**

* 템플릿을 사용하여 프로젝트를 만들 때 충돌
* 내보내기 중 내보내기 대화 상자를 닫을 때 충돌 발생
* &lbrack;Mac&rbrack; 프로젝트 저장 시 오류 발생(내보내기 사전 설정 저장 실패)
* &lbrack;Shelf&rbrack; 새 사전 설정을 생성하면 두 번 표시됩니다
* 관리자 권한이 없으면 &lbrack;Shelf&rbrack; 사전 설정을 읽기 전용 모드로 로드할 수 없습니다.

### 2.4.0

*(릴리스: 2016년 10월 27일)*

**추가됨:**

* &lbrack;Shelf&rbrack; 리소스(트리 보기, 필터 등)를 검색하는 새로운 인터페이스
* &lbrack;Shelf&rbrack; 검색을 사전 설정으로 저장 허용
* &lbrack;Shelf&rbrack; 사전 설정에서 새 창 만들기 허용
* &lbrack;Shelf&rbrack; 리소스 가져오기를 위한 새 인터페이스
* &lbrack;Shelf&rbrack; Documents 폴더에 기본 알고리즘 셸프를 복사하지 않음
* &lbrack;Shelf&rbrack; 새로운 입자 사전 설정 : 전기 회로, 전선, 로코코, 혈관 소형
* &lbrack;Shelf&rbrack; &quot;Rain&quot;과 같이 사용하기 쉬운 이전 입자 사전 설정을 개선했습니다.
* &lbrack;Shelf&rbrack; 리소스 컨텍스트 메뉴에 새로운 정보 추가
* &lbrack;Viewport&rbrack; 환경 맵을 로드할 때 성능 향상
* &lbrack;Viewport&rbrack; 2의 기능이 아닌 환경 맵 지원 추가

**고정:**

* 마스크를 제거할 때 충돌
* 사전 설정을 저장한 후 페인팅할 때 충돌
* 일부 GPU에서 환경 흐림 효과 사용 시 충돌
* 미니 쉘프를 사용하여 잘못된 리소스를 할당할 때 충돌
* &lbrack;Shelf&rbrack; Clean + Save 프로젝트의 리소스에 대한 태그 및 메타데이터 제거
* &lbrack;Shelf&rbrack; 사전 설정을 가져오면 쉘프에 해당 리소스가 표시됩니다.
* Height 채널에서 생성된 &lbrack;내보내기&rbrack; 노멀 맵의 강도가 낮습니다.
* &lbrack;메쉬에서 표준 내보내기&rbrack;이 최종 노멀 맵에 항상 있는 것은 아닙니다
* &lbrack;Export&rbrack; 투명도를 사용한 확장은 경우에 따라 투명도 없이 나타날 수 있습니다
* &lbrack;Scripting&rbrack; &quot;alg.plugin_root_directory&quot;는 잘린 네트워크 경로를 반환할 수 있습니다.
* 정사각형이 아닌 프로젝트를 다시 열 때 &lbrack;TextureSet&rbrack; 잠금 버튼이 활성화됨

### 2.3.1

*(릴리스: 2016년 10월 7일)*

**추가됨:**

* &lbrack;Plugin&rbrack;&lbrack;Photoshop&rbrack; 내보낼 재질/스택/채널을 지정할 수 있습니다.
* &lbrack;스크립팅&rbrack; 함수 이름에 불일치가 있습니다.

**고정:**

* 사용자 정의 내보내기 사전 설정에서 &lbrack;Export&rbrack; Alpha을 삭제할 수 있습니다.
* &lbrack;Export&rbrack; Alpha이 sRGB 채널에서 잘못된 감마 변환을 받습니다
* &lbrack;Export&rbrack; 정사각형이 아닌 문서는 사각형으로 내보냅니다.
* &lbrack;Export&rbrack; 누락된 추가 맵을 내보낼 수 없습니다.
* &lbrack;Array&rbrack; 일부 매개 변수(예: 방출 강도)에는 영향이 없습니다.
* 시작 시 NVIDIA Quadro K2200/GTX 750/760으로 &lbrack;NVIDIA&rbrack; 충돌
* &lbrack;AMD&rbrack; 축소판 및 미리 보기에 대한 잘못된 색상 세트
* &lbrack;AMD&rbrack;이 새 파일 및 파일 열기에서 멈추고 드라이버 오류가 발생함
* &lbrack;Log&rbrack; &quot;software-version&quot;이 로그 파일에 없습니다.

### 2.3.0

*(릴리스: 2016년 9월 15일)*

**추가됨:**

* &lbrack;Plugin&rbrack; 새로운 &quot;Photoshop으로 내보내기&quot; 플러그인(내보내기 완료 레이어 스택)
* &lbrack;내보내기&rbrack; 패딩의 너비(픽셀 또는 무한)를 지정할 수 있습니다.
* &lbrack;내보내기&rbrack; UV 외부의 배경 유형을 설정할 수 있도록 허용
* &lbrack;Shelf&rbrack; 10개 재질을 혼합하는 새로운 재질 레이어 셰이더
* &lbrack;Shelf&rbrack; Height/일반 채널로 세부 정보를 보는 새로운 클레이 셰이더
* &lbrack;Shelf&rbrack; 환경 입력이 포함된 새로운 구운 조명 필터
* &lbrack;Shelf&rbrack; 정사각형이 아닌 변형을 추가하도록 일부 마스크 생성기를 업데이트했습니다.
* &lbrack;뷰 포트(&amp;r); 솔로 모드에 합성된 노멀 맵(normal+Height+bake)를 추가합니다
* &lbrack;스크립팅&rbrack; 추가 맵 내보내기 허용
* &lbrack;Scripting&rbrack; 텍스처 세트당 사용 가능한 추가 맵을 쿼리하도록 허용
* &lbrack;스크립팅&rbrack; 채널 형식 검색 허용
* &lbrack;Scripting&rbrack; 베이킹 설명서에 예제를 추가합니다.
* &lbrack;스크립팅&rbrack; 레이어의 가시성 쿼리 허용
* &lbrack;스크립팅&rbrack; 레이어의 혼합 모드와 불투명도를 쿼리할 수 있도록 허용
* &lbrack;Scripting&rbrack; 변환된 지도(최종 노멀 맵, 혼합된 AO 등) 내보내기 허용
* &lbrack;Substance&rbrack; 사용자 정의 사용 읽기 및 연결
* &lbrack;단축키&rbrack; 솔로 모드를 뒤로 순환하도록 수정자 키(SHIFT)를 추가합니다.
* &lbrack;내보내기&rbrack; 알파를 비활성화하도록 기본 내보내기 사전 설정을 업데이트했음
* 이제 엔진을 사용할 수 있는 경우에만 &lbrack;UI&rbrack; 축소판이 계산됩니다.
* &lbrack;UI&rbrack; 축소판 그림을 계산할 때 언급 표시

**고정:**

* 오래된 프로젝트를 열 때 충돌
* 텍스처 채널 캐시가 손상된 충돌
* 재질 레이어 작업 과정에서 4개 이상의 재질을 혼합할 때 충돌
* 도구 모음이 숨겨진 경우 &lbrack;UI&rbrack; 도구 단축키가 작동하지 않음
* &lbrack;UI&rbrack; Iray 도구 모음은 보기 메뉴에서 &quot;제목 없음&quot;이라는 레이블이 지정됩니다.
* &lbrack;UI&rbrack; 플러그인 도구 모음은 보기 메뉴에서 &quot;기울어지지 않음&quot;이라는 이름이 지정됩니다.
* &lbrack;Baker&rbrack; 베이크 설정을 편집하는 동안 Enter 키를 누르면 베이크 프로세스가 실행됩니다.
* &lbrack;Baker&rbrack; 일부 매개변수에 대한 범위가 잘못되었습니다.
* &lbrack;Import&rbrack; 숫자가 매우 커서 OBJ 메시를 가져올 수 없습니다.
* &lbrack;Import&rbrack; 일부 OBJ 파일을 너무 많은 하위 개체와 함께 가져옵니다
* 내보내기 시 &lbrack;Export&rbrack; 채널 배경이 기본 색상 대신 검은색으로 채워짐
* FOV가 너무 낮으면 &lbrack;Tool&rbrack; 파티클이 제대로 작동하지 않습니다.
* 하위 스택에 마스크가 있는 경우 &lbrack;Tool&rbrack; 브러시 미리 보기 색상이 올바르지 않습니다.
* &lbrack;Viewport&rbrack; 브러시가 2D 보기의 빈 영역으로 들어가면 거대해집니다
* &lbrack;뷰포트&rbrack; 일반 텍스처 페인팅 시 빈 브러시 미리보기
* &lbrack;Scripting&rbrack; 잘못된 설명서 : &#39;ambientocclusion&#39; 대신 &#39;ao&#39;가 나열됨
* &lbrack;스크립팅&rbrack; Painter을 닫을 때 subprocess()로 시작된 프로세스가 종료됨
* &lbrack;Shelf&rbrack; 구워진 조명 필터가 잘못된 AO 입력을 사용함
* &lbrack;MacOS&rbrack; 제거된 소화전 프로젝트(호환되지 않음)
* \*.spp 대신 \*.spt 파일을 로드할 때 기본 프로젝트가 열립니다.

**알려진 문제:**

* &lbrack;Plugin&rbrack; Photoshop 때문에 Height 및 일반 채널을 그대로 변환할 수 없습니다

### 2.2.0

*(릴리스: 2016년 7월 22일)*

**추가됨:**

* &lbrack;Shelf&rbrack; 검색 시스템 및 쿼리 개선
* &lbrack;Shelf&rbrack; 미니 쉘프를 위한 검색 필드 추가
* &lbrack;Shader&rbrack; 슬라이더에 대한 단계 정밀도를 정의할 수 있습니다.
* &lbrack;Shader&rbrack; 셰이더 매개 변수에 대한 실행 취소/다시 실행 버튼 추가
* &lbrack;Shader&rbrack; 셰이더를 다시 로드하면 해당 매개 변수가 재설정되지 않습니다.
* &lbrack;MatLayering&rbrack; 동적 재질 레이어 및 하위 스택에 대한 지원 추가
* &lbrack;MatLayering&rbrack; 셰이더 설정을 위한 json 파일 가져오기 허용
* &lbrack;MatLayering&rbrack; 텍스처 샘플러 제한 잠금 해제(쌍없는 텍스처로 전환)
* &lbrack;스크립팅&rbrack; 베이커 설정을 설정하고 계산을 시작할 수 있도록 허용합니다.
* &lbrack;Substance&rbrack; 식별자 외에 입력/출력 연결에 &quot;사용&quot;을 사용합니다.
* &lbrack;도구(&amp;r); 투영 도구에 대한 뷰포트에서 미리 보기 채널을 선택할 수 있도록 허용

**고정:**

* 시작 중 물질이 잘못된 폴더에 있는 경우 충돌
* 잘못된 로그 파일로 인해 충돌 보고서가 작동하지 않는 경우가 있습니다
* &lbrack;Iray&rbrack; 포스트 효과가 Iray가 일시 중지되었을 때 새로 고쳐지지 않음
* &lbrack;Array&rbrack; 자동 초점 단축키가 더 이상 작동하지 않습니다.
* &lbrack;Iray&rbrack; 조리개 슬라이더 동작이 에셋 크기에 따라 변경됩니다.
* &lbrack;Layers&rbrack; 첫 번째 질감 채널이 모두 비활성화되어 있으면 기본적으로 활성화되지 않습니다.
* &lbrack;Shader&rbrack; &quot;param auto&quot;가 올바르지 않으면 오류가 인쇄되지 않습니다.

**알려진 문제:**

* &lbrack;Mac&rbrack; 텍스처 샘플 제한이 16에서 잠겨 있습니다(GPU 드라이버 문제).

### 2.1.1

*(릴리스: 2016년 7월 1일)*

**추가됨:**

* &lbrack;License&rbrack; 라이선스 파일 위치를 변경할 수 있습니다.
* &lbrack;뷰포트(&amp;r); &quot;B&quot; 단축키를 추가하여 추가 맵 간에 순환
* &lbrack;Import&rbrack; FBX 2016/2017을 올바로 가져올 수 있음
* &lbrack;빠른 마스크(&amp;r); 도구를 사용할 때 검사기 제거
* &lbrack;Array&rbrack; 장면 치수 정보 추가
* &lbrack;Iray&rbrack; 최대 샘플 수 및 렌더링 시간을 늘릴 수 있음
* &lbrack;UI&rbrack; 슬라이더에서 +/- 버튼을 사용할 때 즉시 결과 업데이트
* &lbrack;UI&rbrack; 회색 음영 슬라이더에 대한 정확도 향상 허용
* &lbrack;내보내기&rbrack; RGB 전용 텍스처에 대한 알파 채널을 내보내지 않음
* &lbrack;내보내기&rbrack; Dota 2 내보내기 사전 설정 업데이트
* &lbrack;Shelf&rbrack; 새로운 &quot;육각형 타일&quot; 패턴
* &lbrack;Shelf&rbrack; 새로운 &quot;용접&quot; 도구
* &lbrack;Shelf&rbrack; 방향 컨트롤을 제공하는 마무리 필터 업데이트

**고정:**

* &lbrack;Export&rbrack; PSD 파일을 8비트로 내보낼 수 없습니다.
* &lbrack;Export&rbrack; 8K 내보내기는 일부 하드웨어 구성에서 사용할 수 없습니다.
* &lbrack;내보내기&rbrack; Sketchfab 창이 잘림
* &lbrack;Export&rbrack; [사양/광택] 내보내기 사전 설정의 거칠기 맵이 잘못되었습니다.
* &lbrack;UI&rbrack; 회색 음영 슬라이더에서 입력 기능이 더 이상 작동하지 않음
* &lbrack;UI&rbrack; Substance 입력에 필터를 입력할 수 없음(예: 생성기)
* &lbrack;UI&rbrack; 일부 슬라이더에 홀수 동작이 있음
* &lbrack;UI&rbrack; DeltaTime +/- 파티클 단계가 너무 큽니다.
* &lbrack;Iray&rbrack; 일부 프로젝트는 Iray로 전환할 때 애플리케이션을 차단합니다.
* 하드웨어 감지 시 &lbrack;Array&rbrack; 충돌
* 마스크 모드에서 &lbrack;도구(&amp;r); 브러시 미리 보기 색상이 올바르지 않음
* &lbrack;Tool&rbrack; 재료 선택기는 호환되지 않는 도구와 함께 사용할 수 있습니다.
* &lbrack;Tool&rbrack; 투영 미리 보기가 사양/광택 워크플로우에 따라 확산으로 전환되지 않음
* &lbrack;Shelf&rbrack; 기본 셰이더를 변경하면 스마트 매트/스마트 마스크 미리 보기가 깨집니다.
* &lbrack;Shelf&rbrack; 일부 스마트 재질의 이름이 잘못됨
* &lbrack;Shelf&rbrack; 추가 알파 모양이 손상되어 로드되지 않음
* &lbrack;뷰포트(&rbrack; &quot;추가 맵&quot; 모드로 전환하면 &quot;기타&quot;가 먼저 표시됩니다.
* 추가 지도가 없으면 &lbrack;Viewport&rbrack; 뷰포트가 다시 &quot;기타&quot;로 전환
* &lbrack;충돌&rbrack;&lbrack;리눅스&rbrack; 충돌 보고서가 우분투(Steam)에서 작동하지 않음
* &lbrack;충돌&rbrack;&lbrack;리눅스&rbrack; 웹 URL 링크가 우분투(Steam)에서 작동하지 않음
* &lbrack;충돌&rbrack;&lbrack;Windows&rbrack; Substance 페인터가 더 이상 실행되지 않을 때 &quot;crashwatcher&quot;를 제거합니다.
* &lbrack;충돌&rbrack;&lbrack;Mac&rbrack; 충돌 보고서 시스템이 제대로 작동하지 않습니다
* &lbrack;충돌&rbrack; 이미 메시를 가져오는 동안 메시를 가져오면 충돌이 됩니다.
* 텍스처 세트 선택 단축키가 다시 시작 후 0으로 재설정됨

### 2.1.0

*(릴리스: 2016년 6월 2일)*

**추가됨:**

* &lbrack;UDIM&rbrack; 메시에서 UDIM 타일을 텍스처 세트로 가져오기
* &lbrack;Linux&rbrack; CentOS 6.6 및 Ubuntu 12.4에 대한 추가 지원
* &lbrack;내보내기&rbrack; 8K 해상도 추가(시험적)
* &lbrack;내보내기&rbrack; 내보내기 중 비트 심도 선택 허용
* &lbrack;Baker&rbrack; 한 번에 여러 텍스처 세트를 굽도록 허용
* 고해상도 모니터 지원(높은 DPI 비율)
* &lbrack;Scripting&rbrack; 내보낼 때 사용자 정의 텍스처 및 패딩을 설정합니다.
* &lbrack;Viewport&rbrack; 메시를 클릭하여 설정한 텍스처 간에 전환할 수 있음(Ctrl+Alt+클릭)
* &lbrack;Viewport&rbrack; 마우스 휠로 확대/축소하면 마우스 커서가 있는 위치로 이동합니다
* &lbrack;UI&rbrack; 기본 배경색 및 환경 맵 표시 업데이트
* &lbrack;UI&rbrack; 사용자 채널에 대한 원래 이름의 도구 설명 추가
* &lbrack;UI&rbrack; 이름을 바꿀 수 없는 채널의 배경색 변경
* &lbrack;빠른 마스크(&amp;r); 도구를 사용할 때 검사기 제거
* &lbrack;Shader&rbrack; 셰이더 매개 변수 및 재질/마스크에 대한 그룹을 정의할 수 있습니다.
* &lbrack;엔진&rbrack; 스몰 사이즈 스탬핑의 최적화
* &lbrack;Stencil&rbrack; 마스크를 일시적으로 전환하려면 &quot;W&quot;를 단축키로 추가
* &lbrack;Shelf&rbrack; 검색 필드를 지우기 위한 십자 버튼을 추가합니다.
* &lbrack;Shelf&rbrack; 한 번의 클릭으로 Alpha 불러오기
* &lbrack;Shelf&rbrack; 새로운 내보내기 사전 설정 : Vray UDIM, Arnold UDIM, Spec/Gloss from Metal/Rough
* &lbrack;Shelf&rbrack; 새로운 알파 : 기하학적 모양, 혈관 및 기호
* Substance Painter 실행 파일의 속성에 이름 및 버전 추가

**고정:**

* &lbrack;Substance&rbrack; 일반 채널과 추가 맵을 동시에 사용할 수 없습니다.
* &lbrack;Array&rbrack; MDL 굴절 및 흡수 설정이 작동하지 않음
* &lbrack;Array&rbrack; 원래 장면 배율이 유지되지 않음
* &lbrack;Shelf&rbrack; Specular/광택도 템플릿에서 잘못된 셰이더를 사용합니다.
* &lbrack;Export&rbrack; 기본 내보내기 사전 설정이 일부 맵을 내보내지 않음(예: AO)
* &lbrack;뷰포트&rbrack; 2D 보기의 UV 바깥쪽을 클릭할 때 피벗 포인트가 업데이트되지 않음
* &lbrack;UI&rbrack; 슬라이더 값이 반올림됨
* &lbrack;UI&rbrack; 슬라이더 값을 편집할 때 사용 가능한 공간이 매우 작은 경우가 있습니다
* &lbrack;새 프로젝트&rbrack; 템플릿 드롭다운 목록이 1.x에서 2.x로 올바르게 업데이트되지 않음
* &lbrack;스크립팅&rbrack; 사용자 정의 버튼에서 &quot;호버&quot; 비헤이비어 수정
* &lbrack;Mac&rbrack; 빈 프로젝트에서 실행을 취소하면 카메라가 잠깁니다.

**알려진 문제:**

* 충돌 보고서를 Ubuntu에서 사용할 수 없음
* 일부 URL 버튼이 작동하지 않을 수 있습니다. 해결 방법은 FAQ를 살펴보십시오

### 2.0.5

*(릴리스: 2016년 4월 29일)*

**추가됨:**

* &lbrack;Shelf&rbrack; 비pbr 템플릿, 셰이더 및 내보내기 사전 설정 추가/업데이트
* &lbrack;Shelf&rbrack; 앰비언트 오클루전을 포함하도록 UE4 내보내기 사전 설정 업데이트됨

**고정:**

* 리소스가 손상된 일부 프로젝트를 열고 저장할 때 충돌
* &lbrack;Viewport&rbrack; 와이어프레임이 2D 보기에서 손상된 것으로 나타남
* &lbrack;Shelf&rbrack; 일부 스튜디오 환경 지도의 개선된 성능
* &lbrack;Shelf&rbrack; 일부 스튜디오 환경 맵이 복제됩니다.
* &lbrack;Shelf&rbrack; &quot;Baked Lighting Material&quot;이 없음
* &lbrack;Shelf&rbrack; &quot;회색 음영 변환&quot; 생성기가 없음

### 2.0.4

*(릴리스: 2016년 4월 26일)*

**추가됨:**

* 메시 충돌 개선 및 와이어프레임 렌더링 최적화
* 대형 프로젝트를 통해 성능 및 메모리 관리 향상
* 슬라이더 정밀도 및 단계 개선
* &lbrack;UI&rbrack; 값을 입력할 때가 아니라 슬라이더의 유효성을 검사할 때만 엔진을 업데이트합니다.
* &lbrack;UI&rbrack; 기본 도구 모음의 전용 단추로 Iray 전환 이동(및 단축키 변경)
* &lbrack;도구(&amp;r); 복제 도구 소스 위치 동작에 대한 설정 추가
* &lbrack;Shader&rbrack; 사용자 정의 셰이더에서 메시 꼭지점 색상을 읽을 수 있도록 허용
* &lbrack;스크립팅&rbrack; 텍스처 세트, 채널 및 레이어 목록 검색 허용
* &lbrack;스크립팅&rbrack; 도우미 함수 추가(경로 url, 프로젝트에서 내보내기 경로 가져오기)
* &lbrack;Mac&rbrack; 로그 파일에서 Mac Os &quot;El Capitan&quot; 버전 감지

**고정:**

* Substance share으로 두 번째 내보내기 후 충돌
* 충돌 데이터가 있는 텍스처 세트 간에 레이어를 복사할 때 빠른 마스크
* 일부 프로젝트에는 메모리를 많이 소비하는 매우 긴 업데이터가 있습니다
* 복제/손가락 도구로 입자 사전 설정을 선택할 때 &lbrack;도구(&amp;r); 충돌
* &lbrack;Baker&rbrack; FBX 파일을 로드하면 무거운 메시에 너무 많은 시간이 소요됩니다.
* &amp;lbrack viewport&rbrack;일부 컴퓨터의 늘리다 환경 맵
* &lbrack;Viewport&rbrack; 브러시 알파의 감마 변환이 잘못되었습니다.
* &lbrack;Export&rbrack; Alpha은 Tiff 파일이 있는 별도의 채널 대신 투명도로 저장됩니다.
* &lbrack;내보내기&rbrack; 표준 채널은 항상 OpenGL로 내보내집니다.
* &lbrack;Iray&rbrack; Iray 설정에 대한 슬라이더 이름이 없습니다.
* &lbrack;Rray&rbrack; 렌더링이 Retina/높은 DPI에서 잘못된 해상도로 수행됩니다.
* Iray 모드에서 인터페이스 크기를 조정할 때 &lbrack;Iray&rbrack; 충돌
* &lbrack;Iray&rbrack; 낮은 해상도로 렌더링할 때 성능 저하가 매우 큽니다.
* &lbrack;Iray&rbrack; 일시 중지가 작동하지 않음(Iray는 백그라운드에서 계산)
* 표준 채널에는 때때로 검은 사각형 아티팩트가 있습니다
* 회색 음영 필터를 사용해 표준 채널이 반전됨
* 스택에 알파가 일부 있으면 표준 채널이 제대로 혼합되지 않습니다
* 프로젝트가 아직 저장되지 않았더라도 프로젝트를 열 때 디스크에서 편집됨
* 일부 프로젝트에서 메시를 다시 가져오면 GPU 성능이 매우 저하됩니다
* 메시를 터치하지 않으면 브러시 방향이 잘못됨
* 시작 화면에 substance share 로고가 없습니다.

### 2.0.2

*(릴리스: 2016년 3월 25일)*

**추가됨:**

* &lbrack;Iray&rbrack; Iray와 호환되도록 사양/광택 템플릿 및 셰이더를 업데이트합니다.
* &lbrack;Export&rbrack; 스크린샷을 ArtStation으로 내보낼 수 있음
* &lbrack;Scripting&rbrack; 플러그인 디렉토리에서 실행 지원
* &lbrack;스크립팅&rbrack; &quot;다른 이름으로 저장&quot; 허용
* &lbrack;UI&rbrack; 슬라이더를 두 번 클릭하여 해당 값을 편집할 수 있도록 허용
* 벨라 샘플을 Substance share으로 이동
* 새 샘플 프로젝트 : 구 미리 보기
* 셸 확장 충돌에 대해 사용자에게 경고

**고정:**

* 설치 관리자가 Substance Painter 1.x 설치를 재정의
* &lbrack;UI&rbrack; 채널 목록 레이아웃이 필터로 중단됨
* &lbrack;UI&rbrack; 셰이더 매개 변수가 표시되지 않음
* &lbrack;UI&rbrack; 레이어 창 크기를 조정하면 콘텐츠가 잘못 자릅니다
* &lbrack;도구&rbrack; 불투명도 채널이 항상 올바르게 사용되는 것은 아닙니다.
* &lbrack;도구(&amp;r); 손가락/복제가 대칭에서 작동하지 않음
* 일부 채널에서 &lbrack;도구(&amp;r); 브러시 미리 보기 불투명도가 올바르지 않음
* 아직 생성되지 않은 상태에서 Iray를 사용할 때 &lbrack;Iray&rbrack; 충돌
* &lbrack;Array&rbrack; 프로젝트에서 Ray 설정 데이터를 로드할 수 없음
* &lbrack;Iray&rbrack; Iray는 일시 중지된 후 설정 수정을 처리하지 않습니다.
* &lbrack;Shelf&rbrack; 선반으로의 재료 가져오기가 작동하지 않습니다.
* 스텐실이 표준 채널에서 작동하지 않음
* 일부 프로젝트에서 페인팅할 때 충돌
* 일부 프로젝트에서 입자를 사용하여 페인팅할 때 충돌
* 일부 계산 중 픽셀 프로세서 충돌

### 2.0.0

*(릴리스: 2016년 3월 16일)*

**추가됨:**

* 기본 도구 모음에서 Substance 저장소로 단축키
* 렌더러를 보기 모드 및 스크린샷 내보내기로 내보내기
* &quot;스마트 마스크&quot; 생성 및 사용 지원
* Specular/용어집 PBR 워크플로우 지원(새로운 확산 채널 포함)
* Substance 체인(Substance 이미지 입력에 물질 연결)
* 사용자 정의 플러그인을 사용한 스크립팅 지원
* Sobel 필터를 사용하여 Height을 표준으로 변환 개선
* 스텐실/투영 미리 보기 해상도를 2K로 전환
* 새 프로젝트에 대해 기본적으로 일반 채널 추가
* 출력 노드에서 사용자 데이터 태그를 읽고 기본적으로 Substance의 채널을 활성화/비활성화합니다.
* TextureSet 설정에서 일반/AO 혼합 표시
* &lbrack;도구(&amp;r); 색상 혼합 및 확산을 위한 새로운 손가락 도구
* &lbrack;도구(&amp;r); 텍스처의 일부를 복사하기 위한 새로운 복제 도구
* &lbrack;도구(&amp;r); 손가락, 복제 및 지우개 도구에 대한 채널 선택 허용
* &lbrack;Layer&rbrack; 채우기 효과 이름에 Substance 이름 추가
* &lbrack;레이어&rbrack; 마스크를 클립보드로 내보내기 허용
* &lbrack;뷰포트&rbrack; 원근감 및 직교 모드 간 전환
* &lbrack;뷰 포트(&amp;r); 원근감 모드에서 시야 제어를 허용합니다.
* &lbrack;뷰포트(&amp;r); Ctrl+마우스 가운데 버튼을 클릭하여 필드 거리의 깊이 설정 허용
* &lbrack;뷰포트&rbrack; 3D 보기에 환경 맵을 드래그하여 놓을 수 있습니다.
* &lbrack;Viewport&rbrack; 엔진이 강력한 계산을 수행할 때 향상된 피드백
* &lbrack;Export&rbrack; json 파일의 셰이더 매개 변수 내보내기를 허용합니다.
* &lbrack;UI&rbrack; 새 아이콘, 색상 및 레이아웃으로 인터페이스 업데이트
* &lbrack;UI&rbrack; 미니 쉘프에 에셋 이름 추가
* &lbrack;UI&rbrack; 기본적으로 &quot;채널 매핑&quot; 축소
* &lbrack;Shader&rbrack; 셰이더 텍스처 매개변수에 대한 사용자 정의 색상을 선택합니다.
* 리소스를 끌어서 놓을 때 파일을 가져올 위치를 묻는 &lbrack;Shelf&rbrack;
* &lbrack;Shelf&rbrack; 스마트 재질 및 생성기를 위한 새로운 미리 보기 구
* &lbrack;Shelf&rbrack; Specular 광택도 셰이더 추가
* &lbrack;Shelf&rbrack; 새로운 단단한 표면 모양
* &lbrack;Shelf&rbrack; 새 Alpha 텍스처 및 모양
* &lbrack;Shelf&rbrack; 새 스킨 텍스처
* &lbrack;Shelf&rbrack; 새로운 스캔 기반 재료 및 스마트 재료
* &lbrack;Shelf&rbrack; 기존 스마트 재질의 새로운 글꼴과 사양/광택 지원
* &lbrack;Shelf&rbrack; 금속 표면 시뮬레이션을 위한 새로운 마무리 필터
* &lbrack;Shelf&rbrack; 새로운 강력한 마스크 생성기 &quot;마스크 편집기&quot;
* &lbrack;Shelf&rbrack; 재작업 및 청소된 오래된 재료
* 새로운 &quot;Vela&quot; 샘플 프로젝트

**고정:**

* &lbrack;Settings&rbrack; 카메라 회전 및 확대/축소 속도는 프로젝트에 의해 재정의됩니다
* &lbrack;뷰 포트(&amp;r); 기본 일반 텍스처에서 정밀도 문제가 발생하면 반사가 잘못됩니다
* &lbrack;뷰포트&rbrack; 비네팅이 기본적으로 활성화됨
* &lbrack;Viewport&rbrack; 가공물은 환경 맵 테두리(Nvidia GPU)에 나타납니다
* &lbrack;Viewport&rbrack; 투영/스텐실 모드의 축소판이 로드하기에 매우 깁니다.
* &lbrack;Baker&rbrack; 32비트 대신 16비트 정수로 구운 텍스처 저장
* &lbrack;Layer&rbrack; 오래된 재질이 스택에 잘못 표시됨
* 일부 채널의 기본 색상 및 비트 깊이가 올바르지 않습니다(예: Specular, 광택도).
* 통과 모드에서 혼합을 비활성화하는 지우개 비헤이비어 수정

**알려진 문제:**

* 대칭이 손가락 및 복제 도구에서 작동하지 않음
* ArtStation 내보내기가 없습니다.

## 버전 1

### 1.7.3

*(릴리스: 2016년 3월 1일)*

**추가됨:**

* &lbrack;내보내기&rbrack; 패딩을 비활성화하는 옵션 추가
* &lbrack;Shelf&rbrack; 셸프 폴더 내의 하위 셸프 계층 구조 지원

**고정:**

* 이전 읽기 전용 파일을 저장할 때 충돌 발생
* 두 번째 프로젝트를 열 때 충돌
* 일부 축소판(선반, 레이어 또는 도구 설명)을 로드할 때 충돌
* &quot;메시에서 선 위치 유지&quot; 비활성화가 작동하지 않음
* &lbrack;내보내기&rbrack; 비트맵의 확대/축소는 가장 가까운 필터링으로 수행됩니다.
* &lbrack;Shelf&rbrack; 리소스 검색이 매우 느립니다.
* &lbrack;Shelf&rbrack; 흐림 효과 필터는 16비트와 호환되지 않음
* 이전 대칭 사전 설정을 로드하면 &lbrack;Tool&rbrack; 도구가 작동하지 않습니다
* Specular 채널의 색상 대화 상자에서 색상 공간 변환을 수행하지 않음

### 1.7.2

*(릴리스: 2016년 1월 13일)*

**추가됨:**

* &lbrack;Layers&rbrack; 채우기 레이어에 대한 기본 틸링 지정 허용

**고정:**

* &lbrack;Export&rbrack; Sketchfab 내보내기가 더 이상 작동하지 않음
* &lbrack;Layer&rbrack; 쌍선형 필터링은 변형 없이 채우기에도 적용됩니다.
* &lbrack;Tool&rbrack; 투영 모드에서 이미지 입력이 있는 Substance를 사용한 성능 저하
* &lbrack;도구(&amp;r); 재료 선택기가 망가졌습니다.

### 1.7.1

*(릴리스: 2015년 12월 18일)*

**고정:**

* 텍스처 세트를 전환할 때 충돌 발생
* 페인팅 시 속도가 느림

### 1.7.0

*(릴리스: 2015년 12월 17일)*

**추가됨:**

* &lbrack;성능&rbrack; 레이어 내용 및 해당 축소판을 동시에 계산
* &lbrack;내보내기&rbrack; 프로젝트 옆에 있을 때 내보내기 경로를 상대값으로 저장
* &lbrack;레이어&rbrack; 새 혼합 모드 추가됨 : 빼기 및 추가/하위
* &lbrack;Layers&rbrack; 칠 레이어에 대한 새로운 쌍선형 HQ 필터링
* &lbrack;Shader&rbrack; 기본 설정에서 축소판 생성을 위한 기본 셰이더를 설정합니다.
* &lbrack;Shader&rbrack; 텍스처 세트당 셰이더를 지정할 수 있습니다.
* &lbrack;Shader&rbrack; 셸프에서 텍스처 샘플링 허용
* &lbrack;도구&rbrack; 페인팅을 위한 새로운 &quot;줄 바꿈&quot; 브러시 비헤이비어
* &lbrack;도구&rbrack; 페인팅 중에 필터링 개선 및 앨리어싱 감소
* &lbrack;도구&rbrack; 향상된 하위 픽셀 페인팅 품질
* &lbrack;Tool&rbrack;에서 브러시 설정에 대한 &quot;기본&quot; 표시를 제거하고 프레임 열기/닫기 아이콘을 개선했습니다.
* &lbrack;메뉴&rbrack; 마우스 오른쪽 버튼 클릭 메뉴에 효과 아이콘 추가
* 프로젝트에서 템플릿 만들기
* &lbrack;Shelf&rbrack; 새 템플릿 : PBR, Dota 2
* &lbrack;Shelf&rbrack; 새 내보내기 사전 설정 : Dota 2
* &lbrack;Shelf&rbrack; 새로운 셰더 : Dota 2, PBR 자동차 페인트, PBR 코팅, PBR 벨벳
* &lbrack;Shelf&rbrack; 새로운 재질 : 스틸 녹 및 마모, 스타일화된 조명
* &lbrack;Shelf&rbrack; 새로운 필터 : 흐림 방향, 스타일화된 조명
* &lbrack;Shelf&rbrack; 새로운 브러시 : 더 나은 경도 제어를 위한 새로운 알파가 있는 기본 소프트 및 기본 하드
* &lbrack;Shelf&rbrack; 신규 생성기 : 3D 거리 및 조명
* &lbrack;Shelf&rbrack; 랩 투영 및 백페이스 컬링으로 업데이트된 브러시(기본적으로 활성화됨)
* &lbrack;Shelf&rbrack; 빠른 계산을 위해 흰색 노이즈를 픽셀 프로세서 버전으로 업데이트함

**고정:**

* &lbrack;시작 화면&rbrack; Tutorials 링크 이전 비디오로 보내기
* &lbrack;Channels&rbrack; 레이어 만들기를 AO로 채우기 위해 &quot;아니오&quot;라고 말하면 여전히 레이어가 만들어집니다
* &lbrack;채널&rbrack; UserX 채널 이름이 인터페이스에서 전파되지 않음
* 솔로 채널 목록에서 &lbrack;Viewport&rbrack; 마스크 항목이 비어 있습니다.
* &lbrack;Share&rbrack; 알파를 SP에서 공유로 내보내면 읽을 수 없는 .image 파일이 만들어집니다
* &lbrack;License&rbrack; ASCII 문자가 아닌 사용자 이름에 대한 활성화 수정
* 색상을 선택할 때 &lbrack;Shader&rbrack; Color 매개 변수 대화 상자가 사라짐
* &lbrack;Shelf&rbrack; 축소판 그림을 사용하지 않을 때 메모리에서 언로드되지 않음
* &lbrack;Shelf&rbrack; 고정 그레이디언트 필터
* &lbrack;대칭(&amp;r)가 스텐실/투영에서 작동하지 않음
* &lbrack;Tool&rbrack; 새 브러시 사전 설정을 만들 때 잘못된 이름
* 메시를 다시 가져오는 경우에도 획 보존 설정이 비활성화된 상태로 유지됩니다
* 큰 크기의 입자를 계산할 때 드라이버 초기화(TDR).

### 1.6.1

*(릴리스: 2015년 11월 9일)*

**고정:**

* 2D 보기가 표시되는 경우 프로젝트를 열 때 충돌
* 현재 선반이 없는 경우 새 내보내기 사전 설정을 만들 때 충돌 발생
* &lbrack;도구(&amp;r); 재료 피커 아이콘이 계속 표시될 수 있습니다.
* &lbrack;도구&rbrack; 재료 피커가 동시에 페인팅할 때 마우스 커서 숨기기
* &lbrack;Shelf&rbrack; 메타 데이터는 각 종료 후 디스크에 기록됩니다.

### 1.6.0

*(릴리스: 2015년 10월 29일)*

**추가됨:**

* Windows 10에 대한 공식 지원
* &lbrack;Substance&rbrack; 기본적으로 Substance 매개 변수 그룹 축소
* &lbrack;Substance&rbrack; 새 프레임워크 추가(픽셀 프로세서 성능 향상)
* &lbrack;Viewport&rbrack; 대칭 모드에서 대칭 평면 디스플레이를 비활성화할 수 있습니다.
* &lbrack;뷰포트(&amp;r); 그림자 렌더링 및 성능 향상
* &lbrack;뷰포트&rbrack; 페인팅 시 그림자 계산 일시 중지
* &lbrack;뷰포트(&amp;r); 와이어프레임 렌더링 성능 향상
* &lbrack;엔진&rbrack; Vram 메모리 관리를 개선하여 설치 공간 감소
* &lbrack;엔진&rbrack; 성능 향상을 위해 AMD GPU에서 텍스처 새로 고침 개선
* &lbrack;엔진&rbrack; 성능 향상을 위해 NVIDIA GPU에서 스레드 최적화 설정 비활성화
* &lbrack;효과&rbrack; &quot;패딩&quot; 이미지 입력을 요청하는 태그를 추가합니다.
* &lbrack;Layer&rbrack; 채우기 내 UV 오프셋/비율의 정밀도 증가
* &lbrack;Layer&rbrack; 채우기에서 비율 슬라이더를 기하급수적으로 설정
* &lbrack;Layer&rbrack; [재질]을 레이어 스택에서 직접 드래그하여 놓을 수 있습니다.
* &lbrack;레이어&rbrack; 레이어 스택에서 직접 필터 드래그 앤 드롭 허용
* &lbrack;Layer&rbrack; 마스크 브러시 색상을 새로 만든 마스크 색상으로 조정합니다.
* &lbrack;Shader&rbrack; 다중 텍스트 코드 노출
* &lbrack;Shader&rbrack; 사용자 정의 함수를 허용하는 감마/톤 매핑 함수 노출
* &lbrack;Bakers&rbrack; TriPlanar 사용에 대한 기본 위치 베이커 설정 변경
* &lbrack;Tool&rbrack; &quot;Geometry Decal&quot;의 이름을 &quot;Polygon Fill&quot;로 변경
* &lbrack;Shelf&rbrack; TriPlanar를 지원하는 생성기 업데이트 : MG Metal 가장자리 마모, MG 마스크 빌더, MG Fibre 유리, MG Dirt
* &lbrack;Shelf&rbrack; 새 설정으로 재질 업데이트 및 사용하지 않는 재질 제거
* &lbrack;Shelf&rbrack; 22개의 새로운 스마트 재질(플라스틱, 철, 패브릭, 스틸 등)
* &lbrack;Shelf&rbrack; 이음새를 방지하기 위해 패딩 이미지 입력으로 선명 효과, 흐림 및 뒤틀기 필터를 업데이트합니다.
* &lbrack;Shelf&rbrack; 더 쉽게 사용할 수 있도록 뒤틀기 설정 개선
* &lbrack;Shelf&rbrack; 2개의 새로운 프로시저 노이즈 : 3D Perlin 노이즈 및 3D Worley 노이즈

**고정:**

* Mac에서 전용 GPU에 대한 &lbrack; Engine&rbrack; Vram 양 탐지가 올바르지 않음
* &lbrack;엔진&rbrack; 텍스처가 뷰포트에서 더 어두운 버전으로 전환됨
* &lbrack;Engine&rbrack; 여러 레이어 아래로 페인팅할 때 성능이 저하됨
* 프로젝트를 열 때 계산되는 레이어와 캐시된 버전이 다른 &lbrack;Engine&rbrack;
* &lbrack;Substance&rbrack; Mac에서 4K의 잘못된 결과가 발생함
* &lbrack;Substance&rbrack; 매개 변수의 순서가 잘못되었습니다.
* &lbrack;Shader&rbrack; 툰 및 픽셀화된 셰이더는 완전히 검정색입니다.
* &lbrack;Shader&rbrack; 매개 변수가 env-map 변경 후 사라짐
* png 파일을 제네레이터 폴더에 넣을 때 &lbrack;Shelf&rbrack; 충돌
* &lbrack;Shelf&rbrack; 축소판은 낮은 거칠기로 생성됩니다.
* windows의 브러시 알파에 비트맵을 사용할 때 &lbrack;Tool&rbrack; 충돌
* &lbrack;내보내기&rbrack; 추가 맵 내보내기 사전 설정이 이제 위치에 대한 RGB 맵을 내보냅니다.

### 1.5.7

*(릴리스: 2015년 9월 24일)*

**고정:**

* 충돌 보고서가 더 이상 작동하지 않습니다.

### 1.5.6

*(릴리스: 2015년 9월 21일)*

**추가됨:**

* &lbrack;Shelf&rbrack; 축소판 렌더링 품질 향상(1K 텍스처 사용)

**고정:**

* &lbrack;Share&rbrack; 다른 계정으로 서명할 수 없음
* &lbrack;Shelf&rbrack; 축소판이 디스크에 너무 큼
* &lbrack;Shelf&rbrack; 스마트 재질 로드 속도가 매우 느림
* &lbrack;Windows&rbrack; 라이선스 서비스 설치 수정
* &lbrack;Channels&rbrack; 투과 맵은 기본적으로 G8로 만들어집니다

### 1.5.5

*(릴리스: 2015년 9월 15일)*

**추가됨:**

* &lbrack;Shelf&rbrack; 에셋을 Substance share으로 내보내기
* &lbrack;Shelf&rbrack; 재질에 대한 새 구 미리보기 추가
* &lbrack;Shelf&rbrack; 축소판 생성에 env 맵 &quot;글레이즈드 파티오&quot;를 사용합니다.
* &lbrack;Shelf&rbrack; 축소판 크기 해상도를 512x512 픽셀로 늘리기
* &lbrack;3D 보기&rbrack; 환경 회전 값 노출
* &lbrack;Windows&rbrack; 응용 프로그램에 서명

**고정:**

* &lbrack;Bakers&rbrack; 지도를 동시에 구울 때 잘못된 결과 발생
* &lbrack;3D 보기&rbrack; 프로젝트가 열려 있지 않으면 env 맵이 표시됩니다
* &lbrack;Layers&rbrack; 마스크 생성기가 레이어 콘텐츠에서 작동하지 않음
* &lbrack;Layers&rbrack; 숨겨진 레이어에 페인트 가능
* &lbrack;Shelf&rbrack; Dirt_5 및 Dirt_6 노이즈가 동일함
* &lbrack;Shelf&rbrack; 일부 마스크 생성기는 픽셀화되거나 저품질입니다.
* &lbrack;도구(&amp;r); 특정 각도에서 기즈모 회전이 잘못되었습니다.
* &lbrack;도구&rbrack; 채널이 너무 많으면 채널 버튼이 잘립니다.
* &lbrack;도구(&amp;r); 빠른 마스크에 대한 마스크 단축키 반전이 작동하지 않음
* &lbrack;내보내기&rbrack; Sketchfab: 취소 버튼이 제대로 고려되지 않음
* 라이선스를 복사할 수 없을 때 &lbrack;License&rbrack; 활성화하지 못함
* 프레임 속도 제한이 더 이상 UI에서 작동하지 않음

### 1.5.0

*(릴리스: 2015년 8월 20일)*

**추가됨:**

* &lbrack;Shader&rbrack; Shader 컴파일 오류 메시지에 줄 번호 추가
* &lbrack;Shelf&rbrack; 축소판 미리 보기 품질 향상
* &lbrack;Shelf&rbrack; 스마트 재질에 대한 축소판 생성 자동화
* &lbrack;Tool&rbrack; 단축키를 사용하여 Substance의 경도 설정 제어
* &lbrack;도구&rbrack; 마스크에 있을 때 모양 데칼에 회색 음영 위젯 사용
* 회색 음영 맵에 페인트하는 동안 페인트 색상을 반전시키는 &lbrack;도구&rbrack; 단축키
* &lbrack;뷰포트(&amp;r); 와이어프레임 표시 및 색상 변경 허용
* &lbrack;뷰 포트(&amp;r); 환경 배경에 흐림 효과 적용
* &lbrack;Controls&rbrack; 브러시 마우스 단축키에 회전 추가
* &lbrack;내보내기&rbrack; Sketchfab으로 내보내기
* &lbrack;내보내기&rbrack; 렌더러용 내보내기 사전 설정 만들기
* &lbrack;Export&rbrack; 변환된 맵 반사 추가, F0 및 1/IOR
* &lbrack;UI&rbrack; 시작 화면 추가
* &lbrack;UI&rbrack; 기본 레이아웃 업데이트
* &lbrack;UI&rbrack; 누락된 도구 설명을 추가하고 일부 메뉴 항목의 이름을 바꿉니다.
* &lbrack;Layers&rbrack; 현재 선택된 마스크를 비트맵으로 내보내기
* &lbrack;레이어&rbrack; 마우스 오른쪽 버튼 클릭 메뉴에서 &quot;마스크 반전&quot; 동작 추가

**고정:**

* &lbrack;프로젝트&rbrack; 메시 피벗이 FBX에서 다른 경우 가져올 때 메시가 분해됩니다
* 투영 도구에 사용된 &lbrack;Substance&rbrack; Substance은 256에서 잠깁니다.\*256
* 마스크 지우기를 사용할 때 &lbrack;Layers&rbrack; 충돌
* &lbrack;Export&rbrack; 매우 어두운 텍스처에서 감마 변환이 잘못됨
* &lbrack;Export&rbrack; 위치 맵은 회색 음영 맵으로 사전 설정 내보내기에만 사용할 수 있습니다.
* 마스크에서 사용할 때 &lbrack;도구&rbrack; 형상 데칼 시작 색상은 검정색입니다.
* 알파에 경도가 없는 경우 &lbrack;단축키(&amp;r)가 작동하지 않습니다.

### 1.4.2

*(릴리스: 2015년 7월 15일)*

**고정:**

* 빠른 마스크와 함께 형상 데칼을 사용할 때 &lbrack;Tool&rbrack; 충돌
* 프로젝트를 1.4.0에서 1.4.1로 업데이트하면 모든 컴퓨터 메모리가 소모됩니다
* 이전 프로젝트 형식을 잘못 가져옴
* 사용자 정의 셸프는 전체 계층 구조를 구문 분석하고 모든 곳에 에셋을 복제합니다.

### 1.4.1

*(릴리스: 2015년 6월 23일)*

**추가됨:**

* &lbrack;뷰포트(&amp;r); 패널을 나란히 고정할 수 있도록 허용
* &lbrack;효과&rbrack; 레벨 효과에 대한 배경과 눈금자 추가
* &lbrack;Effect&rbrack; 다른 효과를 사용할 수 있는 페인트 효과를 추가합니다

**고정:**

* 프로젝트가 열려 있지 않으면 &lbrack;Shelf&rbrack; 축소판 생성이 중단됩니다.
* &lbrack;Shelf&rbrack; 재질 사전 설정 미리 보기 생성 실패
* &lbrack;Shelf&rbrack; 재질 미리 보기가 반전된 표준이 있는 메시에 생성됩니다.
* &lbrack;Shelf&rbrack; 축소판은 잘못된 해시 함수 때문에 항상 다시 계산됩니다.
* &lbrack;Shelf&rbrack; Substance 재질을 클릭하면 추가 맵이 연결되지 않음
* &lbrack;도구&rbrack; 재료 선택기로 샘플링된 잘못된 값
* &lbrack;도구&rbrack; 색상 피커 뷰 포트 커서 색상 선택
* &lbrack;2D 보기&rbrack; 매우 낮은 프레임/성능
* 너무 최근 내보내기 사전 설정이 있는 내보내기 창을 열 때 &lbrack;Export&rbrack; 충돌.
* &lbrack;노멀 맵에 대한 Height 채널 내보내기&rbrack;가 잘못된 공간으로 변환됩니다.
* &lbrack;Mac&rbrack; Substance 효과의 BaseColor가 Linear로 표시됨
* &lbrack;Mac&rbrack; 직선 위젯이 Retina에 잘못 그려짐
* 직선은 단축키가 출시된 상태에서도 활성화된 상태를 유지할 수 있습니다.
* 환경 맵을 회전한 후 직선 구이즈모가 사라짐
* 물질의 앰비언트 오클루전 출력은 AO 채널에 자동으로 연결되지 않습니다
* 사용자 이름에 특수 문자가 있는 Windows에서 라이선스 복사 문제 해결

### 1.4.0

*(릴리스: 2015년 6월 10일)*

**추가됨:**

* &lbrack;내보내기&rbrack; 사용 가능한 입력 맵 목록에 추가 맵을 추가합니다.
* &lbrack;Shelf&rbrack; 재료 사전 설정으로 sbsar 재질 사용
* &lbrack;Shelf&rbrack; 사용자 정의 라이브러리 경로 사용 허용
* &lbrack;Shelf&rbrack; 최소 크기 변경
* &lbrack;Shelf&rbrack; 새로운 내용 : 20개의 새로운 스마트 재질
* &lbrack;Shelf&rbrack; 새로운 콘텐츠 : 새로운 프로시저 물질(직조, 메쉬)
* &lbrack;Shelf&rbrack; 흐림 효과 필터 업데이트
* 수정자 키를 사용하여 직선 그리기
* 앰비언트 오클루전 채널 추가 및 레이어 스택에서 AO/표준 동작 다시 작업
* Substance 사용자 데이터에 정의된 이미지 입력에서 기본 색상 읽기
* 도움말 메뉴에서 로그 내보내기 허용

**고정:**

* &lbrack;Baker&rbrack;&lbrack;Mac&rbrack; 메시 베이커에서 표준이 있는 충돌
* 케이지 파일에 UV가 없는 경우 &lbrack;Baker&rbrack; 충돌
* &lbrack;Baker&rbrack; zBrush에서 내보낸 OBJ에서 이름별 일치가 작동하지 않음
* &lbrack;Baker&rbrack; 케이지를 사용하여 굽으면 여러 텍스처 세트 및 겹치는 UV를 사용하는 경우 굽기를 덮어씁니다
* &lbrack;Baker&rbrack; 특정 OBJ 파일로 인해 검은색 텍스처 발생
* 읽기 전용으로 설정된 경우 &lbrack;Shelf&rbrack;에서 리소스를 읽을 수 없습니다.
* &lbrack;Shelf&rbrack; 에셋 파일이 프로젝트에 사용된 경우 Painter으로 작성되고 있습니다.
* &lbrack;Shelf&rbrack; 재로딩도 레이어 업데이트
* &lbrack;Export&rbrack; Tiff는 Photoshop 또는 게임 엔진에서 제대로 읽을 수 없는 32비트 이미지를 내보냅니다
* &lbrack;내보내기&rbrack; 기본 채널 사전 설정은 항상 RGB으로 내보내기
* &lbrack;재질&rbrack; 확산 채널이 재질이 있는 BaseColor 매핑을 재정의합니다.
* &lbrack;3D 보기&rbrack; 특정 환경 맵이 있는 확산 조명이 잘못됨
* &lbrack;Tool&rbrack; 브러시를 특정 각도로 회전할 수 없음
* 텍스트 필드에서 입력하는 동안 뷰포트가 켜져 있으면 포커스가 생김
* 사전 설정이 최신 버전의 선반에 비해 너무 최근의 충돌
* 망 교체 후 충돌
* 입력 수가 다른 Substance를 다시 로드할 때 충돌 발생
* Cinema4D 가져오기의 FBX 메시에서 질감 이름이 잘못되었습니다

### 1.3.5

*(릴리스: 2015년 5월 29일)*

**추가됨:**

* 기존 라이선스 파일이 있는 경우 &lbrack;License&rbrack; 활성화 문제
* 특정 FBX 파일을 로드할 때 &lbrack;Mac&rbrack; 충돌
* &lbrack;Mac&rbrack;&lbrack;3D 보기&rbrack; 통합 GPU에 대한 잘못된 반사
* &lbrack;3D 보기&rbrack; 빠른 마스크 글꼴이 손상되었습니다.
* &lbrack;3D 보기&rbrack; 재료 선택기로 뷰포트가 완전히 까맣게 됨
* 1.3.3에서 만든 프로젝트를 연 후 충돌
* 알파 포함 셰이더를 사용할 때 재질 미리 보기가 비어 있음
* 특정 메시에서 페인팅이 작동하지 않습니다.
* 특정 OBJ 메시로 인해 성능이 많이 저하됨
* 효과를 사용할 때 사용자 채널이 매핑되지 않습니다
* 시작 시 임시 폴더가 정리되지 않음

**고정:**

* 로드할 시간이 매우 긴 프로젝트의 계산 시간 개선
* &quot;GPU 문제 해결&quot; 창을 보다 이해하기 쉽게 변경합니다.
* &lbrack;Layers&rbrack; 칠 레이어의 비율 잠금 상태를 저장하고 기본적으로 &quot;설정&quot;으로 만듭니다
* &lbrack;Bakers&rbrack; 이제 이름별 일치에 구분 기호로 접미어를 사용합니다.

### 1.3.4

*(릴리스: 2015년 4월 27일)*

**추가됨:**

* Mac OS X Yosemite(10.10)가 포함된 &lbrack;Mac&rbrack; 충돌
* &lbrack;Mac&rbrack; 전체 화면 모드를 종료할 수 없음
* &lbrack;Bakers&rbrack; 이름별 일치 항목 굽기 옵션이 작동하지 않음
* &lbrack;Bakers&rbrack; SP에서 사용되는 Mikk 접선 공간이 UE4에서 작동하지 않음
* &lbrack;Bakers&rbrack; ID baker can&#39;t baking material ID colors
* 도형 데칼 도구를 사용할 때 &lbrack;2D 보기&rbrack; 와이어프레임이 나타나지 않음
* &lbrack;도구&rbrack; 브러시 알파 채널이 재질이 있는 투명도 대신 검사기로 표시됨
* 도형 데칼이 있는 &lbrack;Tool&rbrack; 충돌
* &lbrack;Layers&rbrack; 재질 슬롯은 기본적으로 채우기 레이어에서 축소됩니다.
* 텍스처 설정 해상도보다 큰 크기로 내보낼 때 &lbrack;내보내기&rbrack; 충돌
* Specular 채널이 필터에서 인식되지 않습니다.
* clean + save가 spp 아카이브에서 리소스를 제대로 스트립하지 않음
* 높은 다중 저장소 파일에 낮은 다중 변형 저장 안 함
* FBX 파일을 가져올 때 텍스처 세트가 너무 많습니다.

**고정:**

* 효과: 클램프 레벨은 기본적으로 &quot;클래식&quot; 레벨을 모방하기 위해 켜야 합니다
* 레이어: 칠 작업의 최소 및 최대 틸링 변경
* 레이어: 스택 상태 저장 및 복원
* 베이커: AO 베이커는 HP가 명시되지 않은 경우 노멀 맵을 고려한다.
* 베이커: 베이킹 창에 도구 설명 및 추가 정보 추가
* 프로젝트를 저장할 때 백업 파일 만들기

### 1.3.3

*(릴리스: 2015년 4월 1일)*

**추가됨:**

* 제목 표시줄에 소프트웨어 버전 및 프로젝트 이름 추가
* TextureSet 이름 및 스마트 재질 이름 기밀 정보 가리기
* Substance 엔진을 V5로 업데이트
* &lbrack;Shelf&rbrack; 새 환경 지도 추가 : Corsica beach, studio 05, Tornoco studio 등
* &lbrack;Shelf&rbrack; 새 매개변수로 MG Mask Builder 업데이트
* &lbrack;Shelf&rbrack; 이전 환경 맵 업데이트 및 보정

**고정:**

* 내보내기 창을 열 때 충돌
* 고정 해제 시 UI 위젯에서 드래그할 수 없음
* &quot;업데이트 확인&quot;이 작동하지 않음
* &lbrack;Layers&rbrack; 마스크를 Alt+클릭할 때 선택하지 않음
* &lbrack;도구&rbrack; 3회 평면이 일반 채널에서 작동하지 않음
* env 맵의 &lbrack;3D 보기&rbrack; 확산 조명이 올바르지 않음
* &lbrack;3D 보기&rbrack; 노출 계산이 Designer과 다름
* &lbrack;3D 보기&rbrack; 그림자는 100% 금속 표면에 표시되지 않아야 합니다.
* 대칭복사된 UV가 있는 &lbrack;3D 보기&rbrack; 메쉬에 대칭 탄젠트/이각이 있습니다.
* &lbrack;3D 보기&rbrack; 그림자가 특정 메시에서 잘못된 결과를 생성합니다.
* &lbrack;Bakers&rbrack; assbin 파일에 의해 생성된 &quot;.alg_meta&quot; 폴더 제거
* Painter이 동시에 TextureSet를 다시 계산하는 경우 굽기를 수행할 때 &lbrack;Bakers&rbrack; 충돌
* 응용 프로그램 실행 시 &lbrack;Mac&rbrack; 화이트 박스 UI 결함

### 1.3.2

*(릴리스: 2015년 3월 6일)*

**고정:**

* &lbrack;3D 보기&rbrack; 프로젝트와 함께 저장된 env 맵을 다시 로드하지 못함

### 1.3.1

*(릴리스: 2015년 3월 5일)*

**추가됨:**

* &lbrack;Bakers&rbrack; 캐시된 버전의 high-poly 메시를 추가하여 계산 속도를 높입니다.
* &lbrack;Bakers&rbrack; 하이 폴리 메쉬가 로드되지 않은 경우 경고 아이콘을 추가합니다.
* &lbrack;Bakers&rbrack; 높은 폴리 메쉬가 로드되지 않은 경우 프로젝트 메쉬를 대신 사용합니다.

**고정:**

* &lbrack;Bakers&rbrack; 슬라이더 값을 편집할 때 &quot;enter&quot; 키를 누르면 창이 닫힙니다.
* &lbrack;베이커&rbrack; 베이커 활성화/비활성화도 버튼을 트리거합니다.
* &lbrack;Bakers&rbrack; &quot;all/none&quot; 단추를 사용하면 구울 수 없습니다.
* &lbrack;Bakers&rbrack; 제빵사 버튼의 정렬이 올바른 순서가 아닙니다
* &lbrack;Bakers&rbrack; 확인란이 무시되고 모든 베이커가 항상 처리됩니다.
* &lbrack;Bakers&rbrack; 진행률 표시줄 진행률 수정

### 1.3.0

*(릴리스: 2015년 3월 4일)*

**추가됨:**

* &lbrack;Bakers&rbrack;&lbrack;tangents/binormals가 없는 경우 mikkt 탄젠트 공간 계산을 사용합니다.
* &lbrack;베이커&rbrack; 새 베이커 추가 : 일반, ID, 오클루전, 곡률, Thickness, 위치
* &lbrack;Effects&rbrack; 효과 스택이 이제 반전되어 위에서 아래로 표시됩니다(레이어처럼).
* &lbrack;효과&rbrack; 효과 스택에 새 아이콘 추가
* &lbrack;효과&rbrack; 효과 스택에서 칠 작업 사이에 혼합 모드 추가
* &lbrack;Effects&rbrack; 효과 이름 바꾸기(substance effect = filter 등)
* 저장 프로세스 중에 &quot;잠금&quot; 파일 추가
* &lbrack;효과&rbrack; 효과 스택에 채우기 작업 추가
* 새 리소스 추가됨 : 스마트 재질
* &lbrack;레이어&rbrack; 레이어 효과 재정렬 허용
* &lbrack;도구&rbrack; 3회 평면 투영 추가
* &lbrack;3D 보기&rbrack; 그림자 지원 추가
* &lbrack;3D 보기&rbrack; 필요한 OpenGL 상태를 사용자 정의 셰이더로 설정하는 기능
* &lbrack;3D 보기&rbrack; 새로운 셰이더를 통한 알파 지원
* &lbrack;3D 보기&rbrack; 셰이더의 버전이 관리되고 프로젝트에 완전히 저장됩니다.
* &lbrack;3D 보기&rbrack; 셰이더가 더 이상 컴파일되지 않을 경우 사용자에게 경고합니다.

**고정:**

* &lbrack;Layers&rbrack; 접힌 폴더 아래의 드롭 수정
* &lbrack;Shelf&rbrack; 미니 쉘프의 콘텐츠 필터링 수정
* &lbrack;Shelf&rbrack; 범주 이름 바꾸기 및 탭 재구성

### 1.2.1

*(릴리스: 2015년 2월 12일)*

**추가됨:**

* 이제 탐색기에서 두 번 클릭하여 \*.spp 파일을 열 수 있습니다.
* &lbrack;내보내기&rbrack; 내보내기 사전 설정에 대한 새로운 &quot;$project&quot; 태그
* &lbrack;내보내기&rbrack; 각 텍스처 세트 아래에 맵 목록 추가(이름 지정 포함)
* &lbrack;내보내기&rbrack; 텍스처 세트를 선택하려면 모두/없음 버튼을 추가합니다
* &lbrack;Export&rbrack; 내보내기 중 빈 맵이 삭제됩니다.

**고정:**

* &lbrack;내보내기&rbrack; Unity5 사전 설정에 반전된 맵이 있음
* &lbrack;내보내기&rbrack; 사전 설정 이름에 슬래시를 추가하면 손상된 폴더가 생성됩니다.
* 32비트 형식으로 내보낸 &lbrack;Export&rbrack; Height 채널이 잘못 클램프됩니다
* &lbrack;내보내기&rbrack; 텍스처 세트 목록이 프로젝트에서처럼 정렬되지 않음
* &lbrack;도구&rbrack; 백페이스 컬링이 더 이상 작동하지 않음
* 경로에 있는 특수 문자에 대해 저장 기능이 작동하지 않음

### 1.2.0

*(릴리스: 2015년 1월 28일)*

**추가됨:**

* 노멀 맵 데이터를 페인트 하고 결과를 결합할 수 있는 새로운 표준 채널
* &lbrack;Export&rbrack; 사용자 정의 패킹 생성 및 사용자 정의 이름 설정 기능이 있는 새 내보내기 창
* 이제 프로젝트 파일 형식이 폴더 대신 단일 파일입니다
* &lbrack;내보내기&rbrack; 다른 일반 형식(DirectX, OpenGL) 지원
* &lbrack;Export&rbrack; 내보내기 중 임시 &quot;잠금&quot; 파일 만들기
* &lbrack;레이어&rbrack; Shift+마우스 클릭을 사용하여 마스크 전환
* &lbrack;Parameters&rbrack; 이미지 입력 하단에 색상 공간 노출
* &lbrack;Shelf&rbrack; 효과 &quot;MG Mask Builder&quot;에 새로운 설정이 포함됨
* &lbrack;3D 보기&rbrack; 앰비언트 오클루전 맵에서 이제 Specular이 아닌 확산 기여도를 숨깁니다.

**고정:**

* 투영 재질/스텐실 미리 보기가 뷰포트에 제대로 표시되지 않음
* &quot;S&quot;(스텐실) 단축키를 사용할 때 &lbrack;3D 보기&rbrack; 단축키 툴팁이 표시되지 않음
* &lbrack;Shelf&rbrack; 효과 &quot;MatFx Skin Scale&quot;이 이제 저해상도에서 더 나은 성능을 제공합니다.
* 더 큰 문서 크기를 지정할 때 내보내기에서 내보내는 &lbrack; 내보내기&rbrack; 텍스처가 방금 확대됩니다.

### 1.1.2

*(릴리스: 2015년 1월 15일)*

**추가됨:**

* 추가됨: 채우기 레이어에서 새로운 변환, 회전 및 비율 설정
* 브러시 및 칠 레이어에 대한 향상된 필터링
* 이제 평가판 버전은 완전히 기능을 갖추고(내보낼 수 있음) 있지만 시간이 제한됩니다.

**고정:**

* 매우 작은 정밀도로 OBJ 메시를 가져올 수 없음
* Windows 7 및 8에서 라이선스를 활성화할 때 발생하는 문제
* 프로젝트 &quot;다른 이름으로 저장&quot; 중 충돌
* 텍스처 세트의 마지막 채널을 삭제할 때 충돌
* 특정 컨텍스트에서 레이어를 삭제할 때 충돌

### 1.1.1

*(릴리스: 2014년 12월 25일)*

**추가됨:**

* &lbrack;Layer&rbrack; 프로젝트/전환 텍스처 세트를 열 때 맨 위에 있는 레이어를 선택합니다.
* 새로운 압축 알고리즘으로 &quot;저장&quot; 및 &quot;다른 이름으로 저장&quot; 속도를 개선했음
* Painter에 대해 너무 최근에 프로젝트를 열 때 오류 표시

**고정:**

* &lbrack;Tool&rbrack; 형상 데칼(Geometry decal)은 메모리 손상을 생성합니다.
* &lbrack;Brush&rbrack; 브러시 크기에 대해 1 미만의 부동 소수점 값을 수동으로 입력할 수 없음
* &lbrack;레이어&rbrack; 색상 선택 효과를 만들어도 레이어 스택에 추가되지 않음
* &lbrack;Layer&rbrack; 레이어 위로 마우스를 이동하면 Painter이 작업 표시줄에서 깜박임
* &lbrack;Layer&rbrack; 비트맵을 마스크로 추가하면 충돌이 발생할 수 있습니다.
* Height 채널이 있는 솔로 모드의 GUI가 올바르지 않습니다.
* &quot;프로젝트 저장&quot;이 실패하고 프로젝트가 손상될 수 있습니다.
* 오래된 셰이더가 있는 다른 프로젝트를 로드한 후 프로젝트를 열 때 충돌

### 1.1.0

*(릴리스: 2014년 12월 16일)*

**추가됨:**

* &lbrack;효과&rbrack; 새 질감 ID 마스크 작성자
* 브러시 기즈모에 닷지 모양의 흰색/검은색 새 선
* 새 각도 follow 매개 변수
* 새로운 백페이스 컬링 매개 변수
* 새 레이지 마우스 매개 변수
* &lbrack;Layers&rbrack; 다중 선택 및 관리 지원
* &lbrack;레이어&rbrack; 한 텍스처 세트에서 다른 텍스처 세트로 복사 및 붙여넣기
* &lbrack;내보내기&rbrack; Adobe Photoshop PSD 형식
* &lbrack;Shelf&rbrack; 새로운 도구 : 모피, 금속 스티치 및 지퍼
* &lbrack;Shelf&rbrack; 새로운 브러시 : 몰드, 연필, 날카로운 선 및 스티치
* &lbrack;Shelf&rbrack; 새로운 알파 : 가우시안 노이즈, 날카로운 선, 주형, 펜, 스플래시, 스티치, 지퍼
* 필요한 텍스처 일부만 업데이트하여 페인팅 성능이 향상되었습니다.

**고정:**

* &lbrack;Shelf&rbrack; 동일한 레이블을 가진 그래프로 실체를 로드할 수 없음
* &lbrack;Layers&rbrack; 통과 혼합 모드가 마스크에서 작동하지 않음
* 2D 보기에서 &lbrack;Stencil&rbrack; 배율 나누기
* Mac OS Yosemite 관련 문제 및 충돌

### 1.0.2

*(릴리스: 2014년 11월 9일)*

**추가됨:**

* 재질이 포함된 재질 미리보기의 성능 개선
* 문서를 업데이트할 때 브러시 획 미리 보기를 사용하여 성능을 개선했습니다.
* 비작업 영역에 대한 업데이트 비율이 낮은 뷰포트에서 성능 개선
* &lbrack;포스트 효과&rbrack; 설정 관리를 위한 UI 개선
* &lbrack;포스트 효과&rbrack; 기본값으로 재설정
* 오른쪽 클릭 메뉴에서 효과 및 레이어 작업 Substance
* 물질에 미리 곱하기 입력/출력 지원

**고정:**

* &lbrack;3D 보기&rbrack; 사용자 정의 셰이더 매개변수는 큰 공간으로 분리됩니다.
* &lbrack;Export&rbrack; Unity4 사전 설정에 대한 sRGB 변환 누락
* fbx 메시를 로드할 때 가능한 충돌
* 단순 obj 메시를 로드할 때 가끔씩 충돌 발생
* 로드 시 컴퓨팅 바가 100%까지 차단됨
* 물질을 다시 로드하면 모든 범주에 들어갑니다
* DirectX/OpenGL 스위치 고장

### 1.0.1

*(릴리스: 2014년 10월 27일)*

**추가됨:**

* &lbrack;Tool&rbrack; 개선된 재료 매개변수 사용
* 도움말 메뉴의 Uservoice 웹 사이트에 대한 새 단축키
* 엔진의 다양한 성능 향상

**고정:**

* 매개 변수 값은 파티클에 대해 2개의 소수로 제한됩니다
* 캐시에서 로드한 Substance이 오래된 것으로 UI에 표시되지 않음
* 네트워크 url에서 메시를 로드할 때 충돌
* 이제 Painter이 Mac OS X에서 서명된 것으로 인식됩니다.

### 1.0.0

*(릴리스: 2014년 10월 15일)*

**추가됨:**

* 사용자 정의 셰이더 지원
* 4k 해상도 지원
* 샘플 문자 프로젝트
* 긴 계산 시간에 대한 진행률 표시줄 표시
* &lbrack;내보내기&rbrack; 확산 후처리 전에 확장 패스 추가
* 간단한 작업을 위한 SP의 명령줄 인수
* 새로운 재질 및 효과
* 도구 미리 보기(실시간 재질 미리 보기와 획 테스트 영역으로 구분)
* Painter 시작 시 기본 문서 만들기 안 함
* &lbrack;도구(&amp;r); 회색 음영 값을 수동으로 편집할 가능성을 추가합니다.
* 스텐실의 다양한 개선 사항(스냅, 재설정)
* 파티클은 이제 페인팅 브러시, 지우개 및 투영 도구의 하위 도구입니다
* &lbrack;3D 보기&rbrack; 뷰포트 렌더링에서 구운 AO 사용
* 2D 및 3D 보기 간 스텐실 컨트롤 분할
* 라이브러리에서 작은 엄지 크기 수정
* 검색 필드는 각 창마다 다릅니다.
* UI 수정

**고정:**

* &lbrack;Substance&rbrack; 스위치가 작동하지 않습니다.
* &lbrack;색상 대화 상자&rbrack; 색조 그레이디언트를 새로 고치지 않음
* 파일 이름이 동일한 경우 메시를 업데이트할 수 없습니다.
* 도구가 너무 작으면 보기에 표시되지 않음
* Retina 디스플레이의 데칼 도구가 제대로 작동하지 않음
* &lbrack;Substance&rbrack; Int1은 float1로 표시됩니다.
* &lbrack;Substance&rbrack; 기본 색상 입력/출력이 인식되지 않음
* &lbrack;Substance&rbrack; 필터는 다시 로드할 수 없음
* &lbrack;도구(&amp;r)rbrack; 회색 음영 위젯은 항상 축소됩니다.

## 베타

### 0.12.1-베타

*(릴리스: 2014년 9월 18일)*

**추가됨:**

* Unity 5 내보내기 사전 설정

**고정:**

* PBR 셰이더, 렌더링 품질이 많이 개선되어야 합니다
* 포커스 기능이 끊어지고 기본적으로 메시가 잘립니다

### 0.12.0-베타

*(릴리스: 2014년 9월 17일)*

**추가됨:**

* 스포이드 도구
* 테두리 상자가 변경될 때 메시 다시 가져오기에 &quot;선 위치 유지&quot; 옵션이 추가되었습니다.
* Cymourai 기본 메시 노멀 맵
* 도구 뷰 인터페이스 개선(색상이 진행 중)
* &quot;도움말->설정&quot; 메뉴를 &quot;편집->설정&quot;으로 이동
* &quot;모든 채널 내보내기&quot; 창에서 내보내기 경로 저장
* 새로운 수준의 GUI 및 히스토그램 표시
* 자산 관리 개선(드래그 앤 드롭, 리소스 다시 로드, 미사용 삭제)
* &quot;확산&quot;에서 &quot;기본 색상&quot;으로 전환
* 슬라이더 편집 조정 - 쉼표 외에 점 허용
* 칠 레이어: 최대 타일링 값 늘리기
* 기본 환경 맵

**고정:**

* 극단적인 각도의 잘못된 반사 가공물
* 깨진 Specular/광택 내보내기
* Painter의 &quot;정보&quot; 창에 있는 링크가 작동하지 않음
* OSX Yosemite와 충돌
* 메쉬 저장 삼각측정
* [도구] 창의 색상 단축키가 회색 음영 대신 에미터로 전송됩니다
* 레이어에서 마스크로 전환할 때 색상 피커가 열린 상태 유지
* 채우기 레이어의 재질을 저장할 수 없음
* 선반의 세 영역 크기 조정 활성화

### 0.11.0-베타

*(릴리스: 2014년 9월 4일)*

**추가됨:**

* 3D 보기와 2D 보기 사이에 분할 영역 추가
* 2D/3D 보기에서 그레이디언트 배경 사용
* 레벨 막대 그래프에 대한 인터페이스
* 선반과 라이브러리 병합
* 사전 설정을 만들거나 업데이트할 때 저장 작업이 필요하지 않음
* 드래그하여 놓기를 통해 셸프의 에셋 가져오기

**고정:**

* 버튼의 이름이 기본 도구 모음에 표시됩니다.

### 0.10.2-베타

*(릴리스: 2014년 8월 28일)*

**고정:**

* 모든 채널을 내보내면 잘못된 결과가 표시됨

### 0.10.1-베타

*(릴리스: 2014년 8월 26일)*

**고정:**

* 셰이더는 낮은 거칠기의 검정 결과를 제공합니다.
* GPU 확인: &#39;Quadro&#39; 카드를 처리하고 모든 장치를 감지하고 그에 따라 사용자 메시지를 조정합니다.
* 대부분의 물질 물질은 베타 9에서 256으로 제한되어 있습니다
* Height을 비트맵으로 내보낼 때 고정되어 표시됨
* 브러시 미리 보기가 Mac의 투영 오버레이와 다릅니다
* 모양 도구를 사용하여 마스크를 만들면 뷰포트에 표시되지 않습니다
* 빠른 마스크가 끊어짐
* 이전 mac pro에서의 혼합 문제 해결

### 0.10.0-베타

*(릴리스: 2014년 8월 7일)*

**추가됨:**

* 스텐실 마스크

**고정:**

* Quadro 카드 지원
* 셰이더는 낮은 거칠기의 검정 결과를 제공합니다.
* Substance 재료는 256으로 캡핑됨
* 노멀 맵 내보내기가 녹색 채널을 삭제합니다

### 0.9.0-베타

*(릴리스: 2014년 7월 17일)*

**추가됨:**

* Yebis 2 사후 처리
* 새 프로젝트 마법사를 사용하면 입력 맵(AO, 곡률 등)을 가져올 수 있습니다.
* 입력 맵 자동 연결(AO, 곡률 등) 효과 Substance
* 칠 레이어에 적용된 재질에 대한 비율 제어

### 0.8.2-베타

*(릴리스: 2014년 7월 11일)*

**고정:**

* 색조 슬라이더는 흰색으로 기본 설정됨
* 재질 이름에 특수 문자가 포함된 경우 프로젝트 재설정
* 단일 재료 개체에 대한 재료 이름 변경은 프로젝트를 무효화하지 않아야 합니다.
* 프로젝트를 저장하고 다시 열면 UV가 엉망이 됨

### 0.8.1-베타

*(릴리스: 2014년 7월 4일)*

**고정:**

* 다중 GPU 충돌
* 충돌 내보내기 시 채널 표시

### 0.8.0-베타

*(릴리스: 2014년 6월 28일)*

**추가됨:**

* 다중 재질 - 이제 동일한 문서에서 여러 재질을 페인트 할 수 있습니다
* 대칭 페인팅
* 이제 모든 혼합 모드를 사용할 수 있습니다.

**고정:**

* 다중 GPU 충돌
* 재질 이름에 특수 문자가 포함된 경우 프로젝트 재설정
* 프로젝트를 저장한 후 UV가 엉망이 되어 여러 UV로 다시 열림

### 0.7.0-베타

*(릴리스: 2014년 6월 18일)*

**추가됨:**

* 레이어 효과
* 새로운 Substance 스텐실 재질
* 마스크 지우기
* 레이어/마스크 복사/붙여넣기 허용
* 레이어 복제 허용
* 레이어 마스크를 편집할 때 도구 변경
* 이제 Substance에 GPU 지원

**고정:**

* 높이 맵 페인팅은 음수 값을 페인트로 지정하지 않습니다.
* [재질 선택기] 디스플레이는 샘플링된 노멀 맵을 고려하지 않아야 합니다
* 입자 결정론 고장
* 2D 보기의 스텐실 매트릭스
* Obj 파일의 Ngons
* 다양한 충돌

### 0.6.0-베타

*(릴리스: 2014년 6월 4일)*

**추가됨:**

* 거칠기와 금속 채널의 합성에서 Specular 맵을 내보내는 새로운 내보내기 옵션

**고정:**

* Windows Vista 호환성
* 높이 맵에서 음수 값을 페인트 하지 않습니다.

### 0.5.0-베타

*(릴리스: 2014년 5월 7일)*

**추가됨:**

* 3D/2D 보기 스위치
* UV 청크 선택 도구
* 마스크에 페인팅할 때 도구가 자동으로 변경됩니다.
* Substance 해결은 문서의

**고정:**

* 실행 시 충돌
* ASCII 메시가 있는 충돌
* 2D 보기의 고정된 스텐실 매트릭스
* 지우개 충돌

### 0.4.0-베타

*(릴리스: 2014년 4월 17일)*

**추가됨:**

* 원활한 2D 보기
* 비트맵 레이어 마스크
* 환경 노출 제어
* 칠 레이어는 이제 도구 창을 사용하여 속성을 설정합니다
* 재질은 칠 레이어에 적용할 수 있습니다
* 스텐실 라이브러리에 스텐실 추가
* 더 빠른 계산을 위해 입자 사전 설정이 업데이트됨
* 낮은 품질 설정을 위한 PBR 셰이더 최적화 및 품질 개선

**고정:**

* 레이어 축소판이 현재 선택한 채널에 연결되어 있음
* 많은 충돌

### 0.3.0-베타

*(릴리스: 2014년 4월 4일)*

**추가됨:**

* 높이 맵 페인팅에 대해 색상 선택기에서 음수 값 허용
* 선택한 재질/색상의 미리보기 표시
* 도구 모음에 도구에 대한 단축키 추가(1,2,3,4)
* 프로젝트에서 표준 형식(OpenGL 및 DirectX)을 전역적으로 전환
* 새 프로젝트 마법사
* 간격 슬라이더가 더 이상 고정되지 않음
* 업데이트된 슬라이더 스타일
* 색상 피커를 모달이 아닌 모양으로 만들기
* 라이브러리로 재질을 선택하면 그에 따라 도구 유형이 설정됩니다

**고정:**

* 수정: 가져오기 메시 경로가 유지되지 않습니다.
* 수정: 잘못된 텍스처 생성
* 수정: 시작할 때 충돌 발생

### 0.2.0-베타

*(릴리스: 2014년 3월 17일)*

**추가됨:**

* 재질 스포이드(P 단축키)
* 3d 도구 미리 보기 아래의 축소판
* 독립 실행형 버전에 대한 라이선스 시스템
* 브러시 크기에 대한 &lbrack; 및 &rbrack; 단축키
* 내보낸 맵의 패딩
* 업데이트된 도구 창 스타일
* 업데이트된 슬라이더 스타일
* 업데이트된 기본 HDR 환경

**고정:**

* 스텐실: 3D 보기의 흐름 값 변경이 52에서 중지됨
* 스트로크에 0 압력 키를 추가할 때 엔진의 무한 루프가 고정되어 있습니다.
* 도구: 각도 지터가 +/- 90% 이상의 값을 반환하지 않음
* 레이어 마스크를 선택한 경우 3D 보기 표시 변경
* 반전된 확대/축소

### 0.1.0-베타

*(릴리스: 2014년 3월 2일)*

**추가됨:**

* 새 라이브러리 관리
* 새로운 브러시 및 파티클 콘텐츠
* 3D 브러시 미리 보기
* 업데이트된 도구 창 스타일
* 업데이트된 슬라이더 스타일
* 업데이트된 캐시 성능

**고정:**

* 카메라 컨트롤
* 브러시 회전
