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

以下のオプションなどもある
```cmd
-D ドラフト状態のファイルも出力する
-F 未来の日付のファイルも出力する
-h ヘルプを表示する
-p <port>　ポート番号を指定（デフォルトは1313）
```

### 公開用のファイルを生成(build)

```cmd
hugo
```

公開用のファイルを生成するには、hugoコマンドを実行する。実行すると、publicフォルダに公開用のファイル一式(HTML, CSSなど)が生成される。

```cmd
-D ドラフト状態のファイルも出力する
-F 未来の日付のファイルも出力する
-h ヘルプを表示する
--minify HTMLやXMLを圧縮(minify)する
```

## テーマの著作権について

今回使用しているテーマ「pulp」はMITライセンスのもとで配布されている。

MITライセンスのもとで配布されているものは、改変でも、再配布でも、商用利用でも、有料販売でも、どんなことにでも自由に無料でつかうことができる。

そのために守らなくてはいけない条件は、「著作権表示」と「MITライセンスの全文」を記載する、という条件だけ。

「著作権表示」と「ライセンスの全文」の掲載については、ソースコードのなかや、同梱の別ファイルなどに記述で問題なし。

なので、今回は「license.txt」に記載した。

参考サイト: https://wisdommingle.com/mit-license/