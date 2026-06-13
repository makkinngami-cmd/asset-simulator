# asset-simulator — Claude Code入口

## このプロジェクトについて

資産形成シミュレーターの静的Webアプリ。
Money Forward系の利回りシミュレーション画面を参考に、CodexでHTMLプロトタイプを作成したものをこのフォルダへ移管した。

## 現在の実体ファイル

- `index.html`
  - 単一HTMLファイル
  - HTML/CSS/JavaScriptをすべて内包
  - 外部API、DB、ビルド工程なし
  - GitHub Pagesでそのまま公開可能

## 担当ゴール

| ゴール | フォルダ |
|---|---|
| 7-1. 資産形成シミュレーター | `goals/7-1_asset_simulator/` |

## セッション開始時に読むもの

1. この `CLAUDE.md`
2. `STATUS.md`
3. `goals/7-1_asset_simulator/SESSION.md`
4. `goals/7-1_asset_simulator/HANDOFF.md`
5. `index.html`

## セッション終了時に更新するもの

1. `STATUS.md`（担当ゴール部分のみ）
2. `goals/7-1_asset_simulator/HANDOFF.md`
3. `goals/7-1_asset_simulator/WORKLOG.md`

## 起動・確認方法

このフォルダで以下を実行する。

```powershell
python -m http.server 4173
```

ブラウザで開く。

```text
http://localhost:4173/
```

`index.html` は直接ブラウザで開いても動くが、GitHub Pages想定の確認ではHTTPサーバー経由を推奨。

## 注意・触ってはいけないもの

- `STATUS.md` の固定見出しを変更しない（morning_report.py が壊れる可能性がある）
- 新しいゴールはユーザー承認後に追加する
- 既存ファイルの削除、リネーム、移動、大きな上書きはユーザー確認を取る
- 金融シミュレーションなので、公開時は免責文を残す

## 公開方針

GitHub Pagesで公開する想定。
最小構成は以下。

```text
asset-simulator/
  index.html
  CLAUDE.md
  STATUS.md
  goals/
```

GitHub Pagesでは `index.html` がトップページになる。
