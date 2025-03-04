---
sort: 2
---
# HTML(HyperText Markup Language)

## HTMLとは

Webページを作るために使われるマークアップ言語の一つです。
マークアップ言語とは、文章やデータなどのテキスト情報に対して、意味や構造を付与するための言語です。
Webページには、テキスト、画像、動画、音声など様々なコンテンツが含まれます。
HTMLはこれらのコンテンツをどのように表示するかを指定するために使われます。

具体的には、HTMLでは各コンテンツに対して「タグ(<>)」と呼ばれる特定の記号を使って囲みます。
タグによって要素の意味や構造を示します。
例えば、`<p>`というタグは段落を表し、`<img>`というタグは画像を表します。

## HTMLを書いてみよう

cloneした`02_htmlcss-...`は以下の構造をしています。
※ちなみにcloneした  `02_htmlcss-...`の`...`には、Githubアカウントのユーザー名が入ります。

```text
02_htmlcss-...
├── helloWorld.html
├── sample.css
└── sample.html
```

`helloWorld.html`を開き、以下のコードを入力してください。<br>
※`<!-- -->`はHTMLのコメントアウトを表します。
コメントアウトされた部分はブラウザに表示されません。

`helloWorld.html`
```html:helloWorld.html
<!DOCTYPE html>
<html lang="ja">
    <head>
        <meta charset="UTF-8">
        <title>Hello,World</title>
    </head>
    <body>
        <p>Hello,World</p>
        <p>0J0X0XX神戸電子</p>   <!--自分の出席番号と名前に書き換えてください-->
    </body>
</html>
```

入力後、ブラウザで`helloWorld.html`を開いてください。以下のように表示されればOKです。
![](./images/Hello%2CWorld.jpg)
