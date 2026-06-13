# STATUS.md — asset-simulator（資産形成シミュレーター）

更新日: 2026-06-13

## 進捗
80%

## ゴール
☑ 7-1. 資産形成シミュレーター — Codexからコード移管済み。GitHub Pagesで公開済み。

## 現在地
Codexで作成した資産形成シミュレーターを `C:\Users\makki\asset-simulator\index.html` にコピー済み。
単一HTMLの静的Webアプリとして動作する。

公開URL:
`https://makkinngami-cmd.github.io/asset-simulator/`

GitHub:
`https://github.com/makkinngami-cmd/asset-simulator`

## 直近の完了（2026-06-13時点）
- Codex側で資産形成シミュレーターのHTMLモックを作成
- 元本、毎月積立、運用期間、想定利回りを入力できるUIを実装
- 目標金額から必要な毎月積立額を逆算するモードを実装
- 税金ON/OFFを実装
- 元本・積立額合計・利息合計の積み上げ棒グラフを実装
- 最終的な積立金の内訳を円グラフで表示
- 利回りの誤差を±%で指定し、棒グラフにエラーバーとして表示
- 年ごとの推移テーブルを実装
- GitHub Pages向けに `index.html` として移管
- 公開用に `README.md`、`.nojekyll`、`PUBLISH_GITHUB_PAGES.md` を追加
- `index.html` のタイトルから「モック」を外し、免責文を公開向けに調整
- GitHubに `asset-simulator` リポジトリを作成
- GitHub Pagesを有効化し、公開URLでHTTP 200を確認
- 手数料ON/OFFを削除し、手数料は利回り誤差に含めて考える方針に変更

## 次にやること
1. スマホ表示と入力変更時のグラフ表示を再確認する ／ Claude
2. 必要ならOGP、favicon、説明文を追加する ／ Claude
3. 必要なら独自ドメイン設定を検討する ／ ユーザー

## タイムスケジュール
- 随時 | GitHub Pages公開準備 | Claude
- 随時 | UI改善・計算ロジック調整 | Claude

## 注意・触ってはいけないもの
- `STATUS.md` の固定見出しを変更しない
- 金融・投資判断に見えるため、免責文を削らない
