---
id: PRODUCT-001
version: 0.1.5
status: active
created: 2025-10-01
updated: 2025-11-06
author: @Alfred
priority: high
---

# roadmap Product Definition

## HISTORY

### v0.1.5 (2025-11-06)
- **UPDATED**: Added scientific validation for quantum computing in drug discovery
- **AUTHOR**: @Alfred
- **SECTIONS**:
  - Added @DOC:QUANTUM-001 (2022-2025 peer-reviewed papers validation)
  - Nature Biotechnology 2025: KRAS inhibitor discovery (15 molecules synthesized, 2 validated)
  - Scientific Reports 2024: Hybrid quantum computing pipeline (Gibbs free energy, prodrug activation)
  - Industry case studies: AstraZeneca, Moderna, Boehringer, Amgen, 한림제약, 연세대
  - Market outlook: $1B by 2025 (McKinsey), timeline 2025-2030 practical deployment
  - Added 5 references (Nature Biotech, Sci Reports, J Chem Theory Comput, Chem Reviews, McKinsey)
- **RATIONALE**: Address scientific credibility gap with recent (2022-2025) peer-reviewed evidence and real-world pharmaceutical applications

### v0.1.4 (2025-11-06)
- **UPDATED**: Feynman Learning Method integrated as core methodology
- **AUTHOR**: @Alfred
- **SECTIONS**:
  - Added @DOC:LEARNING-001 (Feynman Technique 4-step framework)
  - Updated @SPEC:USER-001 (defined primary/secondary audiences)
  - Updated @SPEC:PROBLEM-001 (3 high-priority problems with Feynman principles)
  - Updated @DOC:STRATEGY-001 (Feynman + Sinek dual strategy)
  - Updated @SPEC:SUCCESS-001 (Feynman Test KPIs)
  - Updated TODO:SPEC-BACKLOG-001 (3 concrete SPEC candidates)
- **RATIONALE**: Applied Feynman's principle "If you can't explain it simply, you don't understand it well enough"

### v0.1.3 (2025-10-17)
- **UPDATED**: Template version synced (v0.3.8)
- **AUTHOR**: @Alfred
- **SECTIONS**: Mission (finalized team of 12 agents: Alfred + 11 specialists)
  - Added implementation-planner, tdd-implementer, quality-gate
  - Split code-builder into implementation-planner + tdd-implementer + quality-gate

### v0.1.2 (2025-10-17)
- **UPDATED**: Agent count adjusted (9 → 11)
- **AUTHOR**: @Alfred
- **SECTIONS**: Mission (updated Alfred SuperAgent roster)

### v0.1.1 (2025-10-17)
- **UPDATED**: Template defaults aligned with the real MoAI-ADK project
- **AUTHOR**: @Alfred
- **SECTIONS**: Mission, User, Problem, Strategy, Success populated with project context

### v0.1.0 (2025-10-01)
- **INITIAL**: Authored the product definition document
- **AUTHOR**: @project-owner
- **SECTIONS**: Mission, User, Problem, Strategy, Success, Legacy

---

## @DOC:MISSION-001 Core Mission

> **"No SPEC, no CODE."**

roadmap combats Frankenstein code at the root by enforcing a **SPEC-first TDD methodology**.

### Core Value Proposition

#### Four Key Values

1. **Consistency**: A three-step SPEC → TDD → Sync pipeline safeguards delivery quality.
2. **Quality**: TRUST principles (Test First, Readable, Unified, Secured, Trackable) apply automatically.
3. **Traceability**: The @TAG system (`@SPEC → @TEST → @CODE → @DOC`) preserves end-to-end lineage.
4. **Universality**: Supports diverse programming languages and frameworks.

#### Alfred SuperAgent

