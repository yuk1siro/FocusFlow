# FocusFlow — 集中タイマー 🌊

ポモドーロ形式の集中タイマーです。**終了時の音を、YouTube やニコニコ動画のリンクから好きに設定**できます。
ビルド不要・外部ライブラリ不要の単一 HTML ファイル（`index.html`）で動きます。

## 特長

- 集中 / 小休憩 / 長休憩の 3 モード（時間・長休憩までの回数を変更可能）
- 残り時間に合わせて水位が下がる円形ダイヤル
- **終了時に YouTube / ニコニコ動画を自動再生**（リンク未設定なら内蔵チャイム）
- 再生開始位置（秒）の指定、設定画面からのテスト再生
- 終了後に次のタイマーを自動開始するオプション
- 今日の集中回数を記録
- ダーク / ライトテーマ対応、スマホ対応
- 設定はブラウザの `localStorage` に保存（サーバー送信なし）
- タブがバックグラウンドでも終了時刻ベースで計測するため、時間がずれにくい

## 使い方

1. `index.html` をブラウザで開く（YouTubeを使う場合は GitHub Pages か `http://localhost` で開いてください。下記の注意事項参照）
2. 「終了時に流す動画」にリンクを貼り付けて **保存**
3. **テスト再生** で確認
4. **スタート** を押して集中開始

スペースキーで開始 / 一時停止、`Esc` でアラームを閉じられます。

### 対応リンク

| サービス | 例 |
|---|---|
| YouTube | `https://www.youtube.com/watch?v=xxxxxxxxxxx` / `https://youtu.be/xxxxxxxxxxx` / `https://www.youtube.com/shorts/xxxxxxxxxxx` / プレイリスト（`list=`） |
| ニコニコ動画 | `https://www.nicovideo.jp/watch/smXXXXXXXX` / `https://nico.ms/smXXXXXXXX` |

URL の `t=90`（YouTube）や `from=90`（ニコニコ）も開始位置として読み取ります。

## サイト
https://yuk1siro.github.io/FocusFlow/
