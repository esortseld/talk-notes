# Talk Notes

Talk Notesは、日々の会話、調べもの、制作ログ、楽曲メモを、あとで使える形に整理して残す個人用ノートです。

雑談や疑問を短いメモとして残しつつ、まずは「Songs / 楽曲メモ」を中心に、曲ごとの基本情報、歌唱メモ、解釈メモ、練習状況、外部歌詞リンクを整理します。

## Songs / 楽曲メモ

`songs.html` では、曲名、アーティスト、タグで検索できます。

バンドまたは用途、進捗でも絞り込みできます。

楽曲メモでは歌詞本文をサイト内に直接掲載しません。歌詞確認は、JOYSOUNDなどの正規外部歌詞ページへのリンクで扱います。

## 新しい楽曲メモを追加する手順

1. `notes/songs/` にHTMLを追加する
2. `data/songs.js` に曲データを追加する
3. `lyricsUrl` にJOYSOUND等の正規ページURLを入れる。未確認なら空欄にする
4. `songs.html` で表示確認する

`data/songs.js` の形式:

```js
const songs = [
  {
    title: "プラスティック・ラブ",
    artist: "竹内まりや",
    lyricist: "",
    composer: "",
    year: "1984",
    originalKey: "",
    myKey: "",
    bands: ["sweet pastime"],
    status: "解釈メモ",
    progress: "",
    tags: ["80年代", "シティポップ", "歌詞解釈", "都市生活"],
    summary: "都市的な恋愛観と消費イメージを含む楽曲。主人公像の解釈メモ。",
    lyricsUrl: "",
    memoUrl: "notes/songs/sample-song.html"
  }
];
```

## 新しい雑多メモを追加する手順

1. `notes/` にHTMLを追加する
2. `data/notes.js` に記事情報を追加する
3. `index.html` で表示確認する

## GitHub Pages設定

GitHub Pagesでは、次の設定で公開します。

- Source: Deploy from a branch
- Branch: main
- Folder: /root
