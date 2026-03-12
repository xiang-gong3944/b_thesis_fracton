# 双極子保存則で拘束された励起を持つ量子誤り訂正符号の物理

**Fractonic Excitations in Dipole-Conserving Hypergraph-Product Codes**

2025年度 東京理科大学 理学部第一部応用物理学科 卒業論文
著者: 西原 翔

## PDF

コンパイル済みの論文PDFは以下から閲覧できます。

[out/master.pdf](out/master.pdf)

## ディレクトリ構造

```
.
├── .gitignore         # gitで追跡しないファイルの登録
├── .latexmkrc         # ビルド設定 (uplatex + upbibtex, 出力先: out/)
├── readme.md          # この文章
├── LICENSE.md         # MIT LICENSE
├── master.tex         # メインファイル (subfileの親)
├── template.sty       # 共通設定・パッケージ読み込み用
├── references.bib     # 参考文献
│
├── chapter/           # 各章のTeXファイル
│   ├── 00_preface.tex
│   ├── 01_shor.tex
│   ├── 02_generalized_pauli.tex
│   ├── 03_stabilizer_CSS.tex
│   │
│   └── figures/       # 図のファイル
│       ├── chap1_*.png
│       └── chap2_*.png
│
└── out/
    └── master.pdf     # コンパイル済みPDF
```

## LaTeX文書の構造

`master.tex` を親ファイルとし、`\subfile{}` で各章を読み込む構成となっています。

```
master.tex
├── 序文                          (chapter/00_preface.tex)
├── 目次
│
└── Part 1: 量子誤り訂正符号
    ├── Chapter 1: Shor符号       (chapter/01_shor.tex)
    ├── Chapter 2: 一般化パウリ演算子とqudit
    │                             (chapter/02_generalized_pauli.tex)
    └── Chapter 3: スタビライザー形式
                                  (chapter/03_stabilizer_CSS.tex)
```

## コンパイル環境

`.latexmkrc` に以下の設定が記述されています。

- コンパイラ: uplatex
- 文献処理: upbibtex
- 出力先: `out/` フォルダ (`out/master.pdf` が生成されます)

VS Code の拡張機能 [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) を使う場合、`.latexmkrc` が自動的に読み込まれ、保存時に自動コンパイルが実行されます。
