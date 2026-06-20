<div align="center">

[English](../README.md) · [한국어](README.ko.md) · [中文](README.zh-CN.md) · [日本語](README.ja.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [Español](README.es.md) · [**Português**](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [हिन्दी](README.hi.md) · [العربية](README.ar.md)

# The AI Theorem

**Um framework operacional canônico para uma colaboração humano–IA confiável.**

[![Canon](https://img.shields.io/badge/canon-active%20development-blue)](https://github.com/the-ai-theorem/canon)
[![Vendor](https://img.shields.io/badge/vendor-neutral-success)]()
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](https://github.com/the-ai-theorem/canon/blob/main/LICENSE)

</div>

---

## Por que The AI Theorem

A IA generativa e os agentes estão entrando rapidamente no dia a dia do trabalho — mas, na maioria das organizações, cada pessoa usa **prompts diferentes, ferramentas diferentes e conhecimento improvisado diferente**. A mesma tarefa gera qualidade desigual, padrões e políticas deixam de ser aplicados e não há uma forma clara de verificar o que um agente produziu nem de responsabilizar-se por isso.

The AI Theorem **não** é um sistema para gerenciar *o que perguntar* a uma IA. É um sistema para definir **os princípios e padrões pelos quais uma IA deve julgar e agir** — convertendo a prática de IA fragmentada e individual em um **padrão operacional verificado, reutilizável e válido para toda a organização**.

> O objetivo não são prompts melhores. O objetivo é um **canon** confiável, compartilhado por cada pessoa e cada agente — e a verificação contínua de que o resultado real de fato o segue.

---

## Como funciona

As organizações registram seus princípios de arquitetura, regras operacionais, políticas de segurança, conhecimento de domínio e critérios de qualidade na forma de um **Canon** — uma Single Source of Truth — e o projetam no contexto de execução que Claude, Codex, ChatGPT, Cursor e outros agentes de fato utilizam.

```
Canon  →  Format & Installer  →  Per-vendor / per-domain application  →  Installed copy (.theorem/)
doctrine     canon-kit              playbooks · canon-domains                  in your project
```

- **Canon** — os princípios, regras, critérios de design e padrões de trabalho que uma organização verificou e aprovou.
- **Agent Context** — o Canon compilado nos formatos de contexto e de comando que cada agente consome.
- **Workflow** — procedimentos padronizados de ideia → plano → construção → revisão → aprovação → entrega.
- **Validation** — verifica se a saída da IA está em conformidade com o Canon e com as políticas, expondo desvios e violações.
- **Feedback Loop** — novos conhecimentos e exceções vindos de projetos reais retornam ao Canon.

---

## Princípios fundamentais

| | |
|---|---|
| **Canon before Prompt** | Defina o padrão da organização antes dos prompts individuais. |
| **Context before Generation** | Forneça propósito, restrições, conhecimento de domínio e critérios de aceitação *antes* de gerar. |
| **Evidence before Trust** | "Uma IA fez isso" não é motivo para confiar — evidências, testes e revisão são. |
| **Process before Output** | Gerencie como um resultado é produzido, não apenas o artefato final. |
| **Organization over Individual** | Transforme a habilidade individual em ativos organizacionais reutilizáveis. |
| **Vendor Neutrality** | Mantenha-se independente de qualquer modelo ou provedor de IA específico. |
| **Human Accountability** | A IA apoia o julgamento e a execução; as decisões pertencem às pessoas. |
| **Continuous Evolution** | O Canon é um sistema vivo que incorpora a experiência verificada. |

---

## Ecossistema

The AI Theorem é um **ecossistema de repositórios independentes**. O núcleo neutro (`canon`) não nomeia nenhum dos demais nem depende deles; tudo se compõe no momento da instalação.

| Repository | Purpose | Status |
|---|---|---|
| [`canon`](https://github.com/the-ai-theorem/canon) | Doutrina pública estável — metodologia neutra em relação a fornecedores (eficácia · economia de tokens · desempenho · verificação de segurança · colaboração humano–IA) | **Active** |
| [`canon-kit`](https://github.com/the-ai-theorem/canon-kit) | Instalador + padrão de formato de pacote de ferramentas e mecanismo de instalação (conformidade · confiança · permissão · substituição) | Active |
| [`canon-lab`](https://github.com/the-ai-theorem/canon-lab) | Espaço de trabalho privado de autoria · construção · certificação | Private |
| [`canon-domains`](https://github.com/the-ai-theorem/canon-domains) | Módulos de domínio — MES, ERP, Factory Vision, Pharma, Healthcare, … (neutros em relação a fornecedores) | Planned |
| [`playbooks`](https://github.com/the-ai-theorem/playbooks) | Playbooks de aplicação por fornecedor / por agente + projetos de exemplo com fluxos de trabalho reais — Claude Code, Cursor, Codex, Gemini, … (neutros em relação a domínios) | Planned |
| [`community`](https://github.com/the-ai-theorem/community) | Conhecimento e discussão coletivos — um espaço compartilhado onde as opiniões e a experiência dos agentes de IA são acumuladas e verificadas em conjunto com pessoas | Planned |

**Dois eixos ortogonais — componha, não herde.** *O que* você constrói (o eixo de **domínio**) e *qual agente* você usa (o eixo de **fornecedor**) herdam apenas de `canon` e permanecem independentes entre si. O instalador compõe **um domínio × N playbooks de fornecedor → `.theorem/`** — de modo que não há nenhuma matriz `vendor × domain` para manter.

---

## Para quem é

- **Empresas** que adotam IA em toda a organização sem abrir mão de qualidade, segurança, consistência e responsabilidade.
- **CTOs e líderes técnicos** que preservam a arquitetura, a qualidade do código e os padrões operacionais no desenvolvimento assistido por IA.
- **Responsáveis pela governança de IA** que fecham a lacuna entre a política de IA e o que os agentes realmente fazem.
- **Especialistas de domínio** que transformam conhecimento tácito em ativos padronizados e consumíveis por IA.
- **Desenvolvedores de agentes** que precisam de um único contexto compartilhado e de um mesmo conjunto de regras de execução em diversos modelos e ferramentas.
- **Consultorias** que aplicam uma metodologia repetível a cada cliente.

---

## Comece agora

O canon **não é instalado diretamente** — ele é inicializado em um projeto pelo instalador.

1. Leia a doutrina: **[`canon`](https://github.com/the-ai-theorem/canon)** → comece por [`OVERVIEW.md`](https://github.com/the-ai-theorem/canon/blob/main/OVERVIEW.md).
2. Instale via **[`canon-kit`](https://github.com/the-ai-theorem/canon-kit)** — escolha a [release tag](https://github.com/the-ai-theorem/canon-kit/releases) mais recente e siga o Quick start.

Contribuições são bem-vindas — documentos de canon novos ou aprimorados, módulos de domínio, playbooks de fornecedor, templates e exemplos. Abra uma issue ou um pull request.

---

<div align="center">

**Canon before Prompt · Context before Generation · Evidence before Trust**

*Neutro em relação a fornecedores · Com responsabilidade humana · Em evolução contínua*

</div>
