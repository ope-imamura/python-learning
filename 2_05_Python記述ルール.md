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

# Python記述ルール
## プログラミング基礎知識

<div class="center title-slide">
<p>株式会社オープンアップエンジニア</p>
</div>

---

## Index

1. Pythonインストール

2. VSCodeインストール

3. 動作環境の確認

**4. Pythonの記述ルール**

---


## 「Hello World!」の実行
### 最初のPythonプログラム

<span class="importance-high">プログラミング学習の第一歩として、「Hello World!」と表示するプログラムから始めましょう。</span>


```python
print("Hello World!")
```


このシンプルな1行のコードを実行すると、画面に「Hello World!」と表示されます。

この例を通して、Pythonの基本的な記述ルールを見ていきましょう。

---

## print関数の説明
### 画面に出力する方法

<span class="importance-medium">`print()`</span>はPythonの組み込み関数の一つで、括弧内の内容を画面に出力するために使用します。

<div class="columns">
<div>

```python
# 文字列を出力（必ずクォーテーションで囲む）
print("こんにちは")
print('シングルクォートも使用可能')

# 数値を出力（クォーテーション不要）
print(123)

# 計算結果を出力（式の評価が可能）
print(3 + 4)  # 結果: 7
print(10 * 5)  # 結果: 50
print(20 / 4)  # 結果: 5.0
```

</div>
<div>

```python
# 複数の値を出力
print("数字は", 5)

# 変数の内容を出力
name = "太郎"
print("私の名前は", name, "です")

# 文字列連結と計算の組み合わせ
price = 1200
tax = 0.1
print("税込価格: " + str(price * (1 + tax)) + "円")
```

</div>
</div>

---

## 順次実行
### プログラムの基本的な流れ

<span class="importance-high">Pythonプログラムは基本的に「順次実行」されます。</span>

つまり、コードは上から下へ、左から右へと順番に実行されていきます。

```python
print("1行目を実行")
print("2行目を実行")
print("3行目を実行")
```

このコードを実行すると、以下の順番でメッセージが表示されます：
1. 「1行目を実行」
2. 「2行目を実行」
3. 「3行目を実行」

これはプログラミングの最も基本的な制御の流れです。

---

## 大小文字の区別
### 正確な記述が必要

<span class="importance-high">Pythonでは大文字と小文字は区別されます。</span>

つまり、`print`と`Print`と`PRINT`は全く別のものとして扱われます。

<div class="columns">
<div>

```python
# 正しい記述
print("正しく実行されます")

# 間違った記述
Print("エラーになります")
PRINT("これもエラーになります")
```

</div>
<div>

<div class="highlight">
エラーメッセージ例：
```
NameError: name 'Print' is not defined
```

このエラーは「Print」という名前が定義されていないことを示しています。
</div>

</div>
</div>

変数名、関数名、予約語などすべてにおいて大文字と小文字の区別があるため、常に正確に記述する必要があります。

---

## 命令文の終わり
### セミコロン不要の言語

<span class="importance-medium">Pythonでは命令文の終わりにセミコロン(`;`)などの特別な記号が不要です。</span>

行の終わりがそのまま命令文の終わりとなります。

<div class="columns">
<div>

```python
# 通常の記述（推奨）
print("1行目")
print("2行目")
```

</div>
<div>

```python
# 1行に複数の命令も可能だが推奨されない
print("1つ目"); print("2つ目"); print("3つ目")
```

</div>
</div>

<div class="highlight">
<span class="importance-high">Point:</span> 可読性を高めるため、基本的には1行に1つの命令を書くことを推奨します。
</div>

---

## コメント
### コードの説明や注釈

<span class="importance-high">コメントはプログラムの動作に影響を与えない説明文です。</span>

Pythonでは、`#`記号から行の終わりまでがコメントとして扱われます。

<div class="columns">
<div>

```python
# これはコメントです
print("Hello")  # 行末のコメント

# コメントは実行されません
# print("This won't be executed")
```

</div>
<div>

**複数行コメント**：
```python
"""
これは
複数行の
コメントです
"""
print("Hello")
```

</div>
</div>

<div class="highlight">
<span class="importance-medium">コメントの主な用途：</span>
- コードの説明
- 一時的にコードを無効化する
- 著者名や更新履歴の記録
</div>

---

## インデントの重要性
### Pythonの特徴的な構文ルール

<span class="importance-high">Pythonではインデント（字下げ）によってコードブロックを定義します。</span>

多くの言語では中括弧`{}`を使いますが、Pythonではスペースやタブでインデントを付けることが必須です。

```python
if True:
    print("この行はインデントされています")
    print("このブロックに属する別の行")
print("インデントがないのでif文のブロックの外です")
```

<div class="highlight">
<span class="importance-medium">インデントのルール：</span>
- 通常4つのスペースを使用（推奨）
- 同じブロックでは同じレベルのインデントを使用
- インデントが正しくないとエラーになる
</div>