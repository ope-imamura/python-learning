---
marp: true
theme: default
paginate: false
footer: © オープンアップエンジニア2024
style: |
  section {
    font-family: 'Meiryo UI', 'Noto Sans JP', sans-serif;
    font-size: 24px;
    padding: 40px;
  }
  header {
    position: absolute;
    left: 30px;
    top: 20px;
    font-size: 18px;
    color: #666;
  }
  footer {
    position: absolute;
    left: auto !important;
    right: 30px !important;
    bottom: 20px;
    font-size: 18px;
    color: #666;
    margin-bottom: 10px; /* フッターの高さに内容が被らないように（字幕用マージン） */
    text-align: right !important;
  }
  h1 {
    font-size: 54px;
    color: #FF8C00;
    margin-top: 100px;
    text-align: center;
    border-bottom: 4px solid #FF8C00;
    padding-bottom: 20px;
  }
  h2 {
    font-size: 38px;
    background: linear-gradient(90deg, #FF8C00, rgba(255, 140, 0, 0.7));
    color: white;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    padding: 15px 40px;
    margin: 0;
    z-index: 10;
  }
  h3 {
    color: #FF8C00;
    font-size: 34px;
    border-left: 8px solid #FF8C00;
    padding-left: 16px;
  }
  a {
    color: #0078D7;
    text-decoration: none;
  }
  strong {
    color: #FF8C00;
    font-weight: bold;
  }
  em {
    font-style: normal;
    font-weight: bold;
    color: #666;
  }
  ul, ol {
    margin-left: 30px;
  }
  li {
    margin-bottom: 10px;
  }
  table {
    border-collapse: collapse;
    margin: 20px 0;
    width: 100%;
  }
  th {
    background-color: #FF8C00;
    color: white;
    padding: 12px;
    border: 1px solid #ccc;
  }
  td {
    padding: 12px;
    border: 1px solid #ccc;
  }
  tr:nth-child(even) {
    background-color: #f8f8f8;
  }
  code {
    background-color: #f0f0f0;
    padding: 2px 5px;
    border-radius: 3px;
    font-family: 'Courier New', monospace;
  }
  .columns {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
  }
  .highlight {
    background-color: rgba(255, 140, 0, 0.2);
    padding: 15px;
    border-radius: 5px;
  }
  .center {
    text-align: center;
  }
  .right {
    text-align: right;
  }
  img {
    max-width: 100%;
    height: auto;
    border-radius: 5px;
  }
  .small-image {
    max-width: 60%;
  }
  .background-cover {
    background-size: cover;
    background-position: center;
    color: white;
  }
  .title-slide {
    background-color: #f5f5f5;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  
  /* 重要度に基づく色設定 */
  .importance-high {
    color: #FF8C00; /* オレンジ */
    font-weight: bold;
    font-size: larger;
  }
  .importance-medium {
    color: #4D8EA0; /* アクア */
    font-weight: bold;
    font-size: larger;
  }
  .importance-low {
    background-color: #E0E0E0; /* 塗りつぶし（大字なし） */
    font-size: larger;
  }
---

# Pythonインストール
## 環境構築

<div class="center title-slide">
<p>株式会社オープンアップエンジニア</p>
</div>

---

## Index


**1. Pythonインストール**

2. VSCodeインストール


3. 動作環境の確認

4. Pythonの記述ルール




---

## Pythonインストール
### Python公式サイトにアクセス

<span class="importance-medium">Pythonをインストールするために、まずはPython公式サイトにアクセスします。</span>

ブラウザで以下のURLにアクセスしてください：
<span class="importance-high">https://www.python.org/</span>



---

## Pythonインストール
### Downloadsを選択

公式サイトのメニューから<span class="importance-high">「Downloads」</span>を選択します。

<div class="columns">
<div>

1. メニューバーの「Downloads」をクリック
2. 表示されるドロップダウンメニューから「Windows」を選択

</div>

</div>

---

## Pythonインストール
### Windowsインストーラーのダウンロード

Windowsのダウンロードページで、<span class="importance-high">最新バージョンのPythonインストーラー</span>を選択します。

<div class="columns">
<div>

- 通常、ページ上部に「Python 3.x.x」（xはバージョン番号）と書かれたボタンがあります
- <span class="importance-medium">「Windows installer (64-bit)」</span>と書かれたリンクをクリックしてダウンロード

</div>

</div>

---

## Pythonインストール
### ダウンロードしたインストーラーの実行



1. ダウンロードしたインストーラー（python-3.x.x-amd64.exe）をダブルクリックして実行

2. Windows 10/11ではセキュリティ警告が表示される場合があります
   → 「はい」をクリックして続行


---

## Pythonインストール
### インストールオプションの設定

インストーラーが起動したら、以下の設定を確認します：

<div class="highlight">
<span class="importance-high">重要: 「Add Python 3.x to PATH」のチェックボックスにチェックを入れる</span>
</div>

これにより、コマンドプロンプトから直接Pythonを実行できるようになります。



---

## Pythonインストール
### インストールの開始



- オプションを設定したら、<span class="importance-medium">「Install Now」</span>ボタンをクリックしてインストールを開始

- 標準インストールの場合、Pythonは以下の場所にインストールされます：
  `C:\Users\ユーザー名\AppData\Local\Programs\Python\Python3x\`

- カスタマイズが必要な場合は「Customize installation」を選択



---

## Pythonインストール
### インストールの進行

インストールが進行中です。しばらくお待ちください。

- 進行状況がプログレスバーで表示されます
- インストール時間は、お使いのコンピュータの性能により異なります（通常1〜5分程度）



---

## Pythonインストール
### インストール完了


- インストールが完了すると、<span class="importance-medium">「Setup was successful」</span>というメッセージが表示

- 「Close」ボタンをクリックしてインストーラーを閉じます



---

## Pythonインストール
### インストールの確認

<span class="importance-high">インストールが正常に完了したかを確認しましょう。</span>



1. Windowsの検索バーに「cmd」と入力し、「コマンドプロンプト」を選択

2. コマンドプロンプトが開いたら、以下のコマンドを入力して実行：

```
python --version
```

インストールされたPythonのバージョンが表示されれば、インストールは成功です。



---

## Pythonインストール
### PIPの確認

<span class="importance-medium">Pythonと一緒にインストールされるパッケージ管理ツール「pip」も確認しましょう。</span>

<div class="columns">
<div>

コマンドプロンプトで以下のコマンドを実行：

```
pip --version
```

pipのバージョンが表示されれば、pipも正常にインストールされています。

</div>
<div>

<div class="highlight">
<span class="importance-high">pip (Package Installer for Python)</span>

Pythonのパッケージ（ライブラリ）をインストール・管理するためのツール。
これを使用して外部ライブラリを簡単に追加できます。
</div>

</div>
</div>