---
title: "Duckでファイルをダウンロードすると、商品名が文字化けする"
categories: [ POS分析 ]
tags: [POS,duck,トラブル]
---

### デフォルトでは文字コードセットが「UTF-8」となっております

* 文字コードセットが、デフォルトの「UTF-8」でダウンロードしたファイルをExcelで開きますと、文字化けが起きます。
* Excelで開く場合は、Duckの分析条件設定画面の下部にあります文字コードを「Shift-JIS」をご指定下さい。

  マニュアル参考ページ：[Duckの操作方法](https://bizoope.github.io/bizoope-manual/duck.html)