**Alfred** coordinates a team of 12 AI agents (Alfred + 11 specialists):
- **spec-builder** 🏗️: Authors SPECs (EARS pattern) – Sonnet
- **implementation-planner** 📋: Analyzes SPECs and derives implementation plans – Sonnet
- **tdd-implementer** 🔬: Executes RED–GREEN–REFACTOR cycles – Sonnet
- **quality-gate** 🛡️: Enforces TRUST principles – Haiku
- **doc-syncer** 📖: Maintains living documentation – Haiku
- **tag-agent** 🏷️: Manages the TAG system – Haiku
- **git-manager** 🚀: Automates Git workflows – Haiku
- **debug-helper** 🔍: Diagnoses runtime issues – Sonnet
- **trust-checker** ✅: Verifies TRUST compliance – Haiku
- **cc-manager** 🛠️: Configures Claude Code – Sonnet
- **project-manager** 📂: Bootstraps projects – Sonnet

## @DOC:LEARNING-001 파인만 학습법 (Feynman Technique)

> **"간단히 설명할 수 없다면, 제대로 이해하지 못한 것이다"** - Richard Feynman

### 핵심 원칙

이 프로젝트는 **파인만 학습법**을 핵심 방법론으로 채택하여, 복잡한 생화학·AI·양자컴퓨팅 개념을 누구나 이해할 수 있도록 단순화합니다.

#### 파인만 학습법 4단계

1. **개념 선택 (Choose a Concept)**
   - 이해하고 싶은 복잡한 개념을 명확히 정의
   - 예: AlphaFold의 단백질 구조 예측 원리, 양자컴퓨팅의 큐비트 중첩 상태

2. **강의용 스크립트 작성 (Teach It to a Child)**
   - 초등학생에게 설명하듯 쉽게 작성
   - 모호한 표현과 전문 용어 발견 → 이해 부족 영역 식별

3. **재학습 (Identify Gaps and Go Back)**
   - 설명이 막히는 부분을 다시 학습
   - 출처 자료를 재검토하고 개념을 재정립

4. **단순화 및 비유 (Simplify and Use Analogies)**
   - 복잡한 개념을 일상적 비유로 전환
   - 예: "단백질 접힘은 종이접기(origami)와 같다"

### 적용 전략

| 영역                  | 파인만 학습법 적용                                                  |
| --------------------- | ------------------------------------------------------------------- |
| **생화학 개념 학습**  | 효소 반응, 유전자 발현 등을 일상 언어로 설명                        |
| **AI 모델 이해**      | AlphaFold, 강화학습을 비전공자도 이해 가능한 수준으로 단순화        |
| **양자컴퓨팅 원리**   | 큐비트, 양자 얽힘을 물리학 비전공자에게 설명 가능한 수준으로 변환   |
| **로드맵 설명**       | 36개월 로드맵의 각 단계를 투자자/협력자에게 5분 안에 설명 가능하게 |
| **문서화 표준**       | 모든 기술 문서는 "초등학생 테스트" 통과 기준 적용                   |

### 검증 기준

✅ **파인만 테스트 통과 조건**
- [ ] 비전공자(예: 인문계 친구)에게 5분 안에 핵심 개념 설명 가능
- [ ] 전문 용어 없이 일상 언어로 설명 가능
- [ ] 질문에 막힘없이 답변 가능
- [ ] 구체적 비유/예시로 추상 개념 전달 가능

❌ **재학습 필요 신호**
- "머리로는 아는데 설명이 안 돼"
- "이 부분은 복잡해서..." (회피)
- 전문 용어에 의존하여 설명
- 질문에 답변 막힘

## @SPEC:USER-001 Primary Users

### Primary Audience
- **Who**: 생화학 지식을 활용한 헬스케어 앱 개발자 및 연구자
- **Core Needs**: AI·양자컴퓨팅을 활용한 신약 개발 로드맵 이해 및 실행
- **Critical Scenarios**: AlphaFold 기반 단백질 구조 예측, 웨어러블 연동 헬스케어 앱 개발

### Secondary Audience
- **Who**: 투자자, 협력 연구기관, 기술 파트너
- **Needs**: 프로젝트의 기술적 타당성과 비즈니스 가치를 명확히 이해

