# Git、GitHub

## 課題へのアクセス、受諾

課題ページは[こちら](https://classroom.github.com/a/QM3UUgtQ)

1. GitHubアカウントでログインしてください
2. GitHub Classroomには既に皆さんの名前を登録しています、自分の名前を選んでクリックして進めてください<br>
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/join_the_classroom.png?raw=true"><br><br>
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.009.png?raw=true"><br><br>
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/accept_the_assignment.png?raw=true">

1. 招待の受け入れをすると、課題リポジトリのリンクが表示されます。リンクが表示されない場合は、ブラウザをリロードしてください。<br>
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/repository_link.png?raw=true">

1. リポジトリリンク(上記の水色背景の行)をクリックすると、課題用に作成されたリポジトリにアクセスできます。
2. clone(取得)用のURLは、緑のボタン(code)から確認できます。httpsを選び、コピー用のボタンでクリップボードに一度取り込んでください。<br>
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.013.jpeg?raw=true">

### Gitの下準備

初めてGitを使う方は、commit(登録)の際に使う名前とメールアドレスを登録しましょう。 PowerShellもしくはコマンドプロンプトから下記コマンドを実行してください。**{}の入力はいりません。自分の名前、メールアドレスは半角英数字で！**

```shell
git config --global user.name {自分の名前}
git config --global user.email {メールアドレス}
```

確認には、下記コマンドを実行します。出力に`user.name`と`user.email`の項目があるので、設定したとおりになっていればOKです。

```shell
git config --list
```

<br>

### VSCode(Visual Studio Code)でのコード取得

#### プラグインJapanese Language Pack for Visual Studio Codeインストール

1. VSCodeにて、Ctrl+Shift+Xを同時に押します
1. "Search Extentions in Marketplace"の欄に"japan"と入力します
1. "Japanese Language Pack for Visual Studio Code"のInstallボタンを押します
1. インストール後、再起動を求められるので再起動します
1. VSCodeのメニューなどが日本語になっていればOK。(なお、VSCode自体の更新がかかると、度々日本語化が失われるときがあります。その場合は、このプラグインを再インストールするとOKです。)

#### プラグインGit Graphインストール

1. 本授業のclone用フォルダ `C:¥web_app_dev` を作成してください。
2. VSCodeにて、Ctrl+Shift+Xを同時に押します。
3. "Search Extentions in Marketplace"の欄に"Git Graph"と入力します。
4. "Git Graph"のInstallボタンを押します
5. インストールが完了し、サイドバーにGit Graphのアイコン<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.016.png?raw=true">が追加されていることを確認します。
6. Git Graphのアイコンをクリックし、リポジトリのクローンを押します。(もしくは、`Ctrl+Shift+P`を押し、フォームに`git: clone`と入力し、`Git:クローン`を押すのでも可)先ほどコピーしたリポジトリのURLを貼り付け、Enterを押してください。
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.017.png?raw=true"><br>

7. フォルダの選択画面になるので、`C:¥web_app_dev` フォルダを選択してください。
8. 認証を求められるので、ブラウザでアカウントを入れて認証してください。(※求められなければ無視してください。)<br>
<img src="https://github.com/2024Web1/web_app_dev/blob/main/git/images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.018.jpeg?raw=true">

9. 認証に成功すれば、`C:¥web_app_dev` 直下にコードがcloneできています。<br><br>

#### cloneできなかった場合

現象と解決策は下記のいずれかと考えられます。

1. `repository not found`とエラーが出る。<br>
  過去に別のGitHubアカウントを作成し、Gitを利用した経験がある方は、`repository not found`のエラーでcloneできない場合があります。その場合は、下記サンプルのように、cloneするリポジトリのURLに`ユーザー名@`を追記し、再度cloneをしてください。※このユーザー名はアカウント作成時に登録したユーザー名です。<br>
    ```
    https://ユーザー名@github.com/〜.git
    ```

1. cloneが終わらない。<br>
  エラーは出ないが、cloneがいつまで経っても終了しない場合があります。実際は、別ウインドウ・ブラウザで、GitHubアカウントの認証待ちの状態になっていることがあるので、認証を済ませてください。

1. `user.name`と`user.email`が設定できていない。<br>
  [Gitの下準備](#gitの下準備)に戻って、設定し直してください。

<div style="page-break-before:always"></div>

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
