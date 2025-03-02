# Git、GitHub

## 作成と提出

### テキストファイルの追加(add)

1. 課題として提出するファイルをVSCodeで開きます。VSCodeのメニューから「ファイル->フォルダーを開く」を選択し、`C:¥web_app_dev¥01-git...`を選択します。
2. `kadai.txt`を開きます。「A.」の横に好きな食べ物を入力し、保存してください。
3. VSCodeサイドバーのGit Graphのアイコン<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.016.png?raw=true">を押します。
4. 変更の欄に`kadai.txt`が表示されていることを確認し、+ボタンを押します。<br>
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.019.png?raw=true">

1. `kadai.txt`がステージされている変更に移動していれば、addは成功です。

<div style="page-break-before:always"></div>

### テキストファイルをコミット(commit)する

commitを行うためには、変更理由を記録する必要があります。最初に変更理由の記録からはじめます。

1. メッセージの欄に変更理由を入力します。ここでは「好きな食べ物を入力」とします。※メッセージを入力しないとcommitできないので、今後も注意！<br>
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.020.png?raw=true">

2. ✔のボタンを押すとcommitは完了です。<br><br>

### テキストファイルをプッシュ(push)する

あとは課題を提出するのみです。

1. 変更の同期ボタンを押します。<br><img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.022.png?raw=true">

1. ブラウザで、再度課題のリンクにアクセスすると(cloneで使ったURLでも良い)、編集内容が反映されているのがわかります。(kadai.txtを押して、中身も変わっているか確認しましょう。)<br>
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.021.png?raw=true">
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.023.png?raw=true">

1. 提出完了です。今後の課題は、このようにGitで提出してもらいますので、よろしくお願いします。<br><br>

<div style="page-break-before:always"></div>

## 付録(Git関連の用語説明)

- **リポジトリ（Repository）**: Gitで管理されるプロジェクトの全ての変更履歴やファイルを保存するデータベースのようなものです。

- **ローカルリポジトリ（Local Repository）**: プロジェクトを自分のローカル環境に複製したリポジトリのことです。自分のPCやサーバーに保存されており、ローカルで変更を加え、コミットやプッシュを行うことができます。

- **リモートリポジトリ（Remote Repository）**: プロジェクトを共有するために、複数の開発者がアクセスできるリポジトリのことです。一般的には、オンラインのGitリポジトリホスティングサービス（例: GitHub, GitLab, Bitbucketなど）に保存されています。
  
- **ステージングエリア(staging area)**: リポジトリにコミットする前に変更を一時的に準備する場所です。ステージングエリアを使用することで、コミットする前に変更の内容を選択的に追加 (ステージ) し、コミットすることができます。

- **クローン(clone)**: リモートリポジトリを自分のローカル環境に複製することを指すコマンドです。リモートリポジトリの全ての履歴やファイルを自分のPCにコピーし、ローカルリポジトリを作成します。

- **プル(pull)**: リモートリポジトリから最新の変更を取得して自分のローカルリポジトリを更新する操作です。

- **アド(add)**: Gitで変更をステージングエリアに追加するコマンドです。ステージングエリアに追加された変更は、次のコミットに含まれます。

- **コミット(commit)**: ステージングエリアにある変更をローカルリポジトリに記録するコマンドです。コミットは、変更の履歴を残し、特定のスナップショットを作成します。

- **プッシュ(push)**: ローカルリポジトリの変更をリモートリポジトリに反映するコマンドです。変更をリモートリポジトリに送信し、共有されたプロジェクトに変更を適用します。<br><br>
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/git_image.jpg?raw=true">