## @SPEC:PROBLEM-001 Problems to Solve

### High Priority
1. **복잡한 생화학·AI 개념의 접근성 장벽**
   - 문제: 단백질 접힘, AlphaFold, 양자컴퓨팅 등 고도의 전문 지식이 필요한 개념들이 비전공자에게 이해 불가능
   - 파인만 원칙 적용: 모든 개념을 "초등학생도 이해 가능한 수준"으로 단순화

2. **36개월 로드맵의 실행 가능성 검증 부족**
   - 문제: Phase 1~4 로드맵이 이론적으로만 존재하며, 각 단계의 실행 가능성이 명확하지 않음
   - 파인만 원칙 적용: 각 Phase를 "투자자에게 5분 안에 설명 가능한" 수준으로 구조화

3. **기술 문서의 과도한 전문 용어**
   - 문제: 기존 로드맵 문서들이 전문 용어로 가득 차 있어, 협력자/투자자 이해 어려움
   - 파인만 원칙 적용: "일상 언어 + 구체적 비유"로 재작성

---

## @DOC:QUANTUM-001 양자컴퓨팅 신약 개발 과학적 근거 (2022-2025 검증)

> **핵심 질문**: "양자컴퓨팅이 신약 개발에 실제로 활용되고 있는가?"
> **답변**: 예. 2024-2025년 주요 논문과 산업 사례가 이를 입증합니다.

### 최신 연구 성과 (Peer-Reviewed Papers)

#### 1. Nature Biotechnology (2025년 1월): KRAS 저해제 발견
- **논문**: "Quantum-computing-enhanced algorithm unveils potential KRAS inhibitors"
- **저자**: Insilico Medicine + University of Toronto 공동연구팀
- **방법론**: 양자-고전 혼합 생성 모델 (Quantum Circuit Born Machines + LSTM)
- **데이터셋**: 110만 개 분자 학습 (KRAS 저해 실험 검증 분자 650개 포함)

**구체적 성과**:
- 설계된 분자: 15개 합성 완료
- 실험 검증 성공: 2개 (ISM061-018-2, ISM061-022)
- 결합 친화도: 마이크로몰 수준 (SPR assay 측정)
- 임상 의의: KRAS G12D/G12C/G12V 다중 변이 표적 가능 (pan-KRAS 저해제)

**쉬운 설명**: KRAS는 암세포의 성장 스위치 역할을 하는 단백질로, 기존에는 "약으로 막을 수 없는 표적(undruggable target)"으로 여겨졌습니다. 양자컴퓨터는 110만 개의 분자 중에서 KRAS에 딱 맞는 열쇠(저해제)를 찾아냈고, 실제로 실험실에서 만들어 암세포에 작동하는지 확인했습니다.

#### 2. Scientific Reports (2024년 7월): 실전 신약 개발 파이프라인
- **논문**: "A hybrid quantum computing pipeline for real world drug discovery"
- **발행**: Nature Scientific Reports, 2024년 7월 23일
- **DOI**: 10.1038/s41598-024-67897-8

**연구 내용**:
1. **프로드러그 활성화 연구**
   - Gibbs 자유 에너지 프로파일 계산 (탄소-탄소 결합 절단)
   - 반응 장벽과 에너지 변화가 기존 실험/이론 연구와 일치

2. **공유결합 저해제 시뮬레이션**
   - KRAS(G12C) 공유결합 저해제 분석 (QM/MM 시뮬레이션)
   - 양자컴퓨터 vs 고전컴퓨터 시간 비교 분석

**쉬운 설명**: 약은 몸속에서 활성화되어야 효과를 발휘합니다. 양자컴퓨터는 약이 활성화될 때 필요한 에너지(Gibbs 자유 에너지)를 정확히 계산해서, 어떤 약이 몸속에서 잘 작동할지 미리 예측할 수 있습니다. 마치 레고 블록이 맞물리는 데 필요한 힘을 계산하는 것과 같습니다.

