<div align="center">

[English](../README.md) · [한국어](README.ko.md) · [**中文**](README.zh-CN.md) · [日本語](README.ja.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [Español](README.es.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [हिन्दी](README.hi.md) · [العربية](README.ar.md)

# The AI Theorem

**面向可靠人机协作的规范化运行框架。**

[![Canon](https://img.shields.io/badge/canon-active%20development-blue)](https://github.com/the-ai-theorem/canon)
[![Vendor](https://img.shields.io/badge/vendor-neutral-success)]()
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](https://github.com/the-ai-theorem/canon/blob/main/LICENSE)

</div>

---

## 为什么选择 The AI Theorem

生成式 AI 与智能体正在迅速融入日常工作，但在多数组织里，每个人用的都是**各不相同的提示词、各不相同的工具，以及零散随意的知识**。同一项任务，产出质量参差不齐；标准与制度难以落地执行；更没有一条清晰的路径去核验智能体的产出，或为其结果追责。

The AI Theorem 要解决的**不是**「该向 AI 提什么问题」。它要定义的是 **AI 据以判断和行动的原则与标准**——把碎片化、个人化的 AI 实践，沉淀为**经过验证、可复用、覆盖全组织的运行标准**。

> 关键不在于更好的提示词，而在于一套人人与每个智能体都共享、且值得信赖的 **canon（规范）**——并持续验证真实产出是否切实遵循了它。

---

## 工作原理

组织把自身的架构原则、运行规则、安全制度、领域知识和质量标准，沉淀为一份 **Canon**——一个 Single Source of Truth——再将其投射到 Claude、Codex、ChatGPT、Cursor 及其他智能体实际运行的执行上下文中。

```
Canon  →  Format & Installer  →  Per-vendor / per-domain application  →  Installed copy (.theorem/)
doctrine     canon-kit              playbooks · canon-domains                  in your project
```

- **Canon** —— 组织已验证并批准的原则、规则、设计标准与工作标准。
- **Agent Context** —— Canon 被编译为各类智能体所消费的上下文与命令格式。
- **Workflow** —— 从构想 → 规划 → 构建 → 评审 → 批准 → 交付的标准化流程。
- **Validation** —— 核验 AI 产出是否符合 Canon 与制度，揪出偏差与违规。
- **Feedback Loop** —— 来自真实项目的新知识与例外，回流并沉淀进 Canon。

---

## 核心原则

| | |
|---|---|
| **Canon before Prompt** | 先定义组织的标准，再谈个人的提示词。 |
| **Context before Generation** | 在生成*之前*，先给足目的、约束、领域知识与验收标准。 |
| **Evidence before Trust** | 「这是 AI 做的」不足以构成信任的理由——证据、测试与评审才是。 |
| **Process before Output** | 管的是结果如何产生的过程，而不只是最终产物。 |
| **Organization over Individual** | 把个人技能转化为可复用的组织资产。 |
| **Vendor Neutrality** | 不绑定任何单一 AI 模型或供应商，保持独立。 |
| **Human Accountability** | AI 辅助判断与执行，决策由人负责。 |
| **Continuous Evolution** | Canon 是一套不断吸纳已验证经验的活系统。 |

---

## 生态体系

The AI Theorem 是一个**由独立仓库构成的生态体系**。中立内核（`canon`）既不指名、也不依赖任何同级仓库；一切都在安装时组合而成。

| Repository | Purpose | Status |
|---|---|---|
| [`canon`](https://github.com/the-ai-theorem/canon) | 公开稳定的方法论——供应商中立（有效性 · 令牌经济 · 性能 · 安全验证 · 人机协作） | **Active** |
| [`canon-kit`](https://github.com/the-ai-theorem/canon-kit) | 安装器 + 工具包格式标准与安装机制（一致性 · 信任 · 权限 · 覆盖） | Active |
| [`canon-lab`](https://github.com/the-ai-theorem/canon-lab) | 私有的编写 · 构建 · 认证工作区 | Private |
| [`canon-domains`](https://github.com/the-ai-theorem/canon-domains) | 领域模块——MES, ERP, Factory Vision, Pharma, Healthcare, …（供应商中立） | Planned |
| [`playbooks`](https://github.com/the-ai-theorem/playbooks) | 面向各供应商 / 各智能体的应用手册 + 真实工作流示例项目——Claude Code, Cursor, Codex, Gemini, …（领域中立） | Planned |
| [`community`](https://github.com/the-ai-theorem/community) | 集体知识与讨论——一个共享空间，让 AI 智能体的观点与经验与人类共同沉淀并相互验证 | Planned |

**两条正交的轴线——靠组合，而非继承。** 你*构建什么*（**领域**轴）与你*用哪个智能体*（**供应商**轴）都只继承自 `canon`，且彼此独立。安装器将**一个领域 × N 个供应商手册 → `.theorem/`** 组合到一起——因此无需再去维护一张 `vendor × domain` 矩阵。

---

## 适用对象

- **企业**——在全组织范围内落地 AI，同时守住质量、安全、一致性与问责。
- **CTO 与技术负责人**——在 AI 辅助开发中守护架构、代码质量与运行标准。
- **AI 治理负责人**——弥合 AI 制度与智能体实际行为之间的落差。
- **领域专家**——把隐性的专业经验转化为标准化、可被 AI 消费的资产。
- **智能体开发者**——需要在众多模型与工具间共享同一套上下文与执行规则。
- **咨询机构**——把一套可复用的方法论应用到每一个客户身上。

---

## 快速上手

canon **不会被直接安装**——它由安装器引导进入你的项目。

1. 通读方法论：**[`canon`](https://github.com/the-ai-theorem/canon)** → 从 [`OVERVIEW.md`](https://github.com/the-ai-theorem/canon/blob/main/OVERVIEW.md) 读起。
2. 通过 **[`canon-kit`](https://github.com/the-ai-theorem/canon-kit)** 安装——选定最新的 [release tag](https://github.com/the-ai-theorem/canon-kit/releases)，照着它的 Quick start 操作即可。

欢迎参与共建——新增或改进 canon 文档、领域模块、供应商手册、模板与示例。提交 issue 或 pull request 即可。

---

<div align="center">

**Canon before Prompt · Context before Generation · Evidence before Trust**

*供应商中立 · 由人负责 · 持续演进*

</div>
