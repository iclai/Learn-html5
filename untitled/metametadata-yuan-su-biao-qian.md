# Meta\(Metadata\) 元素標籤

* Matadata主要為描述資料屬性的資訊，一般中文稱為元資料或詮釋資料。
* Matadata是屬於一個網頁非核心內容的資料，它針對頁面不同的軟件提供輔助的資訊說明。
* SEO\(search engine optimization\)搜尋引擎最佳化，_**很重要!!很重要!!很重要!!要說三次。**_

#### Metadata的主要屬性說明：

Title \(標題屬性\)，代表網頁的主題，影響你的網頁在Google搜尋排名， Title 標記理想的長度為 _**20~30 中文字**_，Title請撰寫明確、幫助使用者認識你的網站。 

![](../.gitbook/assets/image%20%2812%29.png)

####  定義四個屬性 \(attribute\) :

* name，設定網頁文件屬性定義名稱 
* http-equiv，設定網頁文件的狀態 
* Content，設定網頁屬性定義內容
* Charset，設定網頁字元編碼 

Property，專門給Facebook用的協議，社群媒體有它們自己專用的Meta使用方式，才能讓HTML META 屬性提供網頁的標題、縮圖、描述.....等資訊，呈現在各個平台上。

```markup
<meta property="fb:app_id" content="123456789">
<meta property="og:url" content="https://example.com/page.html">
<meta property="og:type" content="website">
<meta property="og:title" content="Content Title">
<meta property="og:image" content="https://example.com/image.jpg">
<meta property="og:description" content="Description Here">
<meta property="og:site_name" content="Site Name">
<meta property="og:locale" content="en_US">
<meta property="article:author" content="">
<!-- Facebook: https://developers.facebook.com/docs/sharing/webmasters#markup -->
<!-- Open Graph: http://ogp.me/ -->
```

