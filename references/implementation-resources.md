<!-- SPDX-License-Identifier: MPL-2.0 -->

# Implementation Resources

公式MCPサーバーとFigmaを使わず、Web実装に必要な公式情報だけを参照する。

## リソース入口

- リソース: https://design.digital.go.jp/dads/resources/
- HTML版GitHub: https://github.com/digital-go-jp/design-system-example-components-html
- HTML版Storybook: https://design.digital.go.jp/dads/html/
- React版GitHub: https://github.com/digital-go-jp/design-system-example-components-react
- React版Storybook: https://design.digital.go.jp/dads/react/
- Tailwindテーマプラグイン: https://github.com/digital-go-jp/tailwind-theme-plugin
- npm: https://www.npmjs.com/package/@digital-go-jp/tailwind-theme-plugin

## HTML版コードスニペット

対象:

- プレーンHTML/CSS/JavaScript。
- フレームワーク非依存で既存サイトに後付けする場合。
- サーバーサイドテンプレート、静的サイト、CMSテンプレートへ移植する場合。

公式README上の構成:

- `src/components/`: 各コンポーネント。
- `src/docs/`: ドキュメント。
- `src/helpers/`: ユーティリティ。
- `src/global.css`: グローバルスタイル。
- 各コンポーネントにはCSS、HTMLサンプル、必要なJavaScript、Storybookストーリー、MDXドキュメントが含まれる。

確認手順:

1. 公式コンポーネントページの各種リソースからHTML版ソースコードとStorybookを開く。
2. Storybookで状態、サイズ、キーボード操作、エラー表示、レスポンシブを確認する。
3. GitHubの該当コンポーネントディレクトリからHTML/CSS/JSを確認する。
4. 既存プロジェクトの命名、CSSスコープ、ビルド、アクセシビリティテストに合わせて移植する。

## React版コードスニペット

対象:

- React/Tailwind CSS/TypeScriptのプロジェクト。
- DADSのコンポーネント構造をReactコンポーネントとして移植する場合。

公式README上の技術スタック:

- React v18。
- Tailwind CSS v3。
- TypeScript。
- React v19で使う場合は軽微な型エラーが出る可能性があるため、公式READMEとプロジェクト側の型設定を確認する。

公式README上の構成:

- `src/components/`: 各コンポーネント。
- `src/docs/`: ドキュメント。
- `src/tokens/`: デザイントークン。
- `src/index.ts`: エクスポート。
- 各コンポーネントにはTSX本体、Storybookストーリー、`index.ts` が含まれる。

確認手順:

1. 公式コンポーネントページの各種リソースからReact版ソースコードとStorybookを開く。
2. 既存プロジェクトのReact、Tailwind、TypeScript、アクセシビリティライブラリ、フォームライブラリと衝突しないか確認する。
3. コンポーネントのprops、状態、ARIA、イベント処理を読み、既存設計へ合わせる。
4. 公式コードの見た目だけでなく、ラベル、フォーカス、キーボード操作、エラーメッセージ、読み上げを確認する。

## Tailwindテーマプラグイン

パッケージ:

```bash
npm install @digital-go-jp/tailwind-theme-plugin
```

Tailwind CSS v3:

```js
plugins: [require("@digital-go-jp/tailwind-theme-plugin")]
```

Tailwind CSS v4:

```css
@import "tailwindcss";
@import "@digital-go-jp/tailwind-theme-plugin/v4";
```

注意:

- 公式リポジトリの対応表を確認する。2026-06-17確認時点では、README上の対応表はFigma 2.3.0から2.14.0に対してプラグイン1.0.1を示していた。
- DADSトップは同日時点でv2.14.1だったため、v2.14.1との厳密な対応が必要な場合はリリース、README、npmを再確認してから判断する。
- 既存Tailwind設定、contentパス、prefix、theme.extend、CSS変数方針と衝突しないように導入する。

## 利用条件と出典

- デザインシステム本体のコンテンツを利用する場合は、公式の利用上の注意事項に従い出典を記載する。
- コンテンツを編集・加工して利用する場合は、編集・加工したことを示し、デジタル庁が作成したかのように扱わない。
- コードスニペットはGitHubで公開され、MIT Licenseが適用される。
- コードスニペットは編集・加工して利用することが前提のため、編集・加工したUI画面パーツを利用者のWebサイト等で使う場合、出典明記は不要とされている。
- コードスニペットを編集・加工せずに利用・公開する場合は、公式の出典記載例に従う。

## 実装時の注意

- 公式コードスニペットをそのままコピーせず、プロジェクトの責務分離とテスト方針に合わせる。
- 既存コンポーネントライブラリを使う場合は、DADSの用途、アクセシビリティ、見た目、状態表現を満たすようにラップまたは拡張する。
- 公式Storybookで見た状態と、実装後の状態差分をブラウザで確認する。
- React版にない、または提供予定のコンポーネントはHTML版や公式ページを参考に、セマンティックHTMLとWCAG/WAI-ARIA要件を優先して実装する。
