---
id: STRUCTURE-001
version: 0.1.2
status: active
created: 2025-10-01
updated: 2025-11-06
author: @Alfred
priority: high
---

# roadmap Structure Design

## HISTORY

### v0.1.2 (2025-11-06)
- **UPDATED**: Feynman Learning Method integrated into system architecture
- **AUTHOR**: @Alfred
- **SECTIONS**:
  - Updated @DOC:ARCHITECTURE-001 (4-layer Feynman architecture)
  - Updated @DOC:MODULES-001 (4 modules: Concept Selection, Simplification Engine, Validation System, Output Formats)
  - Updated TODO:STRUCTURE-001 (4 structural improvement items)
- **RATIONALE**: Designed knowledge transfer structure based on Feynman's teaching principles

### v0.1.1 (2025-10-17)
- **UPDATED**: Template version synced (v0.3.8)
- **AUTHOR**: @Alfred
- **SECTIONS**: Metadata standardization (single `author` field, added `priority`)

### v0.1.0 (2025-10-01)
- **INITIAL**: Authored the structure design document
- **AUTHOR**: @architect
- **SECTIONS**: Architecture, Modules, Integration, Traceability

---

## @DOC:ARCHITECTURE-001 System Architecture

### Architectural Strategy: 파인만 학습법 기반 지식 전달 구조

이 프로젝트는 **4단계 계층 구조**로 복잡한 개념을 단순하게 전달합니다.

```
파인만 학습법 적용 아키텍처
├─ Layer 1: 개념 선택 (Concept Selection)
│  └─ 책임: 학습/전달할 핵심 개념 정의 (예: AlphaFold, 양자컴퓨팅)
│
├─ Layer 2: 단순화 엔진 (Simplification Engine)
│  └─ 책임: 전문 용어 → 일상 언어 변환, 비유 생성
│
├─ Layer 3: 검증 시스템 (Validation System)
│  └─ 책임: 파인만 테스트 실행 (5분 설명, 비전공자 이해도 측정)
│
└─ Layer 4: 출력 포맷 (Output Formats)
   └─ 책임: 문서, 피칭 스크립트, 교육 자료 생성
```

**Rationale**:
- **복잡도 제어**: 각 레이어가 명확한 단순화 책임을 가짐
- **검증 자동화**: Layer 3에서 "설명 가능성" 자동 검증
- **재사용성**: Layer 2의 단순화 엔진이 모든 개념에 적용 가능

## @DOC:MODULES-001 Module Responsibilities

### 1. 개념 선택 모듈 (Concept Selection Module)

- **Responsibilities**: 복잡한 생화학·AI 개념 중 학습/전달 대상 선정
- **Inputs**: 기존 로드맵 문서, 연구 자료, 유튜브 강의 등
- **Processing**:
  1. 핵심 개념 추출 (예: "단백질 접힘", "AlphaFold", "큐비트")
  2. 복잡도 평가 (전문 용어 수, 사전 지식 요구 수준)
  3. 우선순위 지정 (프로젝트 목표 연관도)
- **Outputs**: 개념 선택 리스트 (@SPEC:CONCEPT-XXX)

| Component           | Role             | Key Capabilities                     |
| ------------------- | ---------------- | ------------------------------------ |
| Concept Extractor   | 개념 추출기      | 문서에서 핵심 개념 자동 추출         |
| Complexity Analyzer | 복잡도 분석기    | 전문 용어 밀도, 사전 지식 요구도 평가 |
| Priority Ranker     | 우선순위 정렬기  | 프로젝트 목표 대비 중요도 순위 매김  |

### 2. 단순화 엔진 (Simplification Engine)

- **Responsibilities**: 전문 용어를 일상 언어로 변환, 구체적 비유 생성
- **Inputs**: 선택된 개념 (@SPEC:CONCEPT-XXX)
- **Processing**:
  1. 전문 용어 탐지 및 일상 언어 매핑 (예: "단백질 접힘" → "단백질이 자신의 모양을 찾아가는 과정")
  2. 비유 생성 (예: "단백질 접힘은 종이접기(origami)와 같다")
  3. 문장 단순화 (복문 → 단문, 20단어 이하)
- **Outputs**: 단순화된 설명 문서 (@DOC:SIMPLIFIED-XXX)

| Component            | Role             | Key Capabilities                         |
| -------------------- | ---------------- | ---------------------------------------- |
| Term Mapper          | 용어 변환기      | 전문 용어 → 일상 언어 자동 매핑           |
| Analogy Generator    | 비유 생성기      | 구체적 비유/예시 자동 생성                |
| Sentence Simplifier  | 문장 단순화기    | 복문 분해, 단어 수 제한 (< 20개)          |

### 3. 검증 시스템 (Validation System)

- **Responsibilities**: 파인만 테스트 실행 및 이해도 검증
- **Inputs**: 단순화된 설명 문서 (@DOC:SIMPLIFIED-XXX)
- **Processing**:
  1. 자동 복잡도 측정 (전문 용어 비율, 문장 길이)
  2. 인간 테스트 가이드 제공 ("비전공자에게 5분 설명")
  3. 이해도 점수 수집 (1~5점)
