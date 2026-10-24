# かんたん日記

シンプルな日記アプリです。日付ごとに気分と一言メモを保存し、ブラウザの `localStorage` に記録を残せます。

日々の気分の変化を簡単に残したいときに使いやすい、小さなWebアプリです。

このリポジトリは、学習ログアプリに育てるための土台として使います。

## 概要

- 今日の日付を自動で入力
- 気分を 5 段階で選択
- 日付ごとにメモを保存
- 過去の記録を一覧表示
- 保存済みメモの編集・削除
- メモの検索と気分フィルター
- 最近の気分の流れをグラフ風に表示

## デモ

GitHub Pages で公開されています。

- https://gigaschool.github.io/tiny-diary/

![アプリ画面](image.png)

## 使い方

1. `index.html` をブラウザで開く
2. 日付・気分・メモを入力する
3. 保存ボタンを押す
4. 一覧から過去の記録を確認・編集・削除できる

ビルド手順やサーバー起動は不要です。HTML/CSS/JavaScript のみで動作します。

## ファイル構成

```text
.
├── index.html
├── styles.css
├── app.js
├── README.md
├── LICENSE
├── image.png
└── .github/
```

## 技術スタック

- HTML
- CSS
- JavaScript
- localStorage

## 保存形式

記録は `tiny-diary.entries.v1` というキーで保存されます。例:

```json
[
  {
    "id": "example-id",
    "date": "2026-04-29",
    "mood": "happy",
    "note": "今日は少しうまくいった",
    "createdAt": "2026-04-29T10:00:00.000Z",
    "updatedAt": "2026-04-29T10:00:00.000Z"
  }
]
```

## ライセンス

MIT License
