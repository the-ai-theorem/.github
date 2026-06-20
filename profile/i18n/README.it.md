<div align="center">

[English](../README.md) · [한국어](README.ko.md) · [中文](README.zh-CN.md) · [日本語](README.ja.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [Español](README.es.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [**Italiano**](README.it.md) · [हिन्दी](README.hi.md) · [العربية](README.ar.md)

# The AI Theorem

**Un framework operativo canonico per una collaborazione affidabile tra persone e IA.**

[![Canon](https://img.shields.io/badge/canon-active%20development-blue)](https://github.com/the-ai-theorem/canon)
[![Vendor](https://img.shields.io/badge/vendor-neutral-success)]()
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](https://github.com/the-ai-theorem/canon/blob/main/LICENSE)

</div>

---

## Perché The AI Theorem

L'IA generativa e gli agenti stanno entrando rapidamente nel lavoro di tutti i giorni, ma nella maggior parte delle organizzazioni ognuno usa **prompt diversi, strumenti diversi e conoscenze improvvisate diverse**. Lo stesso compito produce risultati di qualità disomogenea, gli standard e le policy restano disattesi e manca un modo chiaro per verificare ciò che un agente ha prodotto o per attribuirne la responsabilità.

The AI Theorem **non** è un sistema per gestire *cosa chiedere* a un'IA. È un sistema per definire **i principi e gli standard in base ai quali un'IA deve valutare e agire**, e trasforma una pratica dell'IA frammentaria e individuale in uno **standard operativo verificato, riutilizzabile e condiviso da tutta l'organizzazione**.

> Il punto non sono prompt migliori. Il punto è un **canon** affidabile, condiviso da ogni persona e ogni agente, e una verifica continua che gli output reali lo rispettino davvero.

---

## Come funziona

Le organizzazioni codificano i propri principi di architettura, regole operative, policy di sicurezza, conoscenza di dominio e criteri di qualità in un **Canon** — una Single Source of Truth — e lo proiettano nel contesto di esecuzione che Claude, Codex, ChatGPT, Cursor e altri agenti utilizzano concretamente.

```
Canon  →  Format & Installer  →  Per-vendor / per-domain application  →  Installed copy (.theorem/)
doctrine     canon-kit              playbooks · canon-domains                  in your project
```

- **Canon** — i principi, le regole, i criteri di progettazione e gli standard di lavoro che l'organizzazione ha verificato e approvato.
- **Agent Context** — il Canon compilato nei formati di contesto e nei comandi che i diversi agenti utilizzano.
- **Workflow** — procedure standardizzate da idea → piano → sviluppo → revisione → approvazione → rilascio.
- **Validation** — verifica che l'output dell'IA sia conforme al Canon e alle policy, segnalando scostamenti e violazioni.
- **Feedback Loop** — le nuove conoscenze e le eccezioni che emergono dai progetti reali rientrano nel Canon.

---

## Principi fondamentali

| | |
|---|---|
| **Canon before Prompt** | Definire lo standard dell'organizzazione prima dei singoli prompt. |
| **Context before Generation** | Fornire obiettivo, vincoli, conoscenza di dominio e criteri di accettazione *prima* di generare. |
| **Evidence before Trust** | "L'ha fatto un'IA" non è un motivo per fidarsi; lo sono le prove, i test e la revisione. |
| **Process before Output** | Governare il modo in cui un risultato viene prodotto, non solo l'artefatto finale. |
| **Organization over Individual** | Trasformare le competenze individuali in asset organizzativi riutilizzabili. |
| **Vendor Neutrality** | Restare indipendenti da qualsiasi singolo modello o fornitore di IA. |
| **Human Accountability** | L'IA supporta il giudizio e l'esecuzione; le decisioni restano in capo alle persone. |
| **Continuous Evolution** | Il Canon è un sistema vivo che fa propria l'esperienza verificata. |

---

## Ecosistema

The AI Theorem è un **ecosistema di repository indipendenti**. Il nucleo neutrale (`canon`) non nomina alcun repository affine e non dipende da nessuno di essi; tutto si compone al momento dell'installazione.

| Repository | Scopo | Stato |
|---|---|---|
| [`canon`](https://github.com/the-ai-theorem/canon) | Dottrina pubblica e stabile — metodologia neutrale rispetto al vendor (efficacia · economia dei token · prestazioni · verifica della sicurezza · collaborazione tra persone e IA) | **Attivo** |
| [`canon-kit`](https://github.com/the-ai-theorem/canon-kit) | Installer + standard del formato dei tool pack e meccanismo di installazione (conformità · fiducia · permessi · override) | Attivo |
| [`canon-lab`](https://github.com/the-ai-theorem/canon-lab) | Spazio di lavoro privato per creazione · build · certificazione | Privato |
| [`canon-domains`](https://github.com/the-ai-theorem/canon-domains) | Moduli di dominio — MES, ERP, Factory Vision, Pharma, Healthcare, … (neutrali rispetto al vendor) | Pianificato |
| [`playbooks`](https://github.com/the-ai-theorem/playbooks) | Playbook applicativi per-vendor / per-agente + progetti di esempio con workflow reali — Claude Code, Cursor, Codex, Gemini, … (neutrali rispetto al dominio) | Pianificato |
| [`community`](https://github.com/the-ai-theorem/community) | Conoscenza collettiva e confronto — uno spazio condiviso in cui le opinioni e l'esperienza degli agenti IA vengono accumulate e verificate insieme alle persone | Pianificato |

**Due assi ortogonali — comporre, non ereditare.** *Cosa* costruisci (l'asse del **dominio**) e *con quale agente* lo costruisci (l'asse del **vendor**) ereditano entrambi solo da `canon` e restano indipendenti. L'installer compone **un dominio × N playbook di vendor → `.theorem/`**, così non c'è alcuna matrice `vendor × domain` da mantenere.

---

## A chi si rivolge

- **Aziende** che adottano l'IA su scala di tutta l'organizzazione mantenendo qualità, sicurezza, coerenza e responsabilità.
- **CTO e leader tecnici** che vogliono preservare architettura, qualità del codice e standard operativi nello sviluppo assistito dall'IA.
- **Responsabili della governance dell'IA** che vogliono colmare il divario tra le policy sull'IA e ciò che gli agenti fanno davvero.
- **Esperti di dominio** che trasformano la competenza tacita in asset standardizzati e utilizzabili dall'IA.
- **Sviluppatori di agenti** che hanno bisogno di un unico contesto condiviso e di un insieme di regole di esecuzione comuni a molti modelli e strumenti.
- **Società di consulenza** che vogliono applicare una metodologia ripetibile a ogni cliente.

---

## Per iniziare

Il canon **non si installa direttamente** — viene avviato in un progetto tramite l'installer.

1. Leggi la dottrina: **[`canon`](https://github.com/the-ai-theorem/canon)** → parti da [`OVERVIEW.md`](https://github.com/the-ai-theorem/canon/blob/main/OVERVIEW.md).
2. Installa tramite **[`canon-kit`](https://github.com/the-ai-theorem/canon-kit)** — scegli l'ultimo [release tag](https://github.com/the-ai-theorem/canon-kit/releases) e segui il relativo Quick start.

I contributi sono benvenuti — documenti canon nuovi o migliorati, moduli di dominio, playbook di vendor, template ed esempi. Apri una issue o una pull request.

---

<div align="center">

**Canon before Prompt · Context before Generation · Evidence before Trust**

*Neutrale rispetto al vendor · Responsabilità umana · In continua evoluzione*

</div>
