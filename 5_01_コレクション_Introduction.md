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

# Introduction
## コレクション

<div class="center title-slide">
<p>株式会社オープンアップエンジニア</p>
</div>

---

## 目次

1. リスト
2. リストの更新
3. 辞書
4. 辞書の更新
5. 集合とタプル

---
## 目次

<div class="highlight">
Lessonのゴール

①複数のデータをまとめて扱うコレクション型を理解する
②コレクション型の種類と使い分けを習得する
③データの追加・削除・更新の方法を習得する
④コレクション型を活用したプログラミングができるようになる
</div>