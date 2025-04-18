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
  .tips {
    background-color: #FFF3E0;
    border-left: 5px solid #FF8C00;
    padding: 15px;
    margin: 20px 0;
  }
---

<!-- 
タイトルスライド
-->

# Pythonの特徴
## 初心者に優しい汎用プログラミング言語

<div class="center title-slide">
<p>株式会社オープンアップエンジニア</p>
</div>

---
## Index

1. プログラミングとは

**2. Pythonの特徴**

3. 制御構文とは


---

## Pythonとは

### Pythonの概要

<span class="importance-high">Python（パイソン）は、シンプルで習得しやすい汎用プログラミング言語</span>です。

- 1991年にグイド・ヴァン・ロッサムによって開発
- 名前の由来は英国のコメディグループ「モンティ・パイソン」
- <span class="importance-high">読みやすさと簡潔さを重視した設計思想</span>
- 現在は世界中で最も人気のあるプログラミング言語の一つ


---

## Pythonの歴史

### 誕生と発展

- <span class="importance-medium">1991年</span>：グイド・ヴァン・ロッサムがPython 0.9.0をリリース
- <span class="importance-medium">2000年</span>：Python 2.0がリリース（リスト内包表記など多くの機能追加）
- <span class="importance-medium">2008年</span>：Python 3.0がリリース（互換性のない大規模な言語更新）
- <span class="importance-high">2020年</span>：Python 2系のサポート終了。現在はPython 3系が標準

<div class="tips">
Python 2と3は互換性がないため、古いPython 2のコードをPython 3で動かすには修正が必要です。現在は新規開発ではPython 3を使うのが標準です。
</div>

---

## Pythonの基本的な特徴

### シンプルな構文

<span class="importance-high">Pythonはコードの読みやすさを重視しています</span>

他の言語（例：C++）とPythonの比較：

<div class="columns">
<div>

**C++の例**:
```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, World!" << endl;
    return 0;
}
```

</div>
<div>

**Pythonの例**:
```python
print("Hello, World!")
```

</div>
</div>

---

## Pythonの基本的な特徴

### インデントによるブロック構造

<span class="importance-high">Pythonは「インデント」（字下げ）でコードブロックを表現します</span>

他の言語（例：Java）とPythonの比較：

<div class="columns">
<div>

**Javaの例**:
```java
if (x > 0) {
    System.out.println("Positive");
} else {
    System.out.println("Non-positive");
}
```

</div>
<div>

**Pythonの例**:
```python
if x > 0:
    print("Positive")
else:
    print("Non-positive")
```

</div>
</div>

<div class="tips">
他の多くの言語では波括弧 { } でコードブロックを表しますが、Pythonではインデント（空白やタブ）でコードの階層構造を表現します。これにより強制的に読みやすいコードになります。
</div>


---

## Pythonの基本的な特徴

### 豊富な標準ライブラリ

<span class="importance-high">Pythonは「バッテリー同梱（Battery Included）」の思想</span>

標準ライブラリだけでも多くのことができます：

- ファイル操作
- 日付・時刻処理
- 数学計算
- データ圧縮
- データベース接続
- GUIアプリケーション開発

<div class="tips">
「バッテリー同梱」とは、最初からたくさんの機能が含まれているという意味です。追加でインストールしなくても基本的な機能が使えます。
</div>

---

## Pythonの基本的な特徴

### インタプリタ型言語

<span class="importance-medium">Pythonはインタプリタ型言語です</span>

- プログラムを一行ずつ解釈して実行
- コンパイル不要でそのまま実行可能
- 対話的な実行環境（REPLと呼ばれる）が利用可能

```python
# 対話モードの例
>>> 2 + 3
5
>>> "Hello" + " World"
'Hello World'
>>> len("Python")
6
```

<div class="tips">
対話モードを利用すると、簡単なコードを試したり、動作を確認したりするのに便利です。実際の開発では.pyファイルにコードを書くことが多いです。
</div>

---

## Pythonの弱点


- <span class="importance-medium">実行速度が比較的遅い</span>
  - インタプリタ型言語のため、C/C++などに比べて処理速度が遅い
  - 計算量の多い処理には向かないことも

- <span class="importance-medium">モバイルアプリ開発には不向き</span>
  - iOS/Androidのネイティブアプリ開発には一般的に使われない

- <span class="importance-low">大規模システムの型安全性</span>
  - 動的型付けのため、大規模開発では型関連のバグが発生しやすい面も
  - Type Hintsという機能で一部緩和されている

<div class="tips">
どんな言語にも得意・不得意があります。Pythonは多くの用途に適していますが、全ての状況で最適というわけではありません。
</div>

---

## Pythonの人気の理由

### プログラミング言語の人気ランキング

<span class="importance-high">Pythonは世界的に最も人気のある言語の一つです</span>

主要なプログラミング言語ランキングでは常に上位に位置しています：

- TIOBE Index
- PYPL Index
- GitHub人気言語
- Stack Overflow調査

<div class="tips">
Pythonは特に初心者向け言語としても、データサイエンス・AI分野の言語としても高い人気を誇ります。
</div>

---

## Pythonの人気の理由

### なぜPythonが選ばれるのか

<span class="importance-high">Pythonが人気を集める主な理由</span>：

1. <span class="importance-high">学習の容易さ</span>
2. <span class="importance-high">生産性の高さ</span>
3. <span class="importance-high">データサイエンス・AI分野での優位性</span>
4. <span class="importance-medium">求人市場での需要の高さ</span>
5. <span class="importance-medium">コミュニティとエコシステムの充実</span>

<div class="tips">
特にデータ分析やAI分野ではPythonが事実上の標準言語となっており、この分野を目指す場合はPythonスキルが重要です。
</div>


