<div align="center">

[English](../README.md) · [한국어](README.ko.md) · [中文](README.zh-CN.md) · [**日本語**](README.ja.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [Español](README.es.md) · [Português](README.pt-BR.md) · [Русский](README.ru.md) · [Italiano](README.it.md) · [हिन्दी](README.hi.md) · [العربية](README.ar.md)

# The AI Theorem

**信頼できる人間とAIの協働を実現する、規範ベースの運用フレームワーク。**

[![Canon](https://img.shields.io/badge/canon-active%20development-blue)](https://github.com/the-ai-theorem/canon)
[![Vendor](https://img.shields.io/badge/vendor-neutral-success)]()
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](https://github.com/the-ai-theorem/canon/blob/main/LICENSE)

</div>

---

## なぜ The AI Theorem なのか

生成AIとエージェントは、急速に日々の業務へ浸透しつつあります。しかし多くの組織では、誰もが**それぞれ異なるプロンプト、異なるツール、異なる場当たり的な知識**を使っているのが実情です。その結果、同じ作業でも品質はばらつき、標準やポリシーは徹底されず、エージェントが生成した成果物を検証したり、その責任を明確にしたりする手段も存在しません。

The AI Theorem は、AIに*何を尋ねるか*を管理するシステムでは**ありません**。**AIが判断し行動する際に従うべき原則と標準**を定義するシステムであり、断片化した個人任せのAI活用を、**検証済みで再利用可能な、組織全体の運用標準**へと変えるものです。

> 求められているのは、より良いプロンプトではありません。あらゆる人とあらゆるエージェントが共有する、信頼できる**canon**こそが本質です。そして、実際の成果物が本当にその canon に従っているかを、継続的に検証し続けることが欠かせません。

---

## 仕組み

組織は、自らのアーキテクチャ原則、運用ルール、セキュリティポリシー、ドメイン知識、品質基準を**Canon**（Single Source of Truth）として一元的に定義します。そして、その Canon を Claude、Codex、ChatGPT、Cursor をはじめとする各エージェントが実際に使う実行コンテキストへと展開します。

```
Canon  →  Format & Installer  →  Per-vendor / per-domain application  →  Installed copy (.theorem/)
doctrine     canon-kit              playbooks · canon-domains                  in your project
```

- **Canon** — 組織が検証し承認した、原則・ルール・設計基準・作業標準。
- **Agent Context** — 各エージェントが読み込めるコンテキストやコマンド形式へとコンパイルされた Canon。
- **Workflow** — アイデア → 計画 → 構築 → レビュー → 承認 → 出荷に至る、標準化された一連の手順。
- **Validation** — AIの成果物が Canon とポリシーに準拠しているかを検査し、逸脱や違反を可視化する仕組み。
- **Feedback Loop** — 実際のプロジェクトで得られた新たな知見や例外を、Canon へと還流させる仕組み。

---

## 中核となる原則

| | |
|---|---|
| **Canon before Prompt** | 個々のプロンプトに先立って、組織の標準を定義する。 |
| **Context before Generation** | 生成に*入る前に*、目的・制約・ドメイン知識・受け入れ基準を与える。 |
| **Evidence before Trust** | 「AIが作った」ことは信頼の根拠にはならない。信頼を支えるのは、証拠・テスト・レビューである。 |
| **Process before Output** | 最終成果物だけでなく、それがどのように生み出されたかという過程を管理する。 |
| **Organization over Individual** | 個人のスキルを、再利用可能な組織の資産へと昇華させる。 |
| **Vendor Neutrality** | 特定のAIモデルやプロバイダーに依存しない。 |
| **Human Accountability** | AIは判断と実行を支援するが、最終的な意思決定の責任は人間が負う。 |
| **Continuous Evolution** | Canon は、検証された経験を取り込み続ける「生きたシステム」である。 |

---

## エコシステム

The AI Theorem は、**互いに独立したリポジトリ群からなるエコシステム**です。中立なコアである `canon` は、いずれの関連リポジトリの名前にも触れず、どれにも依存しません。すべての要素は、インストール時に初めて合成されます。

| Repository | Purpose | Status |
|---|---|---|
| [`canon`](https://github.com/the-ai-theorem/canon) | 公開・安定版のドクトリン — ベンダー中立な方法論（有効性 · トークン経済 · パフォーマンス · セキュリティ検証 · 人間とAIの協働） | **Active** |
| [`canon-kit`](https://github.com/the-ai-theorem/canon-kit) | 標準とインストール機構を、インストーラー + ツールパッケージとして提供（適合性 · 信頼 · 権限 · オーバーライド） | Active |
| [`canon-lab`](https://github.com/the-ai-theorem/canon-lab) | 非公開の、作成 · ビルド · 認証のためのワークスペース | Private |
| [`canon-domains`](https://github.com/the-ai-theorem/canon-domains) | ドメインモジュール群 — MES, ERP, Factory Vision, Pharma, Healthcare, …（ベンダー中立） | Planned |
| [`playbooks`](https://github.com/the-ai-theorem/playbooks) | ベンダー別 / エージェント別の適用プレイブック + 実際のワークフローのサンプルプロジェクト — Claude Code, Cursor, Codex, Gemini, …（ドメイン中立） | Planned |
| [`community`](https://github.com/the-ai-theorem/community) | 集合知と議論の場 — AIエージェントの見解や経験を、人間とともに蓄積し検証し合う共有スペース | Planned |

**直交する二つの軸 — 継承ではなく、合成する。** *何を*構築するか（**domain** 軸）と、*どのエージェントを*使うか（**vendor** 軸）は、ともに `canon` のみを継承し、互いに独立した関係を保ちます。インストーラーが**一つのドメイン × N個のベンダープレイブック → `.theorem/`** を合成するため、`vendor × domain` の組み合わせマトリクスを維持する必要はありません。

---

## 対象となる方

- AIを組織全体へ展開しつつ、品質・セキュリティ・一貫性・説明責任を維持したい**企業**。
- AI支援開発において、アーキテクチャ・コード品質・運用標準を守りたい**CTOや技術リーダー**。
- AIポリシーと、エージェントの実際の挙動との間にあるギャップを埋めたい**AIガバナンス責任者**。
- 暗黙知としての専門知識を、標準化されAIが読み込める資産へと変えたい**ドメインエキスパート**。
- 数多くのモデルやツールをまたいで、共有された一つのコンテキストと実行ルールを必要とする**エージェント開発者**。
- クライアントごとに、再現可能な方法論を適用したい**コンサルティング会社**。

---

## はじめに

canon は、**直接インストールするものではありません** — インストーラーを通じて、プロジェクトへブートストラップされます。

1. まずドクトリンを読む: **[`canon`](https://github.com/the-ai-theorem/canon)** の [`OVERVIEW.md`](https://github.com/the-ai-theorem/canon/blob/main/OVERVIEW.md) から始めてください。
2. **[`canon-kit`](https://github.com/the-ai-theorem/canon-kit)** 経由でインストールする — 最新の [release tag](https://github.com/the-ai-theorem/canon-kit/releases) を選び、その Quick start に従ってください。

新規または改善された canon 文書、ドメインモジュール、ベンダープレイブック、テンプレート、サンプルなど、貢献を歓迎します。お気軽に Issue または Pull Request をお寄せください。

---

<div align="center">

**Canon before Prompt · Context before Generation · Evidence before Trust**

*ベンダー中立 · 人間が責任を負う · 継続的に進化する*

</div>
