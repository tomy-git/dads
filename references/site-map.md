<!-- SPDX-License-Identifier: MPL-2.0 -->

# Site Map

2026-06-17時点の索引。回答、設計、レビュー、実装判断に影響する場合は、必ず公式ページを開いて最新のバージョン、更新日、提供状況を確認する。

## 公式入口

- デジタル庁デザインシステムβ版: https://design.digital.go.jp/dads/
- 2026-06-17確認時のトップ表記: v2.14.1
- 本体は、デザイン言語、UIコンポーネント、ユーザビリティとアクセシビリティのガイドラインで構成される。
- 想定利用先は、官公庁、地方自治体、公共性の高い組織等のWebサイト、Webアプリケーション、オンラインサービス、システム等。

## 使用しないもの

- 公式MCPサーバー: このSkillでは使わない。
- Figma Community/デザインデータ: 公式ページにリンクがあっても使わない。

このSkillを使う環境では公式MCPサーバーとFigmaにアクセスできない。公式手順がFigmaデザインデータの参照を要求するスタイルガイド作成や、Figma内ガイドラインだけで確認できる事項は、DADS公式準拠として断定せず、Web実装向けの方針整理や暫定補完として扱う。

## 使用してよい一次情報

- DADS公式Webサイト: https://design.digital.go.jp/dads/
- HTML版Storybook: https://design.digital.go.jp/dads/html/
- React版Storybook: https://design.digital.go.jp/dads/react/
- HTML版GitHub: https://github.com/digital-go-jp/design-system-example-components-html
- React版GitHub: https://github.com/digital-go-jp/design-system-example-components-react
- Tailwindテーマプラグイン: https://github.com/digital-go-jp/tailwind-theme-plugin

## セクション

| セクション | URL | 使う場面 |
| --- | --- | --- |
| はじめに | https://design.digital.go.jp/dads/introduction/ | 利用前提、注意事項、出典・ライセンスを確認する |
| ガイダンス | https://design.digital.go.jp/dads/guidance/ | 導入方針、アクセシビリティ、スタイルガイド作成方針を確認する |
| 基本デザイン | https://design.digital.go.jp/dads/foundations/ | 色、文字、余白、レイアウトなどの視覚基盤を決める |
| コンポーネント | https://design.digital.go.jp/dads/components/ | UI部品の用途、仕様、使い方、アクセシビリティ、実装リソースを確認する |
| リソース | https://design.digital.go.jp/dads/resources/ | Storybook、GitHubコードスニペット、Tailwindプラグイン、関連資料を確認する |
| お知らせ | https://design.digital.go.jp/dads/updates/ | 変更履歴、提供状況、名称変更、コードスニペット更新を確認する |

## 導入時に読む順序

1. `introduction/notices/` で利用条件、出典、コードスニペットのライセンスを確認する。
2. `guidance/accessibility/` でアクセシビリティ優先の考え方を確認する。
3. `guidance/style-guides/` でDADSを個別サービスへ再定義する考え方を確認する。ただし、Figmaデザインデータを使う公式手順は実行せず、Web実装向けのスタイル方針整理に限定する。
4. `foundations/` で色、文字、余白、レイアウト、リンク、アイコンを決める。
5. `components/` で具体的なUI部品を選ぶ。
6. `resources/` からStorybook/GitHubコードスニペットを確認する。

## 重要な前提

- DADSはプラットフォーム型デザインシステムであり、個別サイトのブランドや情報設計に合わせてスタイル方針へ落とし込む必要がある。
- DADSを使ってもコンテンツ自体のアクセシビリティは自動的に担保されない。文言、情報設計、運用設計、実装品質は各プロジェクトで確認する。
- 公式ページにはJIS X 8341-3:2016、WCAG 2.2、WAI-ARIA等への参照が含まれる。該当コンポーネントのアクセシビリティタブを優先して読む。
