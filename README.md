# faq

BiZOOPe FAQサイト

## HUGOの動かし方

以下のコマンドはHUGOをインストールしていなければ使用不可

HUGOのインストールについては、githubのdendron-vaultリポジトリにある
[faq.research.hugo.md](https://github.com/bizoope/dendron-vault/blob/main/notes/faq.research.hugo.md)に記載している。

### サーバ起動

```cmd
hugo server 
```

サーバ起動後は、localhost:1313で確認

ポート番号1313が使えない場合は、以下のオプションでサーバを起動

```cmd
hugo server -p <port>　ポート番号を指定（デフォルトは1313）
``

### 公開用のファイルを生成(build)

```cmd
hugo
```

公開用のファイルを生成するには、hugoコマンドを実行する。実行すると、publicフォルダに公開用のファイル一式(HTML, CSSなど)が生成される。

```cmd
--minify HTMLやXMLを圧縮(minify)する
```

## ページ(md)追加方法

### コマンドプロンプトにて下記コードを実行

```cmd
hugo new フォルダ名/フォルダ名.ファイル名
```

* フォルダ名は、システム、管理者、分析の中から選択する。
以下にフォルダごとの質問内容を記載

  システム：

  管理者：管理者ページに関する質問

  分析：
ファイル名に関しては、下記の[ファイル名の命名規約](#ファイル名の命名規約)に従って作成。

### フロントマターを変更

* title : 質問内容
  
  質問内容は、ルールとして疑問文で終わらせない(〇〇できるか？→〇〇したい)

* tags: [ タグ名,タグ名,タグ名]

  既存のタグ名から従属するものを記述、または新しく作成してもよい(複数タグを指定できるので良しなに)

* categories: [ カテゴリ名 ]

  既存のカテゴリ名から従属するものを記述(新しく作成しても良いがなるべく種類を少なくしたい)

  categoriesを記述していない場合、ホーム画面に表示されないので注意

## ファイル名の命名規約

mdが横並びに存在するので管理をしやすくるため、ファイル名は下記の形で統一する。

カテゴリ名.タグ名.キーワード.md

* カテゴリ名
  
  フロントマターに記述するcategoriesをカテゴリ名にする。

* タグ名

  フロントマターに記述するtagsの中からもっとも関連のあるタグ名にする。

* キーワード

  作成する質問に関連するキーワードを考えてください。

カテゴリ名、タグ名、キーワードは全て日本語も使用することができる。

## ページ(ｍｄ)内容の記載規約

* 本文の文体はです・ます調。
* 画像を使用する場合、画像はstatic/imgフォルダに配置する。
* 画像を使用する場合、記述方法は下記のように記述する。

```cmd
![](/img/画像ファイル.png or .jpg)
```

* 改行が必要な時は空白行を入れて段落分け。

## テーマの著作権について

今回使用しているテーマ「pulp」はMITライセンスのもとで配布されている。

MITライセンスのもとで配布されているものは、改変でも、再配布でも、商用利用でも、有料販売でも、どんなことにでも自由に無料でつかうことができる。

そのために守らなくてはいけない条件は、「著作権表示」と「MITライセンスの全文」を記載する、という条件だけ。

「著作権表示」と「ライセンスの全文」の掲載については、ソースコードのなかや、同梱の別ファイルなどに記述で問題なし。

なので、今回は「license.txt」に記載した。

参考サイト: [MITライセンスってなに？どうやって使うの？商用でも無料で使えるの？](https://wisdommingle.com/mit-license/)
