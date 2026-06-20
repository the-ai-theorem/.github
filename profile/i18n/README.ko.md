<div align="center">

[English](../README.md) · [**한국어**](README.ko.md) · [中文](README.zh-CN.md) · [日本語](README.ja.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [Español](README.es.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [हिन्दी](README.hi.md) · [العربية](README.ar.md)

# The AI Theorem

**신뢰할 수 있는 인간–AI 협업을 위한 정전(canonical) 운영 프레임워크.**

[![Canon](https://img.shields.io/badge/canon-active%20development-blue)](https://github.com/the-ai-theorem/canon)
[![Vendor](https://img.shields.io/badge/vendor-neutral-success)]()
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](https://github.com/the-ai-theorem/canon/blob/main/LICENSE)

</div>

---

## The AI Theorem이 필요한 이유

생성형 AI와 에이전트가 일상 업무 속으로 빠르게 들어오고 있지만, 대부분의 조직에서는 구성원마다 **제각각의 프롬프트, 제각각의 도구, 제각각의 임시 지식**에 의존합니다. 같은 작업을 해도 결과물의 품질이 들쭉날쭉하고, 표준과 정책은 실제로 적용되지 않으며, 에이전트가 내놓은 결과를 검증하거나 그 책임을 가릴 명확한 방법도 없습니다.

The AI Theorem은 AI에게 *무엇을 물어볼지*를 관리하는 시스템이 **아닙니다**. **AI가 따라야 할 판단과 행동의 원칙·표준**을 정의하는 시스템으로, 개인 단위로 흩어진 AI 활용을 **검증을 거쳐 재사용할 수 있는 전사 차원의 운영 표준**으로 바꿔 놓습니다.

> 관건은 더 나은 프롬프트가 아닙니다. 모든 구성원과 모든 에이전트가 공유하는 신뢰할 수 있는 **canon**, 그리고 실제 산출물이 그 canon을 제대로 따르고 있는지에 대한 지속적인 검증이 관건입니다.

---

## 작동 방식

조직은 자사의 아키텍처 원칙, 운영 규칙, 보안 정책, 도메인 지식, 품질 기준을 **Canon** — Single Source of Truth — 으로 담아내고, 이를 Claude, Codex, ChatGPT, Cursor를 비롯한 에이전트가 실제로 사용하는 실행 컨텍스트로 투영합니다.

```
Canon  →  Format & Installer  →  Per-vendor / per-domain application  →  Installed copy (.theorem/)
doctrine     canon-kit              playbooks · canon-domains                  in your project
```

- **Canon** — 조직이 검증하고 승인한 원칙, 규칙, 설계 기준, 작업 표준.
- **Agent Context** — 에이전트마다 소비하는 컨텍스트 및 명령 형식에 맞춰 컴파일된 Canon.
- **Workflow** — 아이디어 → 계획 → 빌드 → 검토 → 승인 → 배포로 이어지는 표준화된 절차.
- **Validation** — AI 산출물이 Canon과 정책에 부합하는지 확인해 드리프트와 위반을 드러냄.
- **Feedback Loop** — 실제 프로젝트에서 얻은 새로운 지식과 예외가 다시 Canon으로 환류됨.

---

## 핵심 원칙

| | |
|---|---|
| **Canon before Prompt** | 개별 프롬프트에 앞서 조직의 표준부터 정의합니다. |
| **Context before Generation** | 생성하기 *전에* 목적, 제약, 도메인 지식, 수용 기준을 먼저 제공합니다. |
| **Evidence before Trust** | "AI가 만들었다"는 사실은 신뢰의 근거가 되지 못합니다 — 증거와 테스트, 검토가 근거입니다. |
| **Process before Output** | 최종 산출물만이 아니라 그 결과가 만들어지는 과정까지 관리합니다. |
| **Organization over Individual** | 개인의 역량을 재사용 가능한 조직의 자산으로 전환합니다. |
| **Vendor Neutrality** | 특정 AI 모델이나 공급자에 종속되지 않고 독립성을 유지합니다. |
| **Human Accountability** | AI는 판단과 실행을 거들 뿐, 결정의 책임은 사람이 집니다. |
| **Continuous Evolution** | Canon은 검증된 경험을 흡수하며 성장하는 살아 있는 시스템입니다. |

---

## 생태계

The AI Theorem은 **독립된 저장소들로 이루어진 생태계**입니다. 중립적 코어인 `canon`은 어떤 형제 저장소도 특정하지 않고 어디에도 의존하지 않으며, 모든 구성 요소는 설치 시점에 비로소 조합됩니다.

| Repository | Purpose | Status |
|---|---|---|
| [`canon`](https://github.com/the-ai-theorem/canon) | 공개된 안정적 doctrine — 공급자 중립 방법론 (효과성 · 토큰 경제 · 성능 · 보안 검증 · 인간–AI 협업) | **Active** |
| [`canon-kit`](https://github.com/the-ai-theorem/canon-kit) | 설치 프로그램 + 도구 패키지 형식 표준 및 설치 메커니즘 (적합성 · 신뢰 · 권한 · 재정의) | Active |
| [`canon-lab`](https://github.com/the-ai-theorem/canon-lab) | 비공개 저작 · 빌드 · 인증 작업 공간 | Private |
| [`canon-domains`](https://github.com/the-ai-theorem/canon-domains) | 도메인 모듈 — MES, ERP, Factory Vision, Pharma, Healthcare, … (공급자 중립) | Planned |
| [`playbooks`](https://github.com/the-ai-theorem/playbooks) | 공급자별 / 에이전트별 적용 플레이북 + 실제 워크플로 예제 프로젝트 — Claude Code, Cursor, Codex, Gemini, … (도메인 중립) | Planned |
| [`community`](https://github.com/the-ai-theorem/community) | 집단 지식 · 토론 — AI 에이전트의 의견과 경험을 인간과 함께 축적하고 검증하는 공유 공간 | Planned |

**두 개의 직교 축 — 상속하지 말고 조합하라.** *무엇*을 만드는가(**도메인** 축)와 *어떤 에이전트*를 쓰는가(**공급자** 축)는 오직 `canon`만 상속할 뿐 서로 독립적으로 유지됩니다. 설치 프로그램이 **도메인 하나 × 공급자 플레이북 N개 → `.theorem/`** 로 조합하므로, 따로 유지보수해야 할 `vendor × domain` 행렬이 생기지 않습니다.

---

## 대상 사용자

- **기업** — 품질, 보안, 일관성, 책임성을 지키면서 조직 전반에 AI를 도입하려는 곳.
- **CTO 및 기술 리더** — AI 지원 개발에서도 아키텍처, 코드 품질, 운영 표준을 지켜내려는 분.
- **AI 거버넌스 담당자** — AI 정책과 에이전트의 실제 동작 사이의 간극을 메우려는 분.
- **도메인 전문가** — 암묵적 전문성을 표준화된, AI가 활용 가능한 자산으로 바꾸려는 분.
- **에이전트 개발자** — 여러 모델과 도구에 걸쳐 공유 컨텍스트와 실행 규칙을 하나로 통일하려는 분.
- **컨설팅 기업** — 고객사마다 반복 적용할 수 있는 방법론이 필요한 곳.

---

## 시작하기

canon은 **직접 설치하는 것이 아닙니다** — 설치 프로그램이 프로젝트에 부트스트랩합니다.

1. doctrine 읽기: **[`canon`](https://github.com/the-ai-theorem/canon)** → [`OVERVIEW.md`](https://github.com/the-ai-theorem/canon/blob/main/OVERVIEW.md)부터 시작하세요.
2. **[`canon-kit`](https://github.com/the-ai-theorem/canon-kit)** 으로 설치 — 최신 [release tag](https://github.com/the-ai-theorem/canon-kit/releases)를 선택해 해당 Quick start를 따르세요.

기여는 언제나 환영합니다 — 새롭거나 개선된 canon 문서, 도메인 모듈, 공급자 플레이북, 템플릿, 예제 무엇이든 좋습니다. 이슈나 풀 리퀘스트를 열어 주세요.

---

<div align="center">

**Canon before Prompt · Context before Generation · Evidence before Trust**

*공급자 중립 · 인간이 책임지는 · 지속적으로 진화하는*

</div>
