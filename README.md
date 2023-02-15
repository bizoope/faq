# faq
BiZOOPe FAQサイト

## HUGOインストール手順

1. githubからzipをダウンロード

   githubのHugoで[https://github.com/spf13/hugo/releases]より、自分はwindowsでしたのでhugo_extended_0.110.0_windows-amd64.zipを選んだ。

2. フォルダを作る

   binフォルダを以下のように作ってください。CドライブやDドライブなどはパソコンのパーティション設定などを見ながら決めてください。

   //Hugoのところは好きなフォルダ名で問題なし。

   C:\Hugo\bin

3. zipを展開

   1.でダウンロードしたzipを展開し、hugo.exeを2.で作ったbinフォルダ内に配置してください。

4. 環境変数パスを通す

   画面左下のウィンドウズマークを右クリック⇒システム⇒システムの詳細設定⇒環境変数に進みます。

   windowsパソコンへログインしている現状のユーザーにパスを通す場合、上部の「ユーザーの環境変数」でPathをダブルクリック⇒新規まで進み、2.で作ったフォルダのパスC:\Hugo\binを入力⇒OKで各ウィンドウを閉じる。

   ※2.でDドライブなどにした場合は、D:\Hugo\binなど、適宜最適化してください。

5. helpコマンド動作確認

   cortanaなどでコマンドプロンプトを立ち上げます。

   以下のへルプコマンドを入力し、パスが通ったか確認します。

   ヘルプコマンド一覧が出てきたら、インストール完了です。

   //hugo ヘルプコマンド

   hugo help

## HUGO動作手順

1. Hugo作業用フォルダ作成

   2.で作成したフォルダ(Hugo)に移動

   //2.作成したフォルダ(Hugoフォルダ)に移動

   cd C:\Hugo\

   * 新しくHugo作業用フォルダ作成する場合

   Hugoの初期フォルダを作る
   VMの作業フォルダという感じです。

   //初期フォルダを作る

   hugo new site 好きなサイト名

   * gitから作業用フォルダをcloneする場合(faqサイト)

   下記のリンクからcloneするためのURLやkey取得

   [https://github.com/bizoope/faq]

   2.で作成したフォルダ(Hugo)配下にcloneする。

   フォルダ構成としては、

    ```cmd
    C:.
    ├─bin
    └─faq
       ├─archetypes
       ├─assets
       ├─content
       ├─data
       ├─layouts
       ├─public
       ├─static
       └─themes
    ```

2. サイトプレビュー生成

   先ほど作成したHugo作業用フォルダに移動

   cd C:\Hugo\faq

   下記コマンドでサーバ起動

   ```cmd
   hugo server -D
   ```

   localhost:1313で確認
