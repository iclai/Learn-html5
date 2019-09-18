---
description: HTML文件的組成
---

# HTML結構

## HTML 的結構分為三大部分

* 宣告
* Head
* Body

#### 第一部分 ，宣告

透過此標籤，告訴瀏覽器，我們後面要開始使用HTML語言，這樣瀏覽器會理解，並將後面的HTML語言解讀出來，呈現在瀏覽器上。

```markup
<!DOCTYPE html>
```

#### 第二部分，head

head專門放網頁重要資訊，包括要引用的外部CSS、Javascript、文字、這些不會顯示在網頁上，所以使用者看不到。

包含 `<meta>  <title>   <link>   <script>`

```markup
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>HTML結構</title>
</head>
```

#### 第三部分，body

包含了所有會顯示於網頁瀏覽者眼前的內容。 無論是文字、圖片、影面、互動遊戲...等。

```markup
<body>

  <h1>我是大標題</h1>
  <p>我是文章內文</p>
  
</body>
```

![](../.gitbook/assets/image%20%2832%29.png)

