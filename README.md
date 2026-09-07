# Portfolio

個人開発で取り組んだ課題、設計・技術選定、検証、学びをまとめるポートフォリオです。

## プロジェクト

### [AI Incident Investigator](projects/ai-incident-investigator/README.md)

ログ・メトリクス・デプロイ履歴から、根拠をたどれる調査レポートを作るローカルの障害調査支援ツールです。React / TypeScript、FastAPI / Python、LangGraphを使い、原因候補と観測事実の区別、入力イベントへの移動、保存後の再確認を実装しました。

[紹介記事を読む：画面デモ・構成図・設計判断・検証と学び](projects/ai-incident-investigator/README.md)

### [Career Research Agent](projects/career-research-agent/README.md)

企業名や公開求人URLから出典付きレポートを作り、保存・再表示できる個人用ツールです。SvelteKit / TypeScript、SQLite / Drizzle、Responses API / Web Searchを使い、構成の簡略化、有料APIの呼び出し制御、保存失敗からの復旧と生成内容の検証に取り組みました。

[紹介記事を読む：架空データの画面・構成図・費用と保存の設計・検証の限界](projects/career-research-agent/README.md)

## 掲載する内容

- プロジェクトの背景と解決したい課題
- アーキテクチャ、技術選定、設計判断とその理由
- 公開用の画面キャプチャとデモ
- 検証結果、制約、改善点
- 自身の担当範囲とAI支援の活用方法

## 公開方針

このリポジトリではプロジェクトの紹介資料を公開します。実装コードは非公開リポジトリで管理します。

画面キャプチャとデモには公開用の合成データを使用し、実運用データ、個人情報、APIキー、環境変数の設定値は掲載しません。

検証結果には対象と条件を添え、合成データでの検証と実運用で確認できたことを区別して記載します。

## このリポジトリの作業ルール

編集はIssue・featureブランチ・PRで管理します。作業指示は[AGENTS.md](AGENTS.md)、公開資料の判断記録は[docs/decisions.md](docs/decisions.md)を参照してください。Claude Codeも[CLAUDE.md](CLAUDE.md)から同じ作業指示を読み込みます。
