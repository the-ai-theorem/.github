<div align="center">

[English](../README.md) · [한국어](README.ko.md) · [中文](README.zh-CN.md) · [日本語](README.ja.md) · [Deutsch](README.de.md) · [**Français**](README.fr.md) · [Español](README.es.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [हिन्दी](README.hi.md) · [العربية](README.ar.md)

# The AI Theorem

**Un cadre opérationnel canonique pour une collaboration humain-IA fiable.**

[![Canon](https://img.shields.io/badge/canon-active%20development-blue)](https://github.com/the-ai-theorem/canon)
[![Vendor](https://img.shields.io/badge/vendor-neutral-success)]()
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](https://github.com/the-ai-theorem/canon/blob/main/LICENSE)

</div>

---

## Pourquoi The AI Theorem

L'IA générative et les agents s'imposent rapidement dans le travail quotidien — mais dans la plupart des organisations, chacun recourt à **des prompts différents, des outils différents et des connaissances ad hoc différentes**. Une même tâche débouche sur une qualité inégale, les normes et les politiques ne sont pas respectées, et rien ne permet de vérifier clairement ce qu'un agent a produit ni d'en assumer la responsabilité.

The AI Theorem n'est **pas** un système qui gère *ce qu'il faut demander* à une IA. C'est un système qui définit **les principes et les normes selon lesquels une IA doit juger et agir** — et qui transforme ainsi une pratique de l'IA fragmentée et individuelle en une **norme opérationnelle vérifiée, réutilisable et déployée à l'échelle de l'organisation**.

> L'enjeu n'est pas de meilleurs prompts. L'enjeu, c'est un **canon** digne de confiance que chaque personne et chaque agent partage — et une vérification continue que le résultat réel le respecte bel et bien.

---

## Comment ça fonctionne

Les organisations consignent leurs principes d'architecture, leurs règles opérationnelles, leur politique de sécurité, leurs connaissances métier et leurs critères de qualité sous forme de **Canon** — une Single Source of Truth — puis les projettent dans le contexte d'exécution qu'utilisent réellement Claude, Codex, ChatGPT, Cursor et d'autres agents.

```
Canon  →  Format & Installer  →  Per-vendor / per-domain application  →  Installed copy (.theorem/)
doctrine     canon-kit              playbooks · canon-domains                  in your project
```

- **Canon** — les principes, règles, critères de conception et normes de travail qu'une organisation a vérifiés et validés.
- **Contexte de l'agent** — le Canon compilé dans les formats de contexte et de commandes que consomment les différents agents.
- **Workflow** — des procédures standardisées qui vont de l'idée → la planification → la construction → la revue → l'approbation → la livraison.
- **Validation** — vérifie la conformité du résultat de l'IA au Canon et à la politique, en signalant les dérives et les manquements.
- **Boucle de rétroaction** — les nouvelles connaissances et exceptions issues de projets réels viennent enrichir le Canon.

---

## Principes fondamentaux

| | |
|---|---|
| **Canon before Prompt** | Définir la norme de l'organisation avant les prompts individuels. |
| **Context before Generation** | Fournir l'objectif, les contraintes, les connaissances métier et les critères d'acceptation *avant* de générer. |
| **Evidence before Trust** | « C'est une IA qui l'a fait » n'est pas une raison d'y faire confiance — les preuves, les tests et la revue le sont. |
| **Process before Output** | Maîtriser la façon dont un résultat est produit, et pas seulement l'artefact final. |
| **Organization over Individual** | Convertir la compétence individuelle en actifs organisationnels réutilisables. |
| **Vendor Neutrality** | Rester indépendant de tout modèle ou fournisseur d'IA. |
| **Human Accountability** | L'IA appuie le jugement et l'exécution ; la décision reste entre les mains des humains. |
| **Continuous Evolution** | Le Canon est un système vivant qui intègre l'expérience vérifiée. |

---

## Écosystème

The AI Theorem est un **écosystème de dépôts indépendants**. Le cœur neutre (`canon`) ne nomme aucun voisin et n'en dépend d'aucun ; tout se compose au moment de l'installation.

| Repository | Purpose | Status |
|---|---|---|
| [`canon`](https://github.com/the-ai-theorem/canon) | Doctrine publique stable — méthodologie indépendante des fournisseurs (efficacité · économie de tokens · performance · vérification de sécurité · collaboration humain-IA) | **Actif** |
| [`canon-kit`](https://github.com/the-ai-theorem/canon-kit) | Installateur + norme de format des paquets d'outils et mécanisme d'installation (conformité · confiance · permissions · surcharges) | Actif |
| [`canon-lab`](https://github.com/the-ai-theorem/canon-lab) | Espace de travail privé de rédaction · construction · certification | Privé |
| [`canon-domains`](https://github.com/the-ai-theorem/canon-domains) | Modules métier — MES, ERP, Factory Vision, Pharma, Healthcare, … (indépendants des fournisseurs) | Prévu |
| [`playbooks`](https://github.com/the-ai-theorem/playbooks) | Playbooks d'application par fournisseur / par agent + projets d'exemple de workflows réels — Claude Code, Cursor, Codex, Gemini, … (indépendants des métiers) | Prévu |
| [`community`](https://github.com/the-ai-theorem/community) | Connaissances et discussions collectives — un espace partagé où les opinions et l'expérience des agents IA s'accumulent et se vérifient conjointement avec les humains | Prévu |

**Deux axes orthogonaux — composer plutôt qu'hériter.** *Ce que* vous construisez (l'axe **domaine**) et *quel agent* vous utilisez (l'axe **fournisseur**) héritent uniquement de `canon` et restent indépendants l'un de l'autre. L'installateur compose **un domaine × N playbooks de fournisseurs → `.theorem/`** — aucune matrice `vendor × domain` à maintenir, donc.

---

## À qui s'adresse-t-il

- **Aux entreprises** qui adoptent l'IA à l'échelle de l'organisation tout en préservant la qualité, la sécurité, la cohérence et la responsabilité.
- **Aux CTO et responsables techniques** soucieux de préserver l'architecture, la qualité du code et les normes opérationnelles dans le développement assisté par IA.
- **Aux responsables de la gouvernance de l'IA** qui veulent combler l'écart entre la politique d'IA et ce que les agents font réellement.
- **Aux experts métier** qui transforment leur expertise tacite en actifs standardisés et exploitables par l'IA.
- **Aux développeurs d'agents** qui ont besoin d'un contexte partagé et d'un jeu de règles d'exécution unique sur de nombreux modèles et outils.
- **Aux cabinets de conseil** qui appliquent une méthodologie reproductible d'un client à l'autre.

---

## Pour commencer

Le canon ne s'installe **pas directement** — il est amorcé dans un projet par l'installateur.

1. Lisez la doctrine : **[`canon`](https://github.com/the-ai-theorem/canon)** → commencez par [`OVERVIEW.md`](https://github.com/the-ai-theorem/canon/blob/main/OVERVIEW.md).
2. Installez via **[`canon-kit`](https://github.com/the-ai-theorem/canon-kit)** — choisissez le dernier [tag de version](https://github.com/the-ai-theorem/canon-kit/releases) et suivez son guide de démarrage rapide.

Les contributions sont les bienvenues — documents canon nouveaux ou enrichis, modules métier, playbooks de fournisseurs, modèles et exemples. Ouvrez une issue ou une pull request.

---

<div align="center">

**Canon before Prompt · Context before Generation · Evidence before Trust**

*Indépendant des fournisseurs · Responsabilité humaine · En évolution continue*

</div>
