<!-- SPDX-License-Identifier: MPL-2.0 -->

# Components

コンポーネントを選ぶときに読む。各ページは、ある場合は「概要」「使い方」「アクセシビリティ」「各種リソース」の順に確認する。

## 読み方

1. 用途別索引で候補を絞る。
2. 公式ページの概要でユースケースと注意が必要なケースを確認する。
3. 使い方タブがある場合は、配置、状態、組み合わせ、悪い例を確認する。
4. アクセシビリティタブがある場合は、キーボード操作、ARIA、ラベル、フォーカス、コントラストを確認する。
5. 各種リソースのStorybook/GitHubリンクからHTML版またはReact版の実装を確認する。
6. ガイドライン準備中のページは、Storybook/GitHubと一般的なHTML semantics/WCAG/WAI-ARIAで暫定補完する。DADS固有ガイドラインとして未確認の事項は、準拠済みと断定しない。

## 入力フォーム

| コンポーネント | URL | 使う場面 |
| --- | --- | --- |
| インプットテキスト | https://design.digital.go.jp/dads/components/input-text/ | 名前、電話番号など1行以内のテキスト入力 |
| テキストエリア | https://design.digital.go.jp/dads/components/textarea/ | 複数行の自由記述 |
| セレクトボックス | https://design.digital.go.jp/dads/components/select/ | 複数選択肢から1つを選ぶ標準的なフォーム |
| コンボボックス | https://design.digital.go.jp/dads/components/combobox/ | 入力支援や選択支援を伴う複合的な選択操作 |
| チェックボックス | https://design.digital.go.jp/dads/components/checkbox/ | 複数選択、同意、オン/オフの集合 |
| ラジオボタン | https://design.digital.go.jp/dads/components/radio/ | 相互排他的な選択肢から1つを選ぶ |
| 日付ピッカー／カレンダー | https://design.digital.go.jp/dads/components/date-picker/ | 日付入力、カレンダー選択 |
| ファイルアップロード／ドロップエリア | https://design.digital.go.jp/dads/components/file-upload/ | 単体または複数ファイルのアップロード |
| 検索ボックス | https://design.digital.go.jp/dads/components/search-box/ | サイト内検索、詳細検索、キーワードショートカット |
| ボタン | https://design.digital.go.jp/dads/components/button/ | アクション実行、フォーム送信、ページ遷移のトリガー |

## ナビゲーション

| コンポーネント | URL | 使う場面 |
| --- | --- | --- |
| パンくずリスト | https://design.digital.go.jp/dads/components/breadcrumb/ | 階層内の現在位置を示す |
| 水平メニュー | https://design.digital.go.jp/dads/components/horizontal-menu/ | 上位ナビゲーション、ページ誘導 |
| メガメニュー | https://design.digital.go.jp/dads/components/mega-menu/ | 水平メニューから大きなドロップダウン領域を表示 |
| メニューリスト | https://design.digital.go.jp/dads/components/menu-list/ | メニューアイテムを束ねる |
| メニューリストボックス | https://design.digital.go.jp/dads/components/menu-list-box/ | ラベル付きオープナーでメニューリストを開閉 |
| モバイルメニュー | https://design.digital.go.jp/dads/components/mobile-menu/ | タッチスクリーン向けメニュー |
| ハンバーガーメニューボタン | https://design.digital.go.jp/dads/components/hamburger-menu-button/ | モバイルメニューやドロワーのトリガー |
| ドロワー | https://design.digital.go.jp/dads/components/drawer/ | 画面端から展開するコンテナ |
| ボトムナビゲーション | https://design.digital.go.jp/dads/components/bottom-navigation/ | モバイル等で2から5個の目的地へ移動 |
| ページナビゲーション | https://design.digital.go.jp/dads/components/page-navigation/ | 前後ページや複数ページ遷移 |
| ステップナビゲーション | https://design.digital.go.jp/dads/components/step-navigation/ | 手続きのステップ、進行状況、完了までの俯瞰 |
| スクロールトップボタン | https://design.digital.go.jp/dads/components/scroll-top-button/ | ページ先頭への移動 |
| ユーティリティリンク | https://design.digital.go.jp/dads/components/utility-link/ | ヘッダー等の補助的リンク群 |
| ランゲージセレクター | https://design.digital.go.jp/dads/components/language-selector/ | 表示言語の選択 |

## 情報表示と構造

