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
