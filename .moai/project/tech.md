---
id: TECH-001
version: 0.1.3
status: active
created: 2025-10-01
updated: 2025-11-06
author: @Alfred
priority: high
---

# roadmap Technology Stack

## HISTORY

### v0.1.3 (2025-11-06)
- **UPDATED**: Scholar version - maintain technical terms with explanations
- **AUTHOR**: @Alfred
- **SECTIONS**:
  - Updated @DOC:DOCUMENTATION-001 (복잡도 제한 규칙 - 전문 용어 유지 버전)
  - Updated 파인만 테스트 체크리스트 (학자 버전)
  - Updated 문서 작성 워크플로우 (학자 버전 - 7단계)
- **RATIONALE**: "전문 용어 유지 + 쉬운 설명 추가" 원칙 적용 (학자 요구사항 반영)

### v0.1.2 (2025-11-06)
- **UPDATED**: Feynman Learning Method integrated as documentation standard
- **AUTHOR**: @Alfred
- **SECTIONS**:
  - Added @DOC:DOCUMENTATION-001 (Feynman-based documentation standards)
  - Updated @DOC:STACK-001 (Markdown-focused project definition)
  - Updated @DOC:QUALITY-001 (Feynman Test coverage & complexity analysis)
  - Updated @CODE:TECH-DEBT-001 (4 documentation complexity improvement items)
- **RATIONALE**: Applied Feynman Test as quality gate for all technical documentation

### v0.1.1 (2025-10-17)
- **UPDATED**: Template version synced (v0.3.8)
- **AUTHOR**: @Alfred
- **SECTIONS**: Metadata standardization (single `author` field, added `priority`)

### v0.1.0 (2025-10-01)
- **INITIAL**: Authored the technology stack document
- **AUTHOR**: @tech-lead
- **SECTIONS**: Stack, Framework, Quality, Security, Deploy

---

## @DOC:DOCUMENTATION-001 파인만 학습법 기반 문서화 표준

> **핵심 원칙**: "초등학생도 이해할 수 있는 설명"이 모든 기술 문서의 기준

### 문서화 표준

이 프로젝트는 **파인만 학습법**을 문서화 표준으로 채택합니다. 모든 기술 문서는 다음 기준을 충족해야 합니다.

#### 1. 복잡도 제한 규칙 (전문 용어 유지 버전)

| 항목                  | 기준                         | 측정 방법                                |
| --------------------- | ---------------------------- | ---------------------------------------- |
| **전문 용어 사용**    | 유지 (정확성 최우선)          | 원문의 전문 용어는 그대로 유지           |
| **전문 용어 설명**    | 모든 전문 용어에 쉬운 설명 추가 | 괄호 또는 후속 문장으로 일상 언어 설명   |
| **문장 길이**         | < 30 단어 (설명 포함)         | 평균 문장당 단어 수 (전문 용어 + 설명)   |
| **단락 구조**         | 정의 → 쉬운 설명 → 비유       | 3단계 계층 구조                          |
| **비유/예시 비율**    | 핵심 개념당 최소 1개          | 추상 개념마다 구체적 비유 존재            |

#### 2. 파인만 테스트 체크리스트

모든 문서는 작성 후 다음 테스트를 통과해야 합니다:

✅ **필수 통과 조건 (학자 버전)**
- [ ] 전문 용어는 유지하되, 모든 용어에 쉬운 설명이 추가됨
- [ ] 비전공자가 "전문 용어의 의미"를 이해할 수 있음 (용어 자체를 외우지 않아도 됨)
- [ ] "왜?"라는 질문에 막힘없이 답변 가능
- [ ] 구체적 비유/예시로 추상 개념 전달 가능

❌ **재작성 필요 신호**
- "머리로는 아는데 설명이 안 돼"
- "이 부분은 복잡해서..." (회피)
- 전문 용어만 나열하고 설명 없음
- 비전공자가 "용어의 의미"를 이해 못 함 (이해도 3점 이하)

#### 3. 문서 작성 워크플로우 (학자 버전)