### 산업 적용 사례 (2022-2024)

| 제약사               | 파트너사              | 연구 분야                  | 연도  | 성과                                    |
| -------------------- | --------------------- | -------------------------- | ----- | --------------------------------------- |
| **AstraZeneca**      | AWS, IonQ, NVIDIA     | 소분자 약물 합성 반응      | 2024  | 양자 가속 화학 워크플로우 시연          |
| **Boehringer**       | PsiQuantum            | 금속효소 전자구조 계산     | 2023  | 약물 대사 핵심 효소 분석                |
| **Amgen**            | Quantinuum            | 펩타이드 결합 연구         | 2023  | 양자컴퓨팅 펩타이드 결합 시뮬레이션     |
| **IBM + Moderna**    | IBM Quantum           | mRNA 서열 시뮬레이션       | 2023  | 하이브리드 양자-고전 mRNA 설계          |
| **Biogen**           | 1QBit                 | 신경질환 분자 비교         | 2023  | 알츠하이머/파킨슨병 약물 후보 탐색 가속 |
| **한림제약 (한국)**  | IBM Quantum Network   | 천연물 신약 개발           | 2023  | 양자컴퓨팅 기반 신약 후보 도출          |
| **연세대-리가켐바이오** | IBM (127큐비트 시스템) | 항체-약물 접합체(ADC) 개발 | 2024  | 2025년 논문 발표 예정                   |

### 현재 한계와 미래 전망

**현재 제약사항**:
- VQE(Variational Quantum Eigensolver) 정확도 개선 필요
- 계산 자원 소비 최적화 필요
- 큐비트 수와 오류율 개선 필요

**시장 전망**:
- 생명과학 분야 양자컴퓨팅 시장: 2025년 10억 달러 규모 예상 (McKinsey)
- 신약 개발 비용 절감: 수백만 번의 R&D 사이클을 수천 번으로 단축 가능
- 타임라인: 2025-2030년 실용화 본격 시작

**쉬운 설명**: 양자컴퓨터는 아직 "개발 중인 도구"입니다. 마치 초기 인터넷처럼, 기술은 작동하지만 아직 완벽하지 않습니다. 그러나 AstraZeneca, Moderna 같은 글로벌 제약사들이 이미 실제 신약 개발에 사용하고 있고, 한국에서도 연세대와 한림제약이 연구를 시작했습니다.

### 참고문헌 (2022-2025)

1. **Nature Biotechnology (2025)**: Quantum-computing-enhanced algorithm unveils potential KRAS inhibitors. DOI: 10.1038/s41587-024-02526-3
2. **Scientific Reports (2024)**: A hybrid quantum computing pipeline for real world drug discovery. DOI: 10.1038/s41598-024-67897-8
3. **J. Chem. Theory Comput. (2022)**: Perspective on the Current State-of-the-Art of Quantum Computing for Drug Discovery Applications. DOI: 10.1021/acs.jctc.2c00574
4. **Chemical Reviews (2025)**: Quantum Machine Learning in Drug Discovery: Applications in Academia and Pharmaceutical Industries. DOI: 10.1021/acs.chemrev.4c00678
5. **McKinsey (2024)**: The quantum revolution in pharma: Faster, smarter, and more precise

---

### Medium Priority
- 생화학·AI·웨어러블 세 영역의 통합 전략 명확화
- AlphaFold 기반 신약 개발의 실제 사례 연구 부족

### Current Failure Cases
- **기존 연구 문서**: 전문가 중심 작성으로, 비전공자 접근 불가
- **로드맵 설명**: 추상적 개념 나열로, 실행 단계가 불명확
- **기술 문서**: "머리로는 아는데 설명이 안 되는" 상태

## @DOC:STRATEGY-001 Differentiators & Strengths

