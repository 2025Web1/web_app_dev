# CSS(Cascading Style Sheets)

先ほどお見せした以下の画面ですが、お世辞にも綺麗な画面とは言えませんね...

![](./images/sampleNoCSS.png){: style="width: 660px;height: auto;" }

この問題を解決するために、先ほどのHTMLにCSSを反映させましょう。

## CSSとは

Webページの見た目を指定する言語です。
CSSは、HTMLで定義された構造にスタイルを適用することで、Webページを美しく、見やすくデザインすることができます。

それでは、先ほどのHTMLにCSSを反映させていきましょう。
`sample.html`に、`sample.css`を反映するためのコードを追加します。

```html
<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8">
    <!-- 以下の一文を追加 -->
    <link rel="stylesheet" href="sample.css">
    <!-- ここまで -->
    <title>サンプルWebページ</title>
  </head>
  <body>
    <h1>サンプルWebページ</h1>
    
    <p>
      ようこそ、サンプルWebページへ!ここでは、「商品紹介ページ」という設定の元で、HTML&CSSの参考例を見ていきましょう。
      <img src="pose_gutspose_couple.png" alt="サンプル画像">
    </p>
  
    <table>
      <tr>
        <th>商品名</th>
        <th>説明</th>
        <th>金額</th>
      </tr>
      <tr>
        <td>商品 A</td>
        <td>お求めやすい金額の商品です。</td>
        <td>¥300</td>
      </tr>
      <tr>
        <td>商品 B</td>
        <td>一般的な金額の商品です。</td>
        <td>¥3,000</td>
      </tr>
      <tr>
        <td>商品 C</td>
        <td>高級な金額の商品です。</td>
        <td>¥30,000</td>
      </tr>
    </table>
    
    <p>ご不明な点がございましたらお問合せください。 
      <a href="https://www.kobedenshi.ac.jp/">詳細はこちら</a>
    </p>
    
    <form>
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required>
      <label for="email">Email:</label>
      <input type="text" id="email" name="email" required>
      <label for="message">Message:</label>
      <textarea id="message" name="message" required></textarea>
      <input type="submit" value="Send">
    </form>
  </body>
</html>
```



```html:sample.html
<!-- <link rel="stylesheet" href="sample.css"> -->
```

コメントの外し方は、該当の行で`Ctrl + /`です。
コメントを外すと以下のようになります。

```html:sample.html
<link rel="stylesheet" href="sample.css">
```

では、もう一度ブラウザで`sample.html`を開いてみてください。CSSが動き、画面が綺麗になりました。<br>
![](./images/sampleCSS.jpg)
