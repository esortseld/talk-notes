# Talk Notes

雑談から残す、あとで読むメモ。

このリポジトリは、ChatGPTとの会話の中で出てきた疑問、調べもの、考えたことのうち、後から見返したいものだけを整理して残すための静的サイトです。

## 公開方法

GitHub Pagesで公開する想定です。

Pages設定:

- Source: Deploy from a branch
- Branch: main
- Folder: /root

公開URL:

```text
https://esortseld.github.io/talk-notes/
```

## ファイル構成

```text
talk-notes/
├─ index.html
├─ assets/
│  └─ style.css
├─ data/
│  └─ notes.js
└─ notes/
   └─ sample.html
```

## 新しい記事を追加する手順

1. `notes/` に記事HTMLを追加する
2. `data/notes.js` に記事情報を追加する
3. `index.html` で表示を確認する

## 記事データの形式

```js
const notes = [
  {
    title: "記事タイトル",
    date: "2026-06-12",
    category: "音楽",
    tags: ["歌詞解釈", "80年代"],
    summary: "3行程度の要約。",
    url: "notes/article-file-name.html"
  }
];
```

## 運用方針

ChatGPTとの会話から「これをTalk Notesに追加」と指定したものだけを記事化して追加します。

会話ログを丸ごと保存するのではなく、後から読み返せるように次の形へ整理します。

1. この話題は何か
2. 背景
3. 構造
4. 分類・パターン
5. 判断材料
6. 結論
7. 関連メモ