- **Outputs**: 검증 리포트 (@TEST:FEYNMAN-XXX), 재학습 필요 항목 리스트

| Component               | Role               | Key Capabilities                          |
| ----------------------- | ------------------ | ----------------------------------------- |
| Complexity Meter        | 복잡도 측정기      | 전문 용어 비율, 문장 길이 자동 측정       |
| Human Test Orchestrator | 인간 테스트 조율기 | 비전공자 테스트 가이드 제공               |
| Feedback Collector      | 피드백 수집기      | 이해도 점수 수집 및 개선 항목 추출        |

### 4. 출력 포맷 생성기 (Output Format Generator)

- **Responsibilities**: 검증된 내용을 다양한 포맷으로 변환
- **Inputs**: 검증 통과 문서 (@DOC:SIMPLIFIED-XXX)
- **Processing**:
  1. 마크다운 문서 생성
  2. 피칭 스크립트 생성 (5분 버전, 10분 버전)
  3. 교육 자료 생성 (슬라이드, 인포그래픽)
- **Outputs**: 다양한 포맷의 최종 문서 (@DOC:OUTPUT-XXX)

| Component          | Role              | Key Capabilities                    |
| ------------------ | ----------------- | ----------------------------------- |
| Markdown Generator | 마크다운 생성기   | 구조화된 기술 문서 생성             |
| Pitch Scripter     | 피칭 스크립터     | 시간별 피칭 스크립트 자동 생성      |
| Visual Converter   | 시각 자료 변환기  | 텍스트를 슬라이드/인포그래픽으로 변환 |

## @DOC:INTEGRATION-001 External Integrations

### [External System 1] Integration

- **Authentication**: [Method used]
- **Data Exchange**: [Formats and protocols]
- **Failure Handling**: [Fallback strategy]
- **Risk Level**: [Risk profile and mitigation]

### [External System 2] Integration

- **Purpose**: [Why it is used]
- **Dependency Level**: [Degree of reliance and alternatives]
- **Performance Requirements**: [Latency, throughput, etc.]

## @DOC:TRACEABILITY-001 Traceability Strategy

### Applying the TAG Framework

**Full TDD Alignment**: SPEC → Tests → Implementation → Documentation
- `@SPEC:ID` (`.moai/specs/`) → `@TEST:ID` (`tests/`) → `@CODE:ID` (`src/`) → `@DOC:ID` (`docs/`)

**Implementation Detail Levels**: Annotation within `@CODE:ID`
- `@CODE:ID:API` – REST APIs, GraphQL endpoints
- `@CODE:ID:UI` – Components, views, screens
- `@CODE:ID:DATA` – Data models, schemas, types
- `@CODE:ID:DOMAIN` – Business logic, domain rules
- `@CODE:ID:INFRA` – Infrastructure, databases, integrations

### Managing TAG Traceability (Code-Scan Approach)

- **Verification**: Run `/alfred:3-sync`, which scans with `rg '@(SPEC|TEST|CODE|DOC):' -n`
- **Coverage**: Full project source (`.moai/specs/`, `tests/`, `src/`, `docs/`)
- **Cadence**: Validate whenever the code changes
- **Code-First Principle**: TAG truth lives in the source itself

## Legacy Context

### Current System Snapshot

**[Describe the existing system or assets]**

```
Current System/
├── [Component 1]/     # [Current state]
├── [Component 2]/     # [Current state]
└── [Component 3]/     # [Current state]
```

### Migration Considerations

1. **[Migration item 1]** – [Plan and priority]
2. **[Migration item 2]** – [Plan and priority]
3. **[Migration item 3]** – [Plan and priority]

## TODO:STRUCTURE-001 Structural Improvements

1. **단순화 엔진 자동화** – NLP 기반 전문 용어 탐지 및 일상 언어 매핑 자동화
2. **파인만 테스트 프레임워크 구축** – 비전공자 이해도 측정 자동화 시스템
3. **출력 포맷 생성기 확장** – 피칭 스크립트, 슬라이드, 인포그래픽 자동 생성
4. **복잡도 측정 대시보드** – 전체 문서의 복잡도 지수 실시간 모니터링

## EARS for Architectural Requirements

### Applying EARS to Architecture

Use EARS patterns to write clear architectural requirements:

#### Architectural EARS Example
```markdown
### Ubiquitous Requirements (Baseline Architecture)
- The system shall adopt a layered architecture.
- The system shall maintain loose coupling across modules.

### Event-driven Requirements
- WHEN an external API call fails, the system shall execute fallback logic.
- WHEN a data change event occurs, the system shall notify dependent modules.

### State-driven Requirements
- WHILE the system operates in scale-out mode, it shall load new modules dynamically.
- WHILE in development mode, the system shall provide verbose debug information.

### Optional Features
- WHERE the deployment runs in the cloud, the system may use distributed caching.
- WHERE high performance is required, the system may apply in-memory caching.

### Constraints
- IF the security level is elevated, the system shall encrypt all inter-module communication.
- Each module shall keep cyclomatic complexity under 15.
```

---

_This structure informs the TDD implementation when `/alfred:2-run` runs._
