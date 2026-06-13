# 7-1. 資産形成シミュレーター セッション指示

## 担当範囲

資産形成シミュレーターの修正、保守、機能追加、GitHub Pages公開準備を担当する。
Codexが作成した単一HTMLをベースに進める。

## 主要ファイル

- `C:\Users\makki\asset-simulator\index.html`
  - 現在のアプリ本体
  - HTML/CSS/JavaScriptを1ファイルに内包
  - GitHub Pagesで公開可能

## 作業開始時に読むもの

1. この `SESSION.md`
2. `HANDOFF.md`
3. `WORKLOG.md`
4. `C:\Users\makki\asset-simulator\CLAUDE.md`
5. `C:\Users\makki\asset-simulator\STATUS.md`
6. `C:\Users\makki\asset-simulator\index.html`

## 起動・確認方法

```powershell
cd C:\Users\makki\asset-simulator
python -m http.server 4173
```

確認URL:

```text
http://localhost:4173/
```

ポート4173が使用中の場合は、別ポートで起動してよい。

## 現在の主な機能

- 積立から計算
- 目標から逆算
- 元本、毎月積立、運用期間、想定利回りの入力
- 利回りの誤差を±%で指定
- 税金考慮ON/OFF
- 手数料考慮ON/OFF
- 運用結果サマリー
- 毎年の積立金額推移の積み上げ棒グラフ
- 利回り誤差のエラーバー表示
- 最終的な積立金の内訳円グラフ
- 年ごとの推移テーブル

## 作業後に更新するもの

- `C:\Users\makki\asset-simulator\STATUS.md`（7-1ゴール部分）
- この `HANDOFF.md`
- この `WORKLOG.md`

## 注意事項

- `STATUS.md` の固定見出しを変更しない（morning_report.py が壊れる可能性がある）
- 新しいゴールはユーザー承認後に追加する
- 既存ファイルの削除、リネーム、移動、大きな上書きはユーザー確認を取る
- 金融シミュレーションなので、免責文を残す
