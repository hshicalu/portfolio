# Portfolio

個人開発で取り組んだ課題、設計・技術選定、検証、学びをまとめるポートフォリオです。

## プロジェクト

### [AI Incident Investigator](projects/ai-incident-investigator/README.md)

ログ・メトリクス・デプロイ履歴から、根拠をたどれる調査レポートを作るローカルの障害調査支援ツールです。React / TypeScript、FastAPI / Python、LangGraphを使い、原因候補と観測事実の区別、入力イベントへの移動、保存後の再確認を実装しました。

[紹介記事を読む：画面デモ・構成図・設計判断・検証と学び](projects/ai-incident-investigator/README.md)

### [Career Research Agent](projects/career-research-agent/README.md)

企業名や公開求人URLから出典付きレポートを作り、保存・再表示できる個人用ツールです。SvelteKit / TypeScript、SQLite / Drizzle、Responses API / Web Searchを使い、構成の簡略化、有料APIの呼び出し制御、保存失敗からの復旧と生成内容の検証に取り組みました。

[紹介記事を読む：架空データの画面・構成図・費用と保存の設計・検証の限界](projects/career-research-agent/README.md)

### [GitHub Planning Agent](projects/github-planning-agent/README.md)

GitHub Issueとコードから根拠付きの実装計画を作ることを目指した技術検証プロトタイプです。Next.js / TypeScript、OpenAI Agents SDK、Octokitを使い、固定コミットの引用検証、APIの実行予算、失敗の記録に取り組みました。実計画の有用性は未確認で、現在の実装と実評価からの学びを紹介します。

[紹介記事を読む：合成サンプルの画面・構成図・根拠と予算の設計・未検証事項](projects/github-planning-agent/README.md)

### [Local Codebase Navigator](projects/local-codebase-navigator/README.md)

非公開コードをローカルで解析し、関連ファイルと根拠をエディター内で確認するVS Code拡張です。TypeScript、Tree-sitter、SQLite FTS、任意のOllama文章化を使い、候補の説明可能性、中止後の復帰、保存と処理ホストの境界に取り組みました。

[紹介記事を読む：操作例・構成・設計判断・検証と残課題](projects/local-codebase-navigator/README.md)

### [Private Interview Coach](projects/private-interview-coach/README.md)

職務経歴や開発記録を基に、端末内のLLMが回答を深掘りするテキスト模擬面接の技術プロトタイプです。SvelteKit / TypeScript、SQLite / Drizzle、Ollamaを使い、原文引用の検証、アプリ側の対話状態管理、保存・再表示に取り組みました。合成ケースの実モデル評価と、生成品質に残る課題を紹介します。

[紹介記事を読む：実モデルの合成画面・構成図・根拠と状態の設計・評価と限界](projects/private-interview-coach/README.md)

### [Local Spec Reviewer](projects/local-spec-reviewer/README.md)

短い仕様書・議事録を端末内のLLMで比較し、両方の原文を確認して指摘の採否を保存するMVPです。SvelteKit / TypeScript、SQLite / Drizzle、Ollamaを使い、根拠IDの検証、原文からの引用、再推論なしの復元に取り組みました。検出品質は評価継続中で、40回の実モデル評価と改善候補を不採用にした理由も紹介します。

[紹介記事を読む：保存済み実モデル出力の画面・構成図・根拠と保存の設計・評価と限界](projects/local-spec-reviewer/README.md)

### [Local Data Workbench](projects/local-data-workbench/README.md)

日本語の質問を端末内のLLMで分析計画に変え、人が確認してからCSVを集計する技術プロトタイプです。SvelteKit / TypeScript、Ollama、DuckDB、SQLiteを使い、許可した計画からのSQL生成、元行の確認、再推論なしの再表示に取り組みました。実モデルの固定12/12・独立5/6という評価と、意味解釈に残る限界を紹介します。

[紹介記事を読む：実モデルの集計画面・構成と設計判断・改善と失敗・開発の区切り](projects/local-data-workbench/README.md)

### [Private Voice Journal](projects/private-voice-journal/README.md)

録音済みの音声メモを端末内で文字起こしし、実施内容・判断理由・困りごと・次の行動へ整理する技術プロトタイプです。SvelteKit / TypeScript、whisper.cpp、Ollama、SQLiteを使い、認識原文と修正版、生成した記録の版を分けて保存します。合成音声6ケースの実モデル評価と、モデル選定・誤認識・情報の抜けから得た学びを紹介します。

[紹介記事を読む：実生成の保存画面・構成と版管理・モデル比較・実測と限界](projects/private-voice-journal/README.md)

### [Local Feedback Analyst](projects/local-feedback-analyst/README.md)

問い合わせCSVを端末内のLLMで課題別に分類し、原文を確認しながら人が修正する個人開発プロトタイプです。SvelteKit / TypeScript、SQLite / Drizzle、Ollamaを使い、課題抽出・類似候補検索・分類判断の分離、再分析からの修正保護、保存・出力に取り組みました。合成10件の実モデル評価と、情報不足への過剰分類や処理時間の限界も紹介します。

[紹介記事を読む：操作例と実結果の修正画面・構成図・分類と保存の設計・評価と限界](projects/local-feedback-analyst/README.md)

### [Local File Organizer](projects/local-file-organizer/README.md)

文書の内容から端末内のLLMが分類・名前を提案し、確認した操作だけを実行・取り消しできるmacOS向け技術プロトタイプです。Tauri 2 / Svelte / Rust、Ollama、SQLiteを使い、計画後の変更検知、上書き拒否、履歴と取り消しに取り組みました。実モデル評価と実アプリの操作結果、理由・引用の誤りや未検証の制約を紹介します。

[紹介記事を読む：実アプリの画面・構成と安全性・実モデル評価・失敗と限界](projects/local-file-organizer/README.md)

### [Local Test Data Studio](projects/local-test-data-studio/README.md)

日本語の条件とスキーマから、端末内のLLMで架空のテストデータを作る技術プロトタイプです。SvelteKit / TypeScript、Ollama、Ajv、SQLiteを使い、意図的な異常と期待外の違反の区別、部分再生成候補の採否、修正と保存・出力に取り組みました。実モデルの評価と、重複候補を不採用にして元の行を保持した結果、意味品質と件数の限界を紹介します。

[紹介記事を読む：実生成と保存再表示の画面・構成図・制約検証と修正保護・実測と限界](projects/local-test-data-studio/README.md)

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
