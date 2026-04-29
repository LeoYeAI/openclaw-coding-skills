# OpenClaw Coding Skills

[![Skills](https://img.shields.io/badge/スキル-13-blue?style=for-the-badge)](./skills/INDEX.md)
[![リファレンス](https://img.shields.io/badge/実行リファレンス-21-green?style=for-the-badge)](./skills/)
[![評価サンプル](https://img.shields.io/badge/評価サンプル-39-orange?style=for-the-badge)](./evaluation/)
[![トリガールール](https://img.shields.io/badge/トリガールール-131-purple?style=for-the-badge)](./skills/TRIGGER-MATRIX.md)
[![ライセンス](https://img.shields.io/badge/ライセンス-MIT-brightgreen?style=for-the-badge)](./LICENSE)
[![Powered by MyClaw.ai](https://img.shields.io/badge/Powered%20by-MyClaw.ai-ff6b35?style=for-the-badge)](https://myclaw.ai)

**エージェントがうまくいくことを祈るのはやめよう。信頼できるコーディング行動をデフォルトにしよう。**

[English](./README.md) · [中文](./README.zh-CN.md) · [Deutsch](./README.de.md) · [Français](./README.fr.md) · [Español](./README.es.md) · [Italiano](./README.it.md) · [日本語](./README.ja.md) · [Русский](./README.ru.md)

---

### 概要

| レイヤー | 内容 | 数量 |
|---------|------|------|
| **ワークフロースキル** | `spec` → `plan` → `build` → `test` → `review` → `ship` | 7 |
| **スペシャリストスキル** | `debug` · `security` · `frontend` · `docs` · `deploy` · `refactor` | 6 |
| **実行リファレンス** | 高リスクスキル内の再利用可能な意思決定サポート | 21ファイル |
| **トリガーマトリックス** | リクエスト→スキルマッピングと境界ケースガイダンス | 131ルール |
| **評価アセット** | ラベル付きサンプル、曖昧ケース、dry-run＆live検証 | 39サンプル、6データセット |
| **チューニング基盤** | プレイブック、結果スキーマ、フィードバックループ、チューニングログ | 完全なクローズドループ |

> **70以上のファイル · 13スキル · 21実行リファレンス · 39評価サンプル · 131トリガールール**

---

OpenClawエージェント向けのプロダクションレベルのコーディングスキル。

[MyClaw.ai](https://myclaw.ai)エコシステムの一部：エージェントの生の能力を信頼性の高いソフトウェア実行に変換するために設計された、成長し続けるオープンアセットの集合体。

## MyClaw.aiについて

[MyClaw.ai](https://myclaw.ai)は���各ユーザーに[OpenClaw](https://github.com/openclaw/openclaw)（業界をリードするオープンソースAIエージェントフレームワーク）を実行する完全なサーバーを提供するAIアシスタントプラットフォームです。各MyClawインスタンスは、完全なコード制御、ネットワークアクセス、ツールアクセス、そしてこのようなスキルを直接インストールする能力を提供します。

MyClaw.aiエコシステム内で、このリポジトリは**コーディング行動レイヤー**として機能します：「モデルがコードを書ける」と「エージェントがソフトウェア作業を規律を持って実行できる」の間のギャップを埋めます。MyClawユーザーはこれらのスキルを自分のインスタンスに直接インストールして、コーディングセッションの品質を即座に向上させることができます。

MyClaw.aiオープンソースエコシステムには以下も含まれます：

- **[openclaw-coding-skills](https://github.com/LeoYeAI/openclaw-coding-skills)** — 構造化されたコーディング行動システム（本リポジトリ）
- **[openclaw-guardian](https://github.com/LeoYeAI/openclaw-guardian)** — セキュリティ監視と保護
- **[openclaw-auto-dream](https://github.com/LeoYeAI/openclaw-auto-dream)** — 認知記憶の整理
- **[myclaw-backup](https://github.com/LeoYeAI/myclaw-backup)** — インスタンスの完全バックアップと復元
- **[myclaw-bench](https://github.com/LeoYeAI/myclaw-bench)** — エージェント能力ベンチマーク

すべてオープンソース。すべて同じ目標のために：AIエージェントを実際の仕事でより信頼でき、より有用にすること。

---

このプロジェクトは「モデルをより賢く」するのではなく、「エージェントを実際のコーディングタスクでより成熟させる」ものです。ワークフロースキル、スペシャリストスキル、実行リファレンス、トリガーマッピング、評価サンプル、チューニングループを使って、ドリフトしやすいコーディング行動を、より安定的で、検証可能で、再利用可能な実行システムに変換します。

## このプロジェクトが提供するもの

- ワークフロースキル：`spec`、`plan`、`build`、`test`、`review`、`ship`
- スペシャリストスキル：`debug`、`security`、`frontend`、`docs`、`deploy`、`refactor`
- `references/` — 実行リファレンス：重要な意思決定ポイントでエージェントの推測と誤判断を減らす
- `TRIGGER-MATRIX`：自動トリガーの命中率と境界ケースの明確さを向上
- `examples/`：トリガー品質を校正するためのリアルなリクエストサンプル
- `evaluation/`：ラベル付き評価セット、曖昧サンプル、dry-run検証、live検証、チューニングループ

つまり、これは単一のプロンプトでもスキルの寄せ集めでもなく、実際のコーディングワークフローを中心に構築された行動最適化システムです。

## 中核的価値

改善するのはモデルの重みではなく、コーディング行動の品質です。

多くのエージェントがソフトウェア開発で失敗するのは、コードを書けないからではなく、実行方法が十分に成熟していないからです：スコープを定義せずに着手、変更範囲が大きすぎ、証拠が弱すぎ、レビューとテストが混在、高リスクタスクに十分な構造がない。

このプロジェクトの価値は、これらの失敗パターンを体系的に削減することです：

- まずスコープを定義してからコーディング
- 一度にすべてではなく、小さなステップで進む
- 完了を宣言する前に十分な証拠を要求
- debug、セキュリティ、デプロイ、リファクタリングを高リスクシナリオとして構造的に処理
- サンプル、評価、live検証を通じて継続的に最適化

## 対象者

- OpenClawでより安定したコーディング結果を求めるチーム
- エンジニアリング標準を再利用可能なスキルとして定着させたいチーム
- エージェントの行動を継続的にチューニングしたいチーム — プロンプトの調整だけでなく

## エントリーポイント

- 英語メインドキュメント：[README.md](./README.md)
- インストールガイド：[INSTALL.md](./INSTALL.md)
- 導入ガイド：[ADOPTION-GUIDE.md](./ADOPTION-GUIDE.md)
- トリガーマッピング：[skills/TRIGGER-MATRIX.md](./skills/TRIGGER-MATRIX.md)
- タスク例：[examples/README.md](./examples/README.md)
- 評価とチューニング：[evaluation/README.md](./evaluation/README.md)
