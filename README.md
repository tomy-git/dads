<!-- SPDX-License-Identifier: MPL-2.0 -->

# DADS Skill

デジタル庁デザインシステム（DADS）を参照して、アクセシブルなWebサイト、Webアプリ、行政・公共系UIの設計・実装・レビューを支援するCodex/Claude向けSkillです。

このSkillは、DADS公式Webサイト、Storybook、GitHubコードスニペットを一次情報として扱います。公式MCPサーバーとFigmaデザインデータは使用しません。

## 用途

- DADSを踏まえたWeb UIの設計方針整理
- 行政・公共系サービス向けのアクセシブルな画面設計
- DADSコンポーネントの選定
- HTML/CSS/JavaScript版コードスニペットの参照
- React/Tailwind CSS版コードスニペットの参照
- 既存UIのアクセシビリティ、レスポンシブ、実装方針レビュー

## 使い方

CodexまたはClaudeで、このSkillを有効化してから依頼してください。

例:

```text
Use $dads to build an accessible public-sector web UI with the Digital Agency Design System.
```

日本語では、次のように依頼できます。

```text
$dads を使って、自治体向け申請フォームのUIをDADSに沿って設計してください。
```

## 配布zipの使い方

`dist/` には、配布先ごとに内容を分けたzipファイルを置きます。

- `dist/dads-codex.zip`: Codex向け。`SKILL.md`、`LICENSE`、`references/`、`agents/openai.yaml` を含みます。
- `dist/dads-claude-code.zip`: Claude Code向け。`SKILL.md`、`LICENSE`、`references/` を含みます。

どちらのzipも、展開すると `dads/` フォルダが作られる構成です。zipインポートに対応している環境では、対象に合うzipファイルをそのまま指定してください。ローカルのSkillディレクトリへ配置する環境では、zipを展開して作成された `dads/` フォルダを、その環境のSkill配置先へ置いてください。

Codexで使う場合:

```text
dist/dads-codex.zip
```

Claude Codeで使う場合:

```text
dist/dads-claude-code.zip
```

配布zipにはGitHub閲覧用の `README.md` は含めていません。Skillとして読み込ませる実体は、各zip内の `dads/SKILL.md` と `dads/references/` です。

## 構成

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
│   ├── checklist.md
│   ├── components.md
│   ├── foundations.md
│   ├── implementation-resources.md
│   └── site-map.md
├── dist/
│   ├── dads-claude-code.zip
│   └── dads-codex.zip
├── LICENSE
└── README.md
```

## 参照ファイル

- `SKILL.md`: Skill本体の指示、実行フロー、禁止事項
- `references/site-map.md`: DADS公式サイト、Storybook、GitHubリポジトリの索引
- `references/foundations.md`: カラー、タイポグラフィ、余白、レイアウトなど基本デザインの要点
- `references/components.md`: DADSコンポーネントの用途別索引
- `references/implementation-resources.md`: HTML版、React版、Tailwindテーマプラグインの参照先と確認手順
- `references/checklist.md`: 実装・レビュー・完了報告前の確認項目
- `agents/openai.yaml`: OpenAI向けSkill表示情報

## 基本方針

1. 依頼内容をページ全体、基本デザイン、個別コンポーネント、実装コード、レビューのいずれかに分類します。
2. `references/site-map.md` で公式ソースと現在のサイト構成を確認します。
3. 基本デザインは `references/foundations.md`、コンポーネント選定は `references/components.md` を参照します。
4. 実装へ落とし込む場合は `references/implementation-resources.md` を確認します。
5. 完了前に `references/checklist.md` でアクセシビリティ、レスポンシブ、出典・ライセンスを確認します。

## 注意事項

- `references/` は2026-06-17時点の索引と実務メモです。公式サイトのバージョン、更新日、提供状況が回答や実装判断に影響する場合は、該当する公式ページを最新状態で確認してください。
- DADSをそのまま個別サービスのブランドとして扱わず、対象サービスの情報設計、利用者、既存UI基盤に合わせてWeb実装向けのスタイル方針へ落とし込んでください。
- Figmaデザインデータを前提にした判断は、このSkillではDADS公式準拠として断定しません。
- コードスニペットを使う場合も、そのまま貼り付けず、既存プロジェクトの命名、責務分離、状態管理、CSS方針、テスト方針に合わせて移植してください。

## ライセンス

このSkillはMozilla Public License Version 2.0（MPL-2.0）でライセンスされています。詳細は `LICENSE` を参照してください。
