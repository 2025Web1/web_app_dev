---
sort: 4
---

# GitHub Classroom②

本授業では、 **GitHub Classroom** を利用して課題の提出を行います。
課題の提出方法を以下に示しますので、手順に従って提出してください。

## ファイルの変更をステージングエリアに追加(add)

![](./images/git_image_add.jpg){: style="width: 660px;height: auto;" }

1. 課題として提出するフォルダをVSCodeで開く<br>
   VSCodeのメニューから「ファイル->フォルダーを開く」を選択し、`C:¥web_app_dev¥01-git...`を選択してください。
2. `kadai.txt`を開き、「A.」の横に好きな食べ物を入力し、保存する
3. VSCodeサイドバーのGit Graphのアイコン![](./images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.016.png){: style="width: 660px;height: auto;" }をクリック
4. 変更の欄に`kadai.txt`が表示されていることを確認し、+ボタンをクリック<br>
![](./images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.019.png){: style="width: 660px;height: auto;" }
5. `kadai.txt`がステージされている変更に移動していれば、addは成功

## ファイルの変更をコミット(commit)

![](./images/git_image_commit.jpg){: style="width: 660px;height: auto;" }

commitを行うためには、変更理由を記録する必要があります。
最初に変更理由の記録からはじめます。

1. メッセージの欄に変更理由を入力<br>
   ここでは「好きな食べ物を入力」とします。<br>
    ![](./images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.020.png){: style="width: 660px;height: auto;" }

1. ✔のボタンを押すとcommitは完了です。

```note
### commitのメッセージを入れ忘れると...

commitメッセージを入れ忘れると、commitができません。
解決するには、`COMMIT_EDITMSG`というファイルが開かれるので、1行目に変更理由を入力して保存すればcommitできます。
```

## GitHub Classroomに提出(push)

![](./images/git_image_push.jpg){: style="width: 660px;height: auto;" }

あとは課題を提出するのみです。

1. 変更の同期ボタンをクリック<br>
   ![](./images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.022.png){: style="width: 660px;height: auto;" }
2. GitHub Classroomのリンクにアクセスし、編集内容が反映されていればOK<br>
![](./images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.021.png){: style="width: 660px;height: auto;" }
3. kadai.txtを押して、中身が変わっていればOK
![](./images/Aspose.Words.aedafcf0-3819-4263-af12-50337a38362b.023.png){: style="width: 660px;height: auto;" }
4. 提出完了<br>
   今後の課題は、このようにGitHub Classroomに提出してもらいます。