```
1. 초안 작성 (Draft)
   - 전문 용어는 정확하게 유지
   ↓
2. 전문 용어 식별 (Term Identification)
   - 모든 전문 용어에 마킹
   ↓
3. 설명 추가 (Add Explanations)
   - 각 전문 용어 뒤에 일상 언어 설명 추가
   - 형식: "전문용어(영문): 쉬운 설명"
   ↓
4. 비유 삽입 (Add Analogies)
   - 핵심 개념마다 구체적 비유 추가
   - 3단계 구조: 정의 → 쉬운 설명 → 비유
   ↓
5. 파인만 테스트 (Feynman Test)
   - 비전공자에게 "용어의 의미" 설명
   - 이해도 점수 수집 (1~5점)
   ↓
6. 피드백 반영 (Feedback)
   - 설명이 부족한 용어에 추가 설명
   - 비유가 필요한 개념에 비유 삽입
   ↓
7. 최종 승인 (Approval)
   - 모든 전문 용어에 설명 존재
   - 파인만 테스트 통과 (4점 이상)
```

#### 4. 자동화 도구

| 도구               | 용도                         | 기준                      |
| ------------------ | ---------------------------- | ------------------------- |
| Hemingway Editor   | 문장 복잡도 측정             | Grade 8 이하 (중학생 수준) |
| Grammarly          | 전문 용어 탐지 및 대안 제시  | Jargon count < 10%        |
| Custom Validator   | 파인만 테스트 체크리스트 검증 | 모든 항목 체크            |

## @DOC:STACK-001 Languages & Runtimes

### Primary Language

- **Language**: Markdown (문서화 중심 프로젝트)
- **Version Range**: CommonMark 표준
- **Rationale**: 복잡한 생화학·AI 개념을 단순하게 전달하는 연구 프로젝트이므로, 코드보다 문서화가 핵심
- **Package Manager**: N/A (문서 관리는 Git)

### Multi-Platform Support

| Platform    | Support Level | Validation Tooling  | Key Constraints |
| ----------- | ------------- | ------------------- | --------------- |
| **Windows** | [Supported?]  | [Validation method] | [Constraints]   |
| **macOS**   | [Supported?]  | [Validation method] | [Constraints]   |
| **Linux**   | [Supported?]  | [Validation method] | [Constraints]   |

## @DOC:FRAMEWORK-001 Core Frameworks & Libraries

### 1. Runtime Dependencies

```json
{
  "dependencies": {
    "[library1]": "[version]",
    "[library2]": "[version]",
    "[library3]": "[version]"
  }
}
```

### 2. Development Tooling

```json
{
  "devDependencies": {
    "[dev-tool1]": "[version]",
    "[dev-tool2]": "[version]",
    "[dev-tool3]": "[version]"
  }
}
```

### 3. Build System

- **Build Tool**: [Selected build tool]
- **Bundling**: [Bundler and configuration]
- **Targets**: [Build targets such as browser, Node.js, etc.]
- **Performance Goals**: [Desired build duration]

## @DOC:QUALITY-001 Quality Gates & Policies

### 파인만 테스트 Coverage

- **Target**: 모든 핵심 개념 문서가 파인만 테스트 통과 (이해도 4점 이상)
- **Measurement Tool**:
  - 자동: Hemingway Editor (Grade 8 이하)
  - 수동: 비전공자 5분 설명 테스트
- **Failure Response**:
  - 3점 이하: 전면 재작성 (전문 용어 제거, 비유 추가)
  - 3~4점: 부분 개선 (막히는 부분만 단순화)

### Static Analysis (문서 복잡도 분석)

| Tool             | Role                  | Config File        | Failure Handling                  |
| ---------------- | --------------------- | ------------------ | --------------------------------- |
| Hemingway Editor | 문장 복잡도 측정      | N/A (웹 기반)       | Grade 9 이상 시 문장 단순화 요구   |
| Grammarly        | 전문 용어 탐지        | N/A (웹 기반)       | Jargon 10% 초과 시 일상 언어 변환 |
| Custom Validator | 파인만 체크리스트 검증 | feynman-rules.yml  | 체크리스트 미통과 시 재작성       |

### Automation Scripts

