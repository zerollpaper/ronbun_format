# 卒論フォーマット

LaTeXで卒論を作成するためのファイル集です。

## ファイル構成

- **[main.tex](main.tex)** - メインファイル
- **[0_cover.tex](0_cover.tex)** - 表紙ファイル
- **[1_intro.tex](1_intro.tex)** - 序論ファイル
- **[9_ack.tex](99_ack.tex)** - 謝辞ファイル

## 使用方法

### preamble

[latex_settings](https://github.com/zerollpaper/latex_settings)というリポジトリにある`jpreamble.tex`をダウンロードし、[main.tex](main.tex)の`/path/to/jpreamble`で`jpreamble.tex`のパスを指定してください。

### bibファイル

文献管理に使用しているbibファイルのパスを`/path/to/bibfile`で指定してください。

### 本文

`\input{1_intro}`の後ろに`input{2_***}`, `input{3_***}`のように記述してください。
`2_***.tex`, `3_***.tex`というファイルを作成し、その中に本文を記述してください。

## 依存関係

- LuaTeX
- 各種LaTeXパッケージ（詳細は[jpreamble.tex](jpreamble.tex)を参照）

## ライセンス

このプロジェクトはMITライセンスのもとで公開されています。
個人利用・改変・再配布などは自由に行って構いません。