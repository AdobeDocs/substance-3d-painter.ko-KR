---
source-git-commit: 0376fe6500551442b28831d5742ecbbc9363ab19
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 1%

---
# 알려진 문제 생성기 — Substance 3D Painter

Substance 3D Painter에 대해 알려진 문제 마크다운 문서를 자동으로 생성, 다음 위치에 게시:
`https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html`

문제는 Jira epic `SBSFOUR-6267`에서 출처입니다. 이 스크립트는 모든 문제를 불러오고, 대상 버전에서 이미 수정된 모든 것을 필터링하며, 포맷 된 마크다운 파일을 출력할 준비가 되었습니다.

---

## 빠른 시작

이 단계에서는 아래의 일회성 설정을 이미 완료했다고 가정합니다.

1. **GlobalProtect VPN**&#x200B;에 연결
2. `.env` 파일의 `TARGET_VERSION`을(를) 문서를 생성하는 버전으로 설정합니다(예: `12.0.3`).
3. `scripts/known-issues-automation/` 디렉터리에서 스크립트를 실행합니다.

   ```
   python fetch_known_issues.py
   ```
4. 출력 요약을 확인합니다. 몇 개의 문제를 가져왔으며 몇 개가 제외되었는지 보고합니다.
5. 생성된 `known-issues.md`을(를) `help/release-notes/known-issues.md`(으)로 복사

> 문제가 누락되었거나 예기치 않은 경우 `raw_issues.json`을(를) 검사하여 필터링이 적용되기 전에 Jira가 반환한 내용을 정확하게 확인하십시오.

---

## 1회 설정

### &#x200B;1. 종속성 설치

```bash
pip install requests python-dotenv
```

### &#x200B;2. `.env` 파일 만들기

```bash
cp .env.example .env
```

### &#x200B;3. Jira 개인 액세스 토큰 받기

1. `https://jira.corp.adobe.com`에 로그인
2. 왼쪽 사이드바→ **개인 액세스 토큰** 프로필로 이동합니다.
3. **토큰 만들기**&#x200B;를 클릭하고 이름을 지정한 다음 생성된 값을 복사합니다.

> PAT는 브라우저 세션이 종료되면 만료되지 않으므로 스크립팅된 API 액세스를 위한 세션 쿠키보다 더 안정적입니다.

### &#x200B;4. `.env` 파일 채우기

```
JIRA_PAT=your-personal-access-token
TARGET_VERSION=12.0.3
OUTPUT_FILE=known-issues.md
```

