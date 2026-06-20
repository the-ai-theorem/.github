<div align="center">

[**English**](README.md) · [한국어](i18n/README.ko.md) · [中文](i18n/README.zh-CN.md) · [日本語](i18n/README.ja.md) · [Deutsch](i18n/README.de.md) · [Français](i18n/README.fr.md) · [Español](i18n/README.es.md) · [Português](i18n/README.pt-BR.md) · [Русский](i18n/README.ru.md) · [Italiano](i18n/README.it.md) · [हिन्दी](i18n/README.hi.md) · [العربية](i18n/README.ar.md)

# The AI Theorem

**A canonical operating framework for reliable human–AI collaboration.**

[![Canon](https://img.shields.io/badge/canon-active%20development-blue)](https://github.com/the-ai-theorem/canon)
[![Vendor](https://img.shields.io/badge/vendor-neutral-success)]()
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](https://github.com/the-ai-theorem/canon/blob/main/LICENSE)

</div>

---

## Why The AI Theorem

Generative AI and agents are entering daily work fast — but in most organizations everyone uses **different prompts, different tools, and different ad-hoc knowledge**. The same task produces different quality, standards and policies go unenforced, and there is no clear way to verify or take responsibility for what an agent produced.

The AI Theorem is **not** a system for managing *what to ask* an AI. It is a system for defining **the principles and standards an AI should judge and act by** — turning fragmented, individual AI practice into a **verified, reusable, organization-wide operating standard**.

> The point is not better prompts. The point is a trustworthy **canon** that every person and every agent shares — and continuous verification that real output actually follows it.

---

## How it works

Organizations capture their architecture principles, operating rules, security policy, domain knowledge, and quality criteria as a **Canon** — a Single Source of Truth — and project it into the execution context that Claude, Codex, ChatGPT, Cursor, and other agents actually use.

```
Canon  →  Format & Installer  →  Per-vendor / per-domain application  →  Installed copy (.theorem/)
doctrine     canon-kit              playbooks · canon-domains                  in your project
```

- **Canon** — the principles, rules, design criteria, and work standards an organization has verified and approved.
- **Agent Context** — Canon compiled into the context and command formats different agents consume.
- **Workflow** — standardized procedures from idea → plan → build → review → approve → ship.
- **Validation** — checks whether AI output conforms to Canon and policy, surfacing drift and violations.
- **Feedback Loop** — new knowledge and exceptions from real projects flow back into Canon.

---

## Core principles

| | |
|---|---|
| **Canon before Prompt** | Define the organization's standard before individual prompts. |
| **Context before Generation** | Provide purpose, constraints, domain knowledge, and acceptance criteria *before* generating. |
| **Evidence before Trust** | "An AI made it" is not a reason to trust it — evidence, tests, and review are. |
| **Process before Output** | Manage how a result is produced, not just the final artifact. |
| **Organization over Individual** | Turn individual skill into reusable organizational assets. |
| **Vendor Neutrality** | Stay independent of any single AI model or provider. |
| **Human Accountability** | AI supports judgment and execution; people own the decisions. |
| **Continuous Evolution** | Canon is a living system that absorbs verified experience. |

---

## Ecosystem

The AI Theorem is an **ecosystem of independent repositories**. The neutral core (`canon`) names no sibling and depends on none; everything composes at install time.

| Repository | Purpose | Status |
|---|---|---|
| [`canon`](https://github.com/the-ai-theorem/canon) | Public stable doctrine — vendor-neutral methodology (effectiveness · token economy · performance · security verification · human–AI collaboration) | **Active** |
| [`canon-kit`](https://github.com/the-ai-theorem/canon-kit) | Installer + tool-package format standard & install mechanism (conformance · trust · permission · override) | Active |
| [`canon-lab`](https://github.com/the-ai-theorem/canon-lab) | Private authoring · build · certification workspace | Private |
| [`canon-domains`](https://github.com/the-ai-theorem/canon-domains) | Domain modules — MES, ERP, Factory Vision, Pharma, Healthcare, … (vendor-neutral) | Planned |
| [`playbooks`](https://github.com/the-ai-theorem/playbooks) | Per-vendor / per-agent application playbooks + real-workflow example projects — Claude Code, Cursor, Codex, Gemini, … (domain-neutral) | Planned |
| [`community`](https://github.com/the-ai-theorem/community) | Collective knowledge & discussion — a shared space where AI agents' opinions and experience are accumulated and verified together with humans | Planned |

**Two orthogonal axes — compose, don't inherit.** *What* you build (the **domain** axis) and *which agent* you use (the **vendor** axis) inherit `canon` only and stay independent. The installer composes **one domain × N vendor playbooks → `.theorem/`** — so there is no `vendor × domain` matrix to maintain.

---

## Who it's for

- **Enterprises** adopting AI org-wide while keeping quality, security, consistency, and accountability.
- **CTOs & tech leaders** preserving architecture, code quality, and operating standards in AI-assisted development.
- **AI governance owners** closing the gap between AI policy and what agents actually do.
- **Domain experts** turning tacit expertise into standardized, AI-consumable assets.
- **Agent developers** needing one shared context and execution ruleset across many models and tools.
- **Consultancies** applying a repeatable methodology per client.

---

## Get started

The canon is **not installed directly** — it is bootstrapped into a project by the installer.

1. Read the doctrine: **[`canon`](https://github.com/the-ai-theorem/canon)** → start with [`OVERVIEW.md`](https://github.com/the-ai-theorem/canon/blob/main/OVERVIEW.md).
2. Install via **[`canon-kit`](https://github.com/the-ai-theorem/canon-kit)** — pick the latest [release tag](https://github.com/the-ai-theorem/canon-kit/releases) and follow its Quick start.

Contributions are welcome — new or improved canon documents, domain modules, vendor playbooks, templates, and examples. Open an issue or a pull request.

---

<div align="center">

**Canon before Prompt · Context before Generation · Evidence before Trust**

*Vendor-neutral · Human-accountable · Continuously evolving*

</div>
