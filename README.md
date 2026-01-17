# 論理学 講義レポート

2025年度 第2セメスター 開講科目「論理学」の最終レポート用リポジトリです。

## 概要
本レポートは、講義で扱われた主要な論理体系のまとめと、それに対する考察・感想をまとめたものです。

### レポートの構成
1. **講義内容の要約**
    - 古典命題論理
    - 様相論理
    - 述語論理
2. **考察・感想**
    - 講義を通じて得た知見

---

## 閲覧方法
最新のレポート（PDFファイル）は以下のディレクトリから確認できます。
- [report_main.pdf](./report_main.pdf) (※コンパイル済みPDFを管理に含める場合)

---

## 開発・ビルド環境

本プロジェクトは WSL (Windows Subsystem for Linux) 上の TeX Live 環境で作成しています。

### 動作環境
- **OS:** WSL2 (Ubuntu 22.04 LTS 等)
- **TeX 構成:** TeX Live (パッケージ: `texlive-full`)
- **コンパイラ:** LuaLaTeX / latexmk
- **エディタ:** Visual Studio Code (+ LaTeX Workshop 拡張)

### コンパイル方法
WSL ターミナル上で以下のコマンドを実行してください。
```bash
# latexmk を使用して PDF を生成
latexmk report_main.tex

# 生成物（中間ファイル）の掃除
latexmk -c