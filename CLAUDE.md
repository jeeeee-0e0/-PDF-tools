# pdf-tools

ブラウザ上で動作するPDF加工ツール。サーバー不要、すべてクライアントサイドで処理。

## 使い方
- `index.html` をブラウザで直接開く
- CORSエラーが出る場合は `npx serve .` で簡易サーバーを起動

## 機能
- PDF→画像変換（PNG/JPEG、解像度選択可）
- PDF→GIF変換（1ページあたりの秒数指定可）
- ページ並び替え（ドラッグ&ドロップ）
- ページ削除
- 空白ページ追加
- PDFタイトル編集

## 技術構成
- 単一HTMLファイル（CSS・JSインライン）
- pdf-lib (CDN) — PDF操作
- pdfjs-dist (CDN) — PDFレンダリング
- gif.js (CDN) — GIF生成
- JSZip (CDN) — ZIP生成
- FileSaver.js (CDN) — ファイルダウンロード

## 主要ファイル
- `index.html` — 全機能を含む単一ファイル
