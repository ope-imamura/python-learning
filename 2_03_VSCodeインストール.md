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

# VSCodeインストール
## 環境構築

<div class="center title-slide">
<p>株式会社オープンアップエンジニア</p>
</div>

---

## Index

1. Pythonインストール

**2. VSCodeインストール**

3. 動作環境の確認

4. Pythonの記述ルール

---

## VSCodeインストール
### VSCode公式サイトにアクセス

<span class="importance-medium">Visual Studio Code（VSCode）をインストールするために、公式サイトにアクセスします。</span>

ブラウザで以下のURLにアクセスしてください：
<span class="importance-high">https://code.visualstudio.com/</span>

---

## VSCodeインストール
### インストーラーのダウンロード

公式サイトのトップページに表示される<span class="importance-high">「Download for Windows」</span>ボタンをクリックします。

<span class="importance-medium">Stable版（安定版）</span>をダウンロードすることをお勧めします。

---

## VSCodeインストール
### インストーラーの実行

1. ダウンロードした「VSCodeSetup-x64-x.xx.x.exe」ファイルをダブルクリック
   （x.xx.xはバージョン番号）

2. セキュリティ警告が表示される場合は「はい」をクリックして続行

---

## VSCodeインストール
### 使用許諾契約の同意

インストーラーが起動したら、使用許諾契約書（ライセンス条項）を確認し、<span class="importance-medium">「同意する」</span>を選択して<span class="importance-medium">「次へ」</span>をクリックします。

---

## VSCodeインストール
### インストール先の選択

インストール先のフォルダを選択します。
デフォルトの設定のまま「次へ」をクリックすることをお勧めします。

デフォルトのインストール先：
`C:\Users\ユーザー名\AppData\Local\Programs\Microsoft VS Code\`

---

## VSCodeインストール
### スタートメニューフォルダの選択

スタートメニューに表示されるフォルダ名を選択します。

デフォルトの「Visual Studio Code」のまま「次へ」をクリックします。

---

## VSCodeインストール
### 追加タスクの選択

インストール時の追加タスクを選択します。以下のオプションを<span class="importance-high">すべて選択</span>することをお勧めします：

<div class="columns">
<div>

- デスクトップ上にアイコンを作成する
- エクスプローラーのファイルコンテキストメニューに「Code で開く」アクションを追加する
- エクスプローラーのディレクトリコンテキストメニューに「Code で開く」アクションを追加する

</div>
<div>

- <span class="importance-high">PATH に追加する</span>（再起動後に使用可能）
- <span class="importance-high">.py ファイルをVS Codeに関連付ける</span>

</div>
</div>

<div class="highlight">
これらのオプションを選択することで、VSCodeをより便利に使用できます。
</div>

---

## VSCodeインストール
### インストールの開始

「インストール」ボタンをクリックしてインストールを開始します。

インストールには数分かかる場合があります。

---

## VSCodeインストール
### インストールの完了

インストールが完了したら、<span class="importance-medium">「Visual Studio Code を実行する」</span>にチェックを入れたまま「完了」をクリックします。

これでVSCodeが起動します。

---

## VSCodeの日本語化
### 日本語拡張機能のインストール

<span class="importance-high">VSCodeを日本語化するために、日本語言語パックをインストールします。</span>

<div class="columns">
<div>

1. VSCodeが起動したら、左側のアクティビティバーから「Extensions（拡張機能）」アイコン（パズルのピースの形）をクリックします

2. 上部の検索バーに<span class="importance-medium">「Japanese」</span>と入力します

</div>
<div>

3. 検索結果から<span class="importance-medium">「Japanese Language Pack for Visual Studio Code」</span>を見つけます

4. 「Install（インストール）」ボタンをクリックします

</div>
</div>

---

## VSCodeの日本語化
### 言語設定の変更

<span class="importance-high">日本語言語パックをインストールした後、言語設定を変更します。</span>

<div class="columns">
<div>

1. キーボードで<span class="importance-medium">「Ctrl + Shift + P」</span>を押してコマンドパレットを開きます

2. <span class="importance-medium">「Configure Display Language」</span>と入力し、表示される項目をクリックします

3. ドロップダウンリストから<span class="importance-medium">「ja（日本語）」</span>を選択します

</div>
<div>

4. VSCodeの再起動を求められるので、「Restart（再起動）」をクリックします

5. VSCodeが再起動し、インターフェイスが日本語になります

</div>
</div>

---

## Python拡張機能のインストール
### Python拡張機能の検索

<span class="importance-high">Pythonプログラミングを快適に行うために、Python拡張機能をインストールします。</span>

<div class="columns">
<div>

1. 左側のアクティビティバーから「拡張機能」アイコンをクリックします

2. 検索バーに<span class="importance-medium">「Python」</span>と入力します

</div>
<div>

3. 検索結果から<span class="importance-medium">「Python」</span>（Microsoft公式）を見つけます
   通常、検索結果の一番上に表示されます

4. 「インストール」ボタンをクリックします

</div>
</div>
