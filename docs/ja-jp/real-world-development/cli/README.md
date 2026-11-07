---
slug: ja-jp/real-world-development/cli
title: "GitHub Copilot CLI"
description: "Copilot CLI のモード、カスタマイズ、MCP ツール、プルリクエストの自動化を学びながら、Tailspin Toys の 2 つの変更を実装、検証、提供します。"
authors:
  - geektrainer
lastUpdated: 2026-09-18
---

**[GitHub Copilot CLI][about-copilot-cli]** は、エージェント型コーディングアシスタントとして GitHub Copilot をターミナルで利用できるようにします。コマンドラインからコードベースの調査、コードの生成、コマンドの実行、外部ツールへの接続ができるため、グラフィカルエディターに切り替えずに作業を続けられます。

このワークショップでは、Tailspin Toys の一連の作業を進めます。

1. GitHub Codespaces でプロジェクトを準備し、Copilot CLI をインストールして使い方を確認します。
2. 星評価を追加し、ブラウザーで結果を確認して、最初のプルリクエスト (PR) を手動でマージします。
3. フィルターの Issue から始め、Plan モードで方針を決め、Autopilot モードで実装し、Interactive モードでレビューします。
4. リポジトリの指示を更新し、フィルターの作業に適用します。
5. 既存の `quality-checks` スキルをカスタマイズし、プロジェクトのチェックを実行します。
6. Playwright Model Context Protocol (MCP) サーバーを追加し、ブラウザーでフィルターの動作を確認します。
7. 要件、テスト範囲、検証結果をレビューする品質保証 (QA) カスタム エージェントを作成します。
8. フィルターの変更全体をレビューし、フィルターの PR に Agent Merge を使用します。
9. コンテキスト、モデル、共有、cloud agent への任意の委任に使えるスラッシュコマンドを確認します。

ワークショップに集中できるよう、PR は 2 つ作成します。1 つ目は星評価、2 つ目はフィルターで、指示とスキルの更新、QA プロファイル、テストを含みます。フィルターと品質に関する作業は、同じ会話とブランチで進めるため、各ツールを試しながら作業を積み重ねられます。

## レッスン

| レッスン | トピック | 説明 |
| ------ | ----- | ----------- |
| [0. 前提条件][ex0] | セットアップ | リポジトリと Codespace を作成します |
| [1. Copilot CLI をインストールする][ex1] | インストール | Copilot CLI をインストールして認証し、使い方を確認します |
| [2. 星評価を追加する: すぐにできる改善][ex2] | 最初の変更 | 既存の評価と未評価時の表示を追加し、最初の PR をマージします |
| [3. エージェント モード: Plan と Autopilot][ex3] | エージェント モード | Issue から機能を計画し、Autopilot で実装して Interactive でレビューします |
| [4. カスタム指示で Copilot を導く][ex4] | コンテキスト | 指示を確認、更新し、フィルターの作業に適用します |
| [5. quality-checks スキルをカスタマイズして使う][ex5] | 繰り返し可能なチェック | 既存のスキルを確認し、レポート形式を変更して実行します |
| [6. Playwright MCP で機能を検証する][ex6] | ブラウザーでの確認 | CLI で MCP を設定し、フィルターの動作を調べます |
| [7. QA エージェントを作成して使う][ex7] | 要件とテスト範囲 | 専門エージェントを作成、選択し、最終的な検証結果を集めます |
| [8. 機能の PR を作成してマージする][ex8] | レビューとマージ | 変更全体をレビューして PR を作成し、Agent Merge を使います |
| [9. GitHub Copilot CLI のスラッシュコマンド][ex9] | CLI 機能 | コンテキスト、モデル、共有、任意の委任を確認します |
| [10. まとめと次のステップ][ex10] | まとめ | ワークフロー、再利用可能なカスタマイズ、その他のリソースを確認します |
| [オプション: Foundry を取り入れる][foundry] | ホスト型エージェント | モデルを準備し、カタログに基づくエージェントをデプロイして Web サイトに接続します |

## 前提条件

このワークショップに参加する前に、次のものを用意してください。

- [ ] 有効な **Copilot Student、Pro、Pro+、Business、Enterprise** プランがある GitHub アカウント
- [ ] リポジトリと Codespace を作成する権限
- [ ] ターミナルまたはコマンドラインの基本的な知識

> [!TIP]
> 有料プランを利用していませんか？認証済みの学生は [GitHub Education][student-plan] を通じて GitHub Copilot を無料で利用できます。**Copilot Student** プランには、このワークショップで使うエージェント、MCP、コードレビュー、Copilot CLI の機能が含まれています。

> [!NOTE]
> Copilot Business または Copilot Enterprise を使用する場合は、管理者が Copilot CLI を有効にしていることを確認してください。

## はじめに

**[前提条件から開始 →][ex0]**

[about-copilot-cli]: https://docs.github.com/copilot/concepts/agents/about-copilot-cli
[student-plan]: https://github.com/education/students
[ex0]: 0-prerequisites/
[ex1]: 1-install-copilot-cli/
[ex2]: 2-add-star-rating/
[ex3]: 3-agent-modes/
[ex4]: 4-custom-instructions/
[ex5]: 5-agent-skills/
[ex6]: 6-mcp-playwright/
[ex7]: 7-qa-agent/
[ex8]: 8-create-pull-request/
[ex9]: 9-cli-power-tools/
[ex10]: 10-review/
[foundry]: 8-foundry-agent/