### Strengths Versus Alternatives
1. **파인만 학습법 기반 지식 전달 체계**
   - **차별점**: 복잡한 생화학·AI 개념을 "누구나 이해 가능한" 수준으로 단순화
   - **When it matters**: 투자 유치, 협력 연구기관 설득, 팀원 온보딩 시 5분 안에 핵심 전달 가능

2. **Simon Sinek의 지속적 질문 + 파인만의 단순화**
   - **차별점**: 복잡한 개념을 "왜?"로 파고들며(Sinek), "쉽게"로 전달(Feynman)하는 이중 전략
   - **When it matters**: 연구 방향 설정 시 본질 파악, 외부 커뮤니케이션 시 명확한 전달
   - **예시**: "왜 AlphaFold가 중요한가?" → "단백질 구조 예측" → "단백질은 생명의 레고 블록, 구조를 알면 신약 설계 가능"

## @SPEC:SUCCESS-001 Success Metrics

### Immediately Measurable KPIs
1. **파인만 테스트 통과율**
   - **Baseline**: 모든 핵심 개념 문서가 "비전공자 5분 설명" 테스트 통과
   - **측정 방법**: 인문계 친구/가족에게 설명 후 이해도 확인 (1~5점)

2. **문서 복잡도 지수**
   - **Baseline**: 전문 용어 비율 < 10%, 문장당 단어 수 < 20개
   - **측정 방법**: 자동화 도구로 문서 분석 (예: Hemingway Editor)

3. **로드맵 실행 가능성 점수**
   - **Baseline**: Phase 1~4 각 단계가 "구체적 액션 아이템"으로 분해됨
   - **측정 방법**: 각 Phase당 최소 5개 이상의 실행 가능한 태스크 존재

### Measurement Cadence
- **매 문서 작성 시**: 파인만 테스트 즉시 실행
- **Weekly**: 문서 복잡도 지수 측정 및 단순화 작업
- **Monthly**: 전체 로드맵 실행 가능성 재평가

## Legacy Context

### Existing Assets
- [Reusable assets or resources]
- [Relevant past projects or experience]

## TODO:SPEC-BACKLOG-001 Next SPEC Candidates

1. **SPEC-001**: 파인만 학습법 적용 - Phase 1 로드맵 단순화
   - 기존 Phase 1 문서를 파인만 4단계로 재작성
   - 전문 용어를 일상 언어로 변환
   - 비전공자 5분 설명 테스트 통과

2. **SPEC-002**: AlphaFold 개념 설명 문서 작성
   - "단백질 구조 예측"을 초등학생도 이해 가능한 수준으로 설명
   - 구체적 비유 사용 (예: 레고 블록, 종이접기)
   - YouTube 영상 스크립트 형태로 작성

3. **SPEC-003**: 36개월 로드맵 실행 가능성 검증
   - Phase 1~4 각 단계를 구체적 액션 아이템으로 분해
   - 각 Phase의 "완료 조건"을 파인만 테스트로 정의
   - 투자자용 5분 피칭 스크립트 작성

## EARS Requirement Authoring Guide

### EARS (Easy Approach to Requirements Syntax)

Use these EARS patterns to keep SPEC requirements structured:

#### EARS Patterns
1. **Ubiquitous Requirements**: The system shall provide [capability].
2. **Event-driven Requirements**: WHEN [condition], the system shall [behaviour].
3. **State-driven Requirements**: WHILE [state], the system shall [behaviour].
4. **Optional Features**: WHERE [condition], the system may [behaviour].
5. **Constraints**: IF [condition], the system shall enforce [constraint].

#### Sample Application
```markdown
### Ubiquitous Requirements (Foundational)
- The system shall provide user management capabilities.

### Event-driven Requirements
- WHEN a user signs up, the system shall send a welcome email.

### State-driven Requirements
- WHILE a user remains logged in, the system shall display a personalized dashboard.

### Optional Features
- WHERE an account is premium, the system may offer advanced features.

### Constraints
- IF an account is locked, the system shall reject login attempts.
```

---

_This document serves as the baseline when `/alfred:1-plan` runs._
