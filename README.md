# Gnomon — Study Notes

物理学・数学の学習ノートをまとめた個人サイトです。

- `index.html` … サイト本体（Home・Articles・各記事 A〜Z をすべてこの1ファイルで切り替え。書き方は記事 A「運用ガイド」）
- `fig1.tex` … 図の TikZ ソースの見本（pdflatex → `pdftocairo -svg` で SVG にして記事に埋め込む）
- `pdfs/` … 記事に載せる PDF（記事の `data-pdf="pdfs/xxx.pdf"` で全ページを表示。PDF.js で描画）

## 公開
GitHub Pages（Settings → Pages → Deploy from a branch → `main` / `(root)`）で公開しています。

## 数式
数式は KaTeX で組版しています。各数式は HTML の `data-tex` 属性に書き、ページ下部の
「Typeset with KaTeX · n/n」で全件が正しく表示されたかを確認できます。
