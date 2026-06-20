<div align="center">

[English](../README.md) · [한국어](README.ko.md) · [中文](README.zh-CN.md) · [日本語](README.ja.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [**Español**](README.es.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [हिन्दी](README.hi.md) · [العربية](README.ar.md)

# The AI Theorem

**Un marco operativo canónico para una colaboración fiable entre personas e IA.**

[![Canon](https://img.shields.io/badge/canon-active%20development-blue)](https://github.com/the-ai-theorem/canon)
[![Vendor](https://img.shields.io/badge/vendor-neutral-success)]()
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](https://github.com/the-ai-theorem/canon/blob/main/LICENSE)

</div>

---

## Por qué The AI Theorem

La IA generativa y los agentes se están incorporando rápidamente al trabajo diario, pero en la mayoría de las organizaciones cada persona recurre a **prompts distintos, herramientas distintas y conocimiento ad hoc distinto**. Una misma tarea arroja resultados de calidad dispar, los estándares y las políticas no se cumplen, y no hay una forma clara de verificar lo que produjo un agente ni de rendir cuentas por ello.

The AI Theorem **no** es un sistema para gestionar *qué pedirle* a una IA. Es un sistema para definir **los principios y estándares con los que una IA debe juzgar y actuar**, y así transformar una práctica de IA fragmentada e individual en un **estándar operativo verificado, reutilizable y común a toda la organización**.

> El objetivo no son mejores prompts. El objetivo es un **canon** fiable que compartan todas las personas y todos los agentes, junto con una verificación continua de que el resultado real lo cumple de verdad.

---

## Cómo funciona

Las organizaciones recogen sus principios de arquitectura, reglas operativas, política de seguridad, conocimiento del dominio y criterios de calidad en forma de **Canon** — un Single Source of Truth — y lo proyectan al contexto de ejecución que realmente utilizan Claude, Codex, ChatGPT, Cursor y otros agentes.

```
Canon  →  Format & Installer  →  Per-vendor / per-domain application  →  Installed copy (.theorem/)
doctrine     canon-kit              canon-playbooks · canon-domains            in your project
```

- **Canon** — los principios, reglas, criterios de diseño y estándares de trabajo que una organización ha verificado y aprobado.
- **Agent Context** — el Canon compilado en los formatos de contexto y comandos que consume cada agente.
- **Workflow** — procedimientos estandarizados que van de idea → plan → construcción → revisión → aprobación → entrega.
- **Validation** — comprueba si el resultado de la IA se ajusta al Canon y a la política, y saca a la luz desviaciones e infracciones.
- **Feedback Loop** — el conocimiento nuevo y las excepciones surgidas en proyectos reales vuelven a integrarse en el Canon.

---

## Principios fundamentales

| | |
|---|---|
| **Canon before Prompt** | Define el estándar de la organización antes que los prompts individuales. |
| **Context before Generation** | Aporta propósito, restricciones, conocimiento del dominio y criterios de aceptación *antes* de generar. |
| **Evidence before Trust** | "Lo hizo una IA" no es motivo para confiar en ello; lo son la evidencia, las pruebas y la revisión. |
| **Process before Output** | Gobierna cómo se produce un resultado, no solo el artefacto final. |
| **Organization over Individual** | Convierte la habilidad individual en activos organizativos reutilizables. |
| **Vendor Neutrality** | Mantente independiente de cualquier modelo o proveedor de IA concreto. |
| **Human Accountability** | La IA apoya el juicio y la ejecución; las decisiones son responsabilidad de las personas. |
| **Continuous Evolution** | El Canon es un sistema vivo que asimila la experiencia verificada. |

---

## Ecosistema

The AI Theorem es un **ecosistema de repositorios independientes**. El núcleo neutral (`canon`) no nombra a ningún repositorio hermano ni depende de él; todo se compone en el momento de la instalación.

| Repository | Propósito | Estado |
|---|---|---|
| [`canon`](https://github.com/the-ai-theorem/canon) | Doctrina pública y estable — metodología neutral respecto al proveedor (eficacia · economía de tokens · rendimiento · verificación de seguridad · colaboración entre personas e IA) | **Activo** |
| [`canon-kit`](https://github.com/the-ai-theorem/canon-kit) | Instalador + estándar de formato del paquete de herramientas y mecanismo de instalación (conformidad · confianza · permisos · anulación) | Activo |
| [`canon-lab`](https://github.com/the-ai-theorem/canon-lab) | Espacio de trabajo privado de autoría · construcción · certificación | Privado |
| [`canon-domains`](https://github.com/the-ai-theorem/canon-domains) | Módulos de dominio — MES, ERP, Factory Vision, Pharma, Healthcare, … (neutral respecto al proveedor) | Planificado |
| [`canon-playbooks`](https://github.com/the-ai-theorem/canon-playbooks) | Playbooks de aplicación por proveedor / por agente — Claude Code, Cursor, Codex, Gemini, … (neutral respecto al dominio) | Planificado |
| [`canon-examples`](https://github.com/the-ai-theorem/canon-examples) | Proyectos de ejemplo que aplican el Canon en flujos de trabajo reales | Planificado |

**Dos ejes ortogonales — componer, no heredar.** *Qué* construyes (el eje del **dominio**) y *qué agente* usas (el eje del **proveedor**) heredan únicamente de `canon` y se mantienen independientes entre sí. El instalador compone **un dominio × N playbooks de proveedor → `.theorem/`**, de modo que no hay ninguna matriz `vendor × domain` que mantener.

---

## Para quién es

- **Empresas** que adoptan la IA en toda la organización sin renunciar a la calidad, la seguridad, la consistencia y la rendición de cuentas.
- **CTOs y líderes técnicos** que preservan la arquitectura, la calidad del código y los estándares operativos en el desarrollo asistido por IA.
- **Responsables de gobernanza de IA** que cierran la brecha entre la política de IA y lo que los agentes hacen en la práctica.
- **Expertos de dominio** que convierten el conocimiento tácito en activos estandarizados y consumibles por IA.
- **Desarrolladores de agentes** que necesitan un único contexto compartido y un mismo conjunto de reglas de ejecución para muchos modelos y herramientas.
- **Consultoras** que aplican una metodología repetible cliente a cliente.

---

## Cómo empezar

El canon **no se instala directamente** — es el instalador el que lo incorpora a un proyecto.

1. Lee la doctrina: **[`canon`](https://github.com/the-ai-theorem/canon)** → empieza por [`OVERVIEW.md`](https://github.com/the-ai-theorem/canon/blob/main/OVERVIEW.md).
2. Instala mediante **[`canon-kit`](https://github.com/the-ai-theorem/canon-kit)** — elige la última [release tag](https://github.com/the-ai-theorem/canon-kit/releases) y sigue su Quick start.

Las contribuciones son bienvenidas — documentos de canon nuevos o mejorados, módulos de dominio, playbooks de proveedor, plantillas y ejemplos. Abre un issue o un pull request.

---

<div align="center">

**Canon before Prompt · Context before Generation · Evidence before Trust**

*Neutral respecto al proveedor · Responsabilidad humana · En evolución continua*

</div>