```bash
# 파인만 학습법 기반 Quality gate pipeline
make feynman-check               # 복잡도 자동 측정 (Hemingway + Grammarly)
make simplify                    # 전문 용어 → 일상 언어 변환 제안
make human-test                  # 비전공자 테스트 가이드 출력
make validate                    # 파인만 체크리스트 검증
```

## @DOC:SECURITY-001 Security Policy & Operations

### Secret Management

- **Policy**: [Approach to handling secrets]
- **Tooling**: [Services or tools in use]
- **Verification**: [Automation to validate compliance]

### Dependency Security

```json
{
  "security": {
    "audit_tool": "[security-audit-tool]",
    "update_policy": "[update-policy]",
    "vulnerability_threshold": "[allowed-threshold]"
  }
}
```

### Logging Policy

- **Log Levels**: [Define log levels]
- **Sensitive Data Masking**: [Masking rules]
- **Retention Policy**: [Log retention period]

## @DOC:DEPLOY-001 Release Channels & Strategy

### 1. Distribution Channels

- **Primary Channel**: [Main release path]
- **Release Procedure**: [Deployment process]
- **Versioning Policy**: [Version management strategy]
- **Rollback Strategy**: [Rollback plan]

### 2. Developer Setup

```bash
# Developer mode setup
[local-install-command]
[dependency-install-command]
[dev-environment-command]
```

### 3. CI/CD Pipeline

| Stage     | Objective   | Tooling | Success Criteria |
| --------- | ----------- | ------- | ---------------- |
| [Stage 1] | [Objective] | [Tool]  | [Condition]      |
| [Stage 2] | [Objective] | [Tool]  | [Condition]      |
| [Stage 3] | [Objective] | [Tool]  | [Condition]      |

## Environment Profiles

### Development (`dev`)

```bash
export PROJECT_MODE=development
export LOG_LEVEL=debug
[dev-env-command]
```

### Test (`test`)

```bash
export PROJECT_MODE=test
export LOG_LEVEL=info
[test-env-command]
```

### Production (`production`)

```bash
export PROJECT_MODE=production
export LOG_LEVEL=warning
[prod-env-command]
```

## @CODE:TECH-DEBT-001 Technical Debt Management

### Current Debt (문서화 복잡도 개선 필요 항목)

1. **기존 Phase 1~4 로드맵 문서** – 전문 용어 과다, 파인만 테스트 미통과 (우선순위: 높음)
2. **AlphaFold 설명 문서 부재** – 핵심 기술에 대한 "쉬운 설명" 문서 없음 (우선순위: 높음)
3. **생화학 개념 용어집 부재** – 단백질 접힘, 효소 반응 등 기본 개념의 일상 언어 설명 없음 (우선순위: 중간)

### Remediation Plan

- **즉시 (1주)**: 기존 Phase 1 문서를 파인만 4단계로 재작성
- **단기 (1개월)**: AlphaFold, 양자컴퓨팅 핵심 개념의 "초등학생 설명" 버전 작성
- **중기 (3개월)**: 생화학 용어집 구축 (100개 핵심 용어 → 일상 언어 매핑)
- **장기 (6개월+)**: 자동화 도구 구축 (NLP 기반 전문 용어 탐지 및 단순화 제안)

## EARS Technical Requirements Guide

### Using EARS for the Stack

Apply EARS patterns when documenting technical decisions and quality gates:

#### Technology Stack EARS Example
```markdown
### Ubiquitous Requirements (Baseline)
- The system shall guarantee TypeScript type safety.
- The system shall provide cross-platform compatibility.

### Event-driven Requirements
- WHEN code is committed, the system shall run tests automatically.
- WHEN a build fails, the system shall notify developers immediately.

### State-driven Requirements
- WHILE in development mode, the system shall offer hot reloading.
- WHILE in production mode, the system shall produce optimized builds.

### Optional Features
- WHERE Docker is available, the system may support container-based deployment.
- WHERE CI/CD is configured, the system may execute automated deployments.

### Constraints
- IF a dependency vulnerability is detected, the system shall halt the build.
- Test coverage shall remain at or above 85%.
- Build time shall not exceed 5 minutes.
```

---

_This technology stack guides tool selection and quality gates when `/alfred:2-run` runs._
