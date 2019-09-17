# Meta\(Metadata\) 元素標籤

* Matadata主要為描述資料屬性的資訊，一般中文稱為元資料或詮釋資料。
* Matadata是屬於一個網頁非核心內容的資料，它針對頁面不同的軟件提供輔助的資訊說明。
* SEO\(search engine optimization\)搜尋引擎最佳化，_**很重要!!很重要!!很重要!!要說三次。**_

### Metadata的主要屬性說明：

Title \(標題屬性\)，代表網頁的主題，影響你的網頁在Google搜尋排名， Title 標記理想的長度為 _**20~30 中文字**_，Title請撰寫明確、幫助使用者認識你的網站。 

![](../.gitbook/assets/image%20%2815%29.png)

###  定義四個屬性 \(attribute\) :

* \*\*\*\*[**Name**](metametadata-yuan-su-biao-qian.md#name-chang-yong-de-content-she-ding-shu-xing-you)**，設定網頁文件屬性定義名稱** 
* \*\*\*\*[**Http-equiv**](metametadata-yuan-su-biao-qian.md#httpequiv-de-content-she-ding-shu-xing-you)**，設定網頁文件的狀態** 
* **Content，設定網頁屬性定義內容**
* **Charset，設定網頁字元編碼** 

###  **Name常用的content設定屬性有：**

* description \(描述，內容的主要描述\)
* keywords \(關鍵字\) 
* author \(作者，標註本網頁作者姓名等資料\)
* generator \(編輯器，編輯器等版本說明\) 
* copyright \(版權宣告，本網頁由XXX設計， 用來標示網頁的版權或著作權聲明\) 
* distribution \(用來記錄網頁的發佈地區\)

`<meta name>="description" content="對網頁的簡短描述">`

Meta Description\(網頁描述\)是HTML屬性，提供簡短的網頁摘要。通常出現在搜尋引擎結果頁面。

![description&#x63CF;&#x8FF0;&#x7684;&#x6587;&#x5B57;&#x6703;&#x51FA;&#x73FE;&#x5728;&#x641C;&#x5C0B;&#x5F15;&#x64CE;](../.gitbook/assets/image%20%289%29.png)

![description&#x63CF;&#x8FF0;&#x7684;&#x6587;&#x5B57;](../.gitbook/assets/image%20%284%29.png)

* Description \(敘述屬性\)，包含頁面內容的簡短和精確的描述，描述頁面的主要內容，幫助用戶判斷是否是他要搜尋的資訊，並著重在提升用戶體驗、點擊率。
* Description 的字數雖然沒有限制，但搜尋引擎會在超過 160 字元 時，把多的字截短，_**理想長度為50-80中字元。**_
* Google 在 2009 就宣布 meta descriptions 和 meta keywords 都不會影響 Google ranking ，只有在 Google 的進階搜尋時才會使用 meta descriptions，也就是說，description 吸引用戶點擊，點擊數才會影響排名。_**\(意思就是文字內容吸不吸引人很重要\)**_

#### Keyword \(關鍵字屬性\)

* Keyword 對 _**SEO 已經沒有效**_
* Keyword 裡面有刻意堆疊過多的關鍵字（比方說裡面塞個20組以上的關鍵字），建議將它移除，避免被搜尋引擎判定我們有意圖作弊的嫌疑。

### http-equiv的content設定屬性有:

* content-type
* content-language
* refresh
* Pragma
* windows-Target



Property，專門給Facebook用的協議，社群媒體有它們自己專用的Meta使用方式，才能讓HTML META 屬性提供網頁的標題、縮圖、描述.....等資訊，呈現在各個平台上。

```markup
<meta property="fb:app_id" content="APPID">
<meta property="og:url" content="https://xxx.com/page.html">
<meta property="og:type" content="類型">
<meta property="og:title" content="文章標題">
<meta property="og:image" content="https://xxx.com/image.jpg">
<meta property="og:description" content="這是一段簡介文字">
<meta property="og:site_name" content="網站名稱">
<meta property="og:locale" content="zh_TW">
<meta property="article:author" content="">
<!-- Facebook: https://developers.facebook.com/docs/sharing/webmasters#markup -->
<!-- Open Graph: http://ogp.me/ -->
```