`TARGET_VERSION`은(는) 알려진 문제 페이지를 생성하는 Substance 3D Painter 버전입니다. 어떤 수정된 문제가 제외되는지 제어합니다. 아래의 [필터링 논리](#filtering-logic)를 참조하십시오.

---

## 저장소 구조

```
.
├── README.md                  # This file
├── fetch_known_issues.py      # Main script
├── .env.example               # Environment variable template (safe to commit)
├── .env                       # Your local credentials — never commit this
├── raw_issues.json            # Raw Jira dump from last run — gitignored
└── known-issues.md            # Generated output from last run — gitignored
```

---

## Jira Reference

| 필드 | 값 |
|---|---|
| Jira 인스턴스 | `https://jira.corp.adobe.com` |
| 프로젝트 키 | `SBSFOUR` |
| 알려진 문제 epic | `SBSFOUR-6267` |

알려진 모든 문제가 이 서사시에 연결되어 생성된 문서에 나타나야 합니다. 문제를 페이지에 추가하거나 제거해야 하는 경우 마크다운을 수동으로 편집하는 대신 Jira에서 서사를 업데이트하십시오.

---

## 스크립트 작동 방식

### 1단계 — 가져오기

스크립트는 JQL을 사용하여 Jira REST API를 쿼리합니다.

```
"Epic Link" = SBSFOUR-6267 ORDER BY created ASC
```

결과는 페이지당 50개의 문제로 페이지가 지정됩니다. 각 문제에 대해 다음 필드가 검색됩니다. `summary`, `issuetype`, `status`, `affectedVersions`, `fixVersions`, `labels`.

인증에서 `JIRA_PAT`의 전달자 토큰을 사용합니다. 회사 Jira 인스턴스는 내부 SSL 인증서를 사용하므로 이러한 요청에 대해 인증서 확인이 비활성화됩니다. 이는 Adobe 네트워크에서 예상된 동작입니다.

### 2단계 — Raw 덤프

필터링 또는 서식 지정 전에 스크립트는 `raw_issues.json`을(를) 씁니다. 이는 Jira가 반환한 모든 문제에 대한 간단한 스냅샷이며, 다음에 어떤 일이 일어나든 항상 생성됩니다. 출력이 잘못 보이면 먼저 이 파일을 검사하십시오. Jira가 제공한 데이터가 정확히 표시됩니다.

### 3단계 — 필터

두 가지 규칙이 함께 적용되어 문제가 필터링됩니다.

1. **상태 필터** — `Backlog` 및 `Dev In Progress` 문제만 알려진 활성 문제입니다. 상태가 `Fixed`인 문제는 제외할 후보이며, 아래 버전을 확인할 수 있습니다.

2. **버전 필터** — `Fixed` 문제는 수정 버전 중 하나가 `TARGET_VERSION`보다 작거나 같은 경우에만 제외됩니다. 수정 버전이 `TARGET_VERSION`보다 높은 경우 문서화 중인 버전에 대한 수정 사항이 제공되지 않았으므로 문제가 계속 포함됩니다.

두 버전이 동시에 개발 중인 경우를 처리합니다. `12.1.0`에서 수정된 문제는 `12.0.3`에 대해 알려진 문제로 남아 있습니다.

전체 결정 테이블에 대해서는 [필터링 논리](#filtering-logic)를 참조하십시오.

### 4단계 — 범주 구문 분석

각 문제 요약은 문자열 시작 시 범주 태그에 대해 구문 분석됩니다.

- `[Shader] Some description` → 범주: `["Shader"]`, 설명: `"Some description"`
- `[Crash][Engine] Some description` → 범주: `["Crash", "Engine"]`, 설명: `"Some description"`
- `No brackets here`→이(가) 분류되지 않은 것으로 처리되어 범주 없음

**기본 범주**&#x200B;는 항상 첫 번째 태그입니다. 그룹화 및 섹션 배치를 결정합니다.

### 5단계 — 그룹화 및 정렬

문제는 다음과 같이 구성됩니다.

- 문제는 기본 범주별로 그룹화됩니다.
- 그룹은 문제 수, 내림차순(가장 큰 그룹이 먼저)으로 정렬됩니다.
- 문제가 두 개 이상인 그룹이 문서 상단에 표시됩니다
- 문제가 하나뿐인 그룹과 분류되지 않은 문제는 섹션 헤더가 없는 다중 문제 그룹 뒤에 표시됩니다
- `[Crash]`을(를) 기본 범주로 사용하는 문제는 항상 `## Stability` 섹션 아래에 있습니다.

### 6단계 — 포맷 및 쓰기

스크립트 출력 `known-issues.md`:

- YAML 앞면 문제 (helpx 메타데이터)
- 대상 버전의 이름을 지정하는 소개 단락이 있는 `# Known issues` 제목
- 다음 형식으로 서식이 지정된 문제: `` * `[Category]` Description ``
- 다중 범주 문제: `` * `[Category1]` `[Category2]` Description ``
- 범주 그룹 사이의 빈 줄
- 충돌 문제에 대한 `## Stability` 섹션 끝

---

## 필터링 논리

| 상태 | 버전 세트를 수정하시겠습니까? | 버전 및 대상 수정 | 포함되었습니까? |
|---|---|---|---|
| `Backlog` | — | — | 예 |
| `Dev In Progress` | — | — | 예 |
| `Fixed` | 아니요 | — | 아니요(보수적으로 제외) |
| `Fixed` | 예 | 대상≤ 버전 수정 | 아니요(이미 배송됨) |
| `Fixed` | 예 | 버전 > 대상 수정 | 예(수정 사항은 향후 버전임) |

---

## 출력 포맷

```markdown
---
helpx_url: "https://helpx.adobe.com/substance-3d-painter/release-notes/know-issues.html"
...
---

# Known issues

This page lists all the active known issues present in v12.0.3 of Substance 3D Painter:

* `[Engine]` Error when using Smart Materials if Texture Set has no tile 1001
* `[Engine]` Geometry mask shows artifacts at UV borders with instanced layers

* `[Shader]` user0 channel always can not be read as sRGB with specific shader

* `[Export]` GLTF exports at the wrong size
* `[Import]` Cannot import obj file with "nan" values

## Stability

* `[Crash]` Select "Export mesh" when mesh failed to load
```

**서식 메모:** 범주 태그는 이중 백틱이 아닌 단일 백틱 래핑(`` `[Category]` ``)을 사용합니다. 기존 수동으로 유지 관리된 문서에 이중 백틱 오류가 포함되었습니다. 스크립트는 항상 올바른 형식을 생성합니다.

---

## 문제 해결

**401 권한 없음**
- **GlobalProtect VPN**&#x200B;에 연결되어 있는지 확인
- PAT가 만료되었거나 해지되었을 수 있습니다. `https://jira.corp.adobe.com/secure/ViewProfile.jspa`에 새 PAT를 생성하고 `.env`을(를) 업데이트하십시오.

**`JIRA_PAT is not set`오류**
- `.env.example`에서 `.env` 파일을 만들고 토큰을 입력했는지 확인하세요.
- `python-dotenv`이(가) `.env` 파일을 찾을 수 있도록 `scripts/known-issues-automation/` 디렉터리 내에서 스크립트를 실행하고 있는지 확인합니다.

**출력에서 누락된 문제**
- `raw_issues.json` 확인 — 문제가 없는 경우 Jira에서 epic `SBSFOUR-6267`에 연결되지 않습니다.
- 문제가 `raw_issues.json`에 있지만 출력에는 없는 경우 필터에 의해 제외되었습니다. `TARGET_VERSION`에 대해 문제를 확인하고 버전을 수정하십시오.

런타임에 **`TARGET_VERSION`경고**
- 스크립트가 실행되지만 `TARGET_VERSION`이(가) 설정되지 않은 경우 모든 `Fixed` 문제가 보수적으로 제외됩니다. 최종 문서를 생성하기 전에 항상 설정하십시오.
