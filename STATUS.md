# STATUS.md — asset-simulator（資産形成シミュレーター）

更新日: 2026-06-13

## 進捗
60%

## ゴール
☑ 7-1. 資産形成シミュレーター — Codexからコード移管済み。GitHub Pages公開に向けて調整・保守を進める。

## 現在地
Codexで作成した資産形成シミュレーターを `C:\Users\makki\asset-simulator\index.html` にコピー済み。
単一HTMLの静的Webアプリとして動作する。

## 直近の完了（2026-06-13時点）
- Codex側で資産形成シミュレーターのHTMLモックを作成
- 元本、毎月積立、運用期間、想定利回りを入力できるUIを実装
- 目標金額から必要な毎月積立額を逆算するモードを実装
- 税金ON/OFF、手数料ON/OFFを実装
- 元本・積立額合計・利息合計の積み上げ棒グラフを実装
- 最終的な積立金の内訳を円グラフで表示
- 利回りの誤差を±%で指定し、棒グラフにエラーバーとして表示
- 年ごとの推移テーブルを実装
- GitHub Pages向けに `index.html` として移管
- 公開用に `README.md`、`.nojekyll`、`PUBLISH_GITHUB_PAGES.md` を追加
- `index.html` のタイトルから「モック」を外し、免責文を公開向けに調整

## 次にやること
1. GitHub CLIにログインする ／ ユーザー
2. GitHubリポジトリを作成してpushする ／ Claude
3. GitHub Pagesで公開する ／ Claude
4. 公開URLで動作確認する ／ Claude
5. スマホ表示と入力変更時のグラフ表示を再確認する ／ Claude

## タイムスケジュール
- 随時 | GitHub Pages公開準備 | Claude
- 随時 | UI改善・計算ロジック調整 | Claude

## 注意・触ってはいけないもの
- `STATUS.md` の固定見出しを変更しない
- 金融・投資判断に見えるため、免責文を削らない
