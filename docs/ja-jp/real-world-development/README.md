---
title: "実践的な開発"
slug: ja-jp/real-world-development
authors:
  - geektrainer
lastUpdated: 2026-09-16
---

現実的なシナリオ、完成したアプリケーション、共有バックログを使って、ソフトウェア開発ライフサイクル全体で GitHub Copilot を活用します。変更の計画、コードの作成、動作のテスト、プルリクエストのレビュー、エージェントを使った作業の管理を繰り返しながら進めます。

## シナリオ

開発をテーマにしたボードゲームのクラウドファンディングを提供する架空の会社、Tailspin Toys の新しい開発者として作業します。チームのバックログは GitHub Issue として登録されており、取り組む項目を選べます。フィルターやページネーションなどの機能作業に加え、アクセシビリティやコーディング規約などの品質改善も含まれています。

## 作業環境を選択する

GitHub Copilot は、どの環境で作業していても利用できます。開発に使う環境を選択してください。各ワークショップは個別のセットアップから始まり、共通の Tailspin Toys シナリオを使用します。

### [GitHub Copilot CLI][cli]

ターミナルでエージェント型アシスタントを使います。Plan モードと Autopilot モード、指示、スキル、カスタムエージェント、Playwright MCP、Agent Merge、便利なスラッシュコマンドを活用します。

### [GitHub Copilot アプリ][app]

エージェントセッションを並行して実行し、セッションモードを切り替え、Canvas で共同作業し、デスクトップアプリから GitHub Issue とプルリクエストを管理します。

### [GitHub Copilot cloud agent][cloud]

GitHub Issue を非同期エージェントに割り当て、作業を案内し、進行状況を監視して、エージェントが作成したプルリクエストをレビューします。

### [Visual Studio Code][vscode]

Visual Studio Code と GitHub Codespaces で GitHub Copilot を使います。エディターを離れずに、Copilot Chat のエージェント モード、MCP サーバー、カスタム エージェントを活用します。

[cli]: cli/
[app]: app/
[cloud]: cloud/
[vscode]: vscode/