| コンポーネント | URL | 使う場面 |
| --- | --- | --- |
| 見出し | https://design.digital.go.jp/dads/components/heading/ | ページやセクションの主題を示す |
| カード | https://design.digital.go.jp/dads/components/card/ | 単一主題のコンテンツをまとめる |
| 説明リスト | https://design.digital.go.jp/dads/components/description-list/ | 名前と値、説明したいことと説明文のペア |
| 箇条書きリスト | https://design.digital.go.jp/dads/components/list/ | 1つ以上の項目を列挙 |
| 引用ブロック | https://design.digital.go.jp/dads/components/blockquote/ | 段落単位の引用 |
| 画像 | https://design.digital.go.jp/dads/components/image/ | ページ中に画像を埋め込む |
| リソースリスト | https://design.digital.go.jp/dads/components/resource-list/ | 共通した複数オブジェクトのリスト |
| テーブル／データテーブル | https://design.digital.go.jp/dads/components/table/ | 行と列で構造化されたデータ表示、比較、大量データ操作 |
| テーブルコントロール | https://design.digital.go.jp/dads/components/table-control/ | データテーブルの絞り込み、表示制御、操作群 |
| ディバイダー | https://design.digital.go.jp/dads/components/divider/ | セクションやコンテンツグループの区切り |

## 開閉・状態・補助表示

| コンポーネント | URL | 使う場面 |
| --- | --- | --- |
| アコーディオン | https://design.digital.go.jp/dads/components/accordion/ | 同種セクションが連続し、各ボディを折りたたむ |
| ディスクロージャー | https://design.digital.go.jp/dads/components/disclosure/ | メイン情報への追加・補足情報を折りたたむ |
| タブ | https://design.digital.go.jp/dads/components/tab/ | 関連するタブパネルを切り替える |
| モーダルダイアログ | https://design.digital.go.jp/dads/components/dialog/ | 重要情報、決定、選択を求めるダイアログ |
| チップタグ | https://design.digital.go.jp/dads/components/chip-tag/ | 任意情報をアイテム化し、表示・削除しやすくする |
| チップラベル | https://design.digital.go.jp/dads/components/chip-label/ | 状態や分類を短いラベルで示す |
| プログレスインジケーター | https://design.digital.go.jp/dads/components/progress-indicator/ | 処理中・進行中を通知 |
| ノティフィケーションバナー | https://design.digital.go.jp/dads/components/notification-banner/ | サイト全体またはページ/要素単位の重要通知 |
| 緊急時バナー | https://design.digital.go.jp/dads/components/emergency-banner/ | 通常コミュニケーションを中断してでも注意喚起すべき緊急情報 |

## メディア

| コンポーネント | URL | 使う場面 |
| --- | --- | --- |
| イメージスライダー | https://design.digital.go.jp/dads/components/image-slider/ | 複数画像を切り替えて見るギャラリー的表示 |
| カルーセル | https://design.digital.go.jp/dads/components/carousel/ | 複数スライドを順番に表示。使いどころに注意する |

## ページ骨格

| コンポーネント | URL | 使う場面 |
| --- | --- | --- |
| ヘッダーコンテナ | https://design.digital.go.jp/dads/components/header-container/ | ロゴ、検索、リンク、言語選択、水平メニュー、ハンバーガーボタン等を格納 |

## 選定メモ

- アコーディオンは同種の複数セクション向け。単に省スペースにしたいだけなら使わない。
- ディスクロージャーはセクション内の追加・補足情報向け。セクション全体の折りたたみはアコーディオンを検討する。
- 表組みデータにはテーブル、名前と値の単純なペアには説明リストを検討する。
- フォームコントロールはラベル、サポートテキスト、エラーテキスト、必須/任意、入力制約をセットで設計する。
- ボタンは重要度でスタイルを分ける。ひとつの画面でプライマリーを乱用しない。
- disabledの多用は避ける。操作できない理由を説明し、押下後に不足を案内できないか検討する。
- カルーセルやイメージスライダーは、重要情報を隠さない。停止、キーボード操作、読み上げ順を必ず確認する。
- 緊急時バナーは本来のコミュニケーションを中断してでも必要な場合に限定する。
- ガイドライン準備中のページでも、各種リソースにHTML版/React版実装が提供されている場合がある。公式ページの提供状況を確認し、Figma内ガイドラインだけで確認できる内容は未確認事項として報告する。
