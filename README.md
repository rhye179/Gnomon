# Gnomon — Study Notes

物理学・数学の学習ノートをまとめた個人サイトです。

- `index.html` … サイト本体（Home・Articles・記事ページの見た目と仕組み）
- `articles/` … 記事。1本につき `.html` を1つ置き、`articles/list.txt` にファイル名を足すと公開される（ひな形は `articles/_template.html`、書き方は記事「運用ガイド」）
- `fig1.tex` … 図の TikZ ソースの見本（pdflatex → `pdftocairo -svg` で SVG にして記事に埋め込む）
- `pdfs/` … 記事に載せる PDF（記事の `data-pdf="pdfs/xxx.pdf"` で全ページを表示。PDF.js で描画）

## 公開
GitHub Pages（Settings → Pages → Deploy from a branch → `main` / `(root)`）で公開しています。

## プレビュー
記事はページを開いたときに読み込むので、`index.html` をダブルクリックで直接開くと記事が出ません。
VS Code の拡張機能「Live Server」を入れて、右下の「Go Live」で開いてください。

## 数式
数式は KaTeX で組版しています。各数式は HTML の `data-tex` 属性に書き、ページ下部の
「Typeset with KaTeX · n/n」で全件が正しく表示されたかを確認できます。
