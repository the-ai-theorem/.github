<div align="center">

[English](../README.md) · [한국어](README.ko.md) · [中文](README.zh-CN.md) · [日本語](README.ja.md) · [**Deutsch**](README.de.md) · [Français](README.fr.md) · [Español](README.es.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [हिन्दी](README.hi.md) · [العربية](README.ar.md)

# The AI Theorem

**Ein kanonisches Betriebsframework für verlässliche Mensch-KI-Zusammenarbeit.**

[![Canon](https://img.shields.io/badge/canon-active%20development-blue)](https://github.com/the-ai-theorem/canon)
[![Vendor](https://img.shields.io/badge/vendor-neutral-success)]()
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](https://github.com/the-ai-theorem/canon/blob/main/LICENSE)

</div>

---

## Warum The AI Theorem

Generative KI und Agenten halten rasant Einzug in den Arbeitsalltag — doch in den meisten Organisationen arbeitet jede und jeder mit **anderen Prompts, anderen Werkzeugen und anderem Ad-hoc-Wissen**. Dieselbe Aufgabe liefert mal so, mal so gute Ergebnisse, Standards und Richtlinien werden nicht durchgesetzt, und es fehlt ein klarer Weg, das von einem Agenten Erzeugte zu überprüfen oder dafür Verantwortung zu übernehmen.

The AI Theorem ist **kein** System dafür, *was man eine KI fragt*. Es ist ein System, um **die Prinzipien und Standards zu definieren, nach denen eine KI urteilen und handeln soll** — und macht aus fragmentierter, individueller KI-Praxis einen **verifizierten, wiederverwendbaren Betriebsstandard für die gesamte Organisation**.

> Es geht nicht um bessere Prompts. Es geht um einen vertrauenswürdigen **Canon**, den alle Beteiligten und alle Agenten teilen — und um die kontinuierliche Verifizierung, dass die tatsächliche Ausgabe ihm auch wirklich folgt.

---

## So funktioniert es

Organisationen halten ihre Architekturprinzipien, Betriebsregeln, Sicherheitsrichtlinien, ihr Domänenwissen und ihre Qualitätskriterien als **Canon** fest — eine Single Source of Truth — und projizieren ihn in den Ausführungskontext, mit dem Claude, Codex, ChatGPT, Cursor und andere Agenten tatsächlich arbeiten.

```
Canon  →  Format & Installer  →  Per-vendor / per-domain application  →  Installed copy (.theorem/)
doctrine     canon-kit              canon-playbooks · canon-domains            in your project
```

- **Canon** — die Prinzipien, Regeln, Designkriterien und Arbeitsstandards, die eine Organisation verifiziert und freigegeben hat.
- **Agent Context** — Canon, übersetzt in die Kontext- und Befehlsformate, die verschiedene Agenten verarbeiten.
- **Workflow** — standardisierte Abläufe von Idee → Plan → Umsetzung → Review → Freigabe → Auslieferung.
- **Validation** — prüft, ob die KI-Ausgabe Canon und Richtlinien entspricht, und macht Abweichungen und Verstöße sichtbar.
- **Feedback Loop** — neues Wissen und Ausnahmen aus realen Projekten fließen zurück in den Canon.

---

## Kernprinzipien

| | |
|---|---|
| **Canon before Prompt** | Definiere den Standard der Organisation, bevor einzelne Prompts entstehen. |
| **Context before Generation** | Liefere Zweck, Rahmenbedingungen, Domänenwissen und Abnahmekriterien *vor* der Generierung. |
| **Evidence before Trust** | „Eine KI hat es erstellt" ist kein Grund, ihr zu vertrauen — Belege, Tests und Review sind es. |
| **Process before Output** | Steuere, wie ein Ergebnis entsteht, nicht nur das fertige Artefakt. |
| **Organization over Individual** | Mache aus individuellem Können wiederverwendbaren Wert für die Organisation. |
| **Vendor Neutrality** | Bleibe unabhängig von einem einzelnen KI-Modell oder Anbieter. |
| **Human Accountability** | KI unterstützt Urteil und Ausführung; die Verantwortung tragen Menschen. |
| **Continuous Evolution** | Canon ist ein lebendiges System, das verifizierte Erfahrung aufnimmt. |

---

## Ökosystem

The AI Theorem ist ein **Ökosystem unabhängiger Repositories**. Der neutrale Kern (`canon`) benennt keine Geschwister-Repositories und hängt von keinem ab; alles wird zur Installationszeit zusammengesetzt.

| Repository | Purpose | Status |
|---|---|---|
| [`canon`](https://github.com/the-ai-theorem/canon) | Öffentliche, stabile Doktrin — anbieterneutrale Methodik (Wirksamkeit · Token-Ökonomie · Performance · Sicherheitsverifizierung · Mensch-KI-Zusammenarbeit) | **Active** |
| [`canon-kit`](https://github.com/the-ai-theorem/canon-kit) | Installer + Standard für Paketformat und Installationsmechanismus von Tools (Konformität · Vertrauen · Berechtigung · Override) | Active |
| [`canon-lab`](https://github.com/the-ai-theorem/canon-lab) | Privater Arbeitsbereich für Authoring · Build · Zertifizierung | Private |
| [`canon-domains`](https://github.com/the-ai-theorem/canon-domains) | Domänenmodule — MES, ERP, Factory Vision, Pharma, Healthcare, … (anbieterneutral) | Planned |
| [`canon-playbooks`](https://github.com/the-ai-theorem/canon-playbooks) | Anwendungs-Playbooks pro Anbieter / pro Agent — Claude Code, Cursor, Codex, Gemini, … (domänenneutral) | Planned |
| [`canon-examples`](https://github.com/the-ai-theorem/canon-examples) | Beispielprojekte, die Canon in realen Workflows anwenden | Planned |

**Zwei orthogonale Achsen — komponieren statt vererben.** *Was* du baust (die **Domänen**-Achse) und *welchen Agenten* du einsetzt (die **Anbieter**-Achse) erben jeweils nur von `canon` und bleiben voneinander unabhängig. Der Installer komponiert **eine Domäne × N Anbieter-Playbooks → `.theorem/`** — so muss keine `vendor × domain`-Matrix gepflegt werden.

---

## Für wen es gedacht ist

- **Unternehmen**, die KI organisationsweit einführen und dabei Qualität, Sicherheit, Konsistenz und Verantwortlichkeit wahren wollen.
- **CTOs und technische Führungskräfte**, die Architektur, Codequalität und Betriebsstandards in der KI-gestützten Entwicklung sichern.
- **Verantwortliche für KI-Governance**, die die Lücke zwischen KI-Richtlinie und dem schließen, was Agenten tatsächlich tun.
- **Domänenexpertinnen und -experten**, die implizites Fachwissen in standardisierten, KI-verwertbaren Wert überführen.
- **Agentenentwicklerinnen und -entwickler**, die über viele Modelle und Werkzeuge hinweg einen gemeinsamen Kontext und ein einheitliches Ausführungsregelwerk brauchen.
- **Beratungsunternehmen**, die eine wiederholbare Methodik bei jedem Kunden anwenden.

---

## Erste Schritte

Der Canon wird **nicht direkt installiert** — der Installer bootstrappt ihn in ein Projekt.

1. Lies die Doktrin: **[`canon`](https://github.com/the-ai-theorem/canon)** → beginne mit [`OVERVIEW.md`](https://github.com/the-ai-theorem/canon/blob/main/OVERVIEW.md).
2. Installiere über **[`canon-kit`](https://github.com/the-ai-theorem/canon-kit)** — wähle das neueste [Release-Tag](https://github.com/the-ai-theorem/canon-kit/releases) und folge dessen Quick start.

Beiträge sind willkommen — neue oder verbesserte Canon-Dokumente, Domänenmodule, Anbieter-Playbooks, Vorlagen und Beispiele. Öffne ein Issue oder einen Pull Request.

---

<div align="center">

**Canon before Prompt · Context before Generation · Evidence before Trust**

*Anbieterneutral · Menschlich verantwortet · Kontinuierlich evolvierend*

</div>
