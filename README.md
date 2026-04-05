# 東京大学百年史 通史一 — GitHub Pages 公開手順

## フォルダ構成

```
(リポジトリ直下)
├── index.html       ← 目次ページ
├── viewer.html      ← PDFビューワー
├── README.md        ← この説明
└── pdfs/
    ├── hen1_ch1.pdf  ← 第一編 第一章
    ├── hen1_ch2.pdf  ← 第一編 第二章
    ├── hen1_ch3.pdf  ← 第一編 第三章
    ├── hen2_ch1.pdf  ← 第二編 第一章
    ├── hen2_ch2.pdf  ← 第二編 第二章
    ├── hen3_ch1.pdf  ← 第三編 第一章
    ├── hen3_ch2.pdf  ← 第三編 第二章
    └── hen3_ch3.pdf  ← 第三編 第三章
```

## 手順

### 1. PDFの分割

ilovepdf（無料）などで359MBのPDFを章ごとに分割します。
各ファイルが100MB以下になるよう分割してください（GitHub上限）。

- https://www.ilovepdf.com/ja/split_pdf

分割したファイルを上記のファイル名に変更してください。

### 2. GitHubリポジトリの作成

1. https://github.com/new にアクセス
2. リポジトリ名を入力（例：`hyakunenshi`）
3. 「Public」を選択
4. 「Create repository」をクリック

### 3. ファイルのアップロード

**方法A：ブラウザ上で操作（簡単）**

1. 作成したリポジトリのページで「Add file」→「Upload files」
2. `index.html`、`viewer.html` をドラッグ＆ドロップ
3. 「Commit changes」をクリック
4. `pdfs/` フォルダを作るため：「Add file」→「Create new file」
   - ファイル名に `pdfs/.gitkeep` と入力して保存
5. 再度「Add file」→「Upload files」でPDFファイルを
   `pdfs/` フォルダにアップロード

**方法B：GitHub Desktop（推奨）**

GitHub Desktop を使うとフォルダごとまとめて操作できます。

### 4. GitHub Pages の有効化

1. リポジトリの「Settings」タブ
2. 左メニュー「Pages」
3. Branch: `main`、フォルダ: `/ (root)` を選択
4. 「Save」をクリック
5. 数分後、以下のURLで公開されます：
   `https://okisayaka.github.io/（リポジトリ名）/`

### 5. 学生への配布

目次URLを共有するだけです：
```
https://okisayaka.github.io/（リポジトリ名）/
```

## 注意事項

- GitHubの1ファイル上限は **100MB** です
- 各章のPDFが100MBを超える場合はさらに細かく分割してください
- PDFはブラウザ内で表示されるため、学生側のストレージ消費はありません
- スマートフォンからも閲覧可能です
