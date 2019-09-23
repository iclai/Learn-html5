# Meta\(Metadata\) 元素標籤

* Matadata主要為描述資料屬性的資訊，一般中文稱為元資料或詮釋資料。
* Matadata是屬於一個網頁非核心內容的資料，它針對頁面不同的軟件提供輔助的資訊說明。
* SEO\(search engine optimization\)搜尋引擎最佳化，_**很重要!!很重要!!很重要!!要說三次。**_

## Metadata的主要屬性說明：

Title \(標題屬性\)，代表網頁的主題，影響你的網頁在Google搜尋排名， Title 標記理想的長度為 _**20~30 中文字**_，Title請撰寫明確、幫助使用者認識你的網站。 

![](../.gitbook/assets/image%20%2861%29.png)

###  定義屬性 \(attribute\) :

* \*\*\*\*[**Name**](meta-element-tag.md#name-chang-yong-de-content-she-ding-shu-xing-you)**，設定網頁文件屬性定義名稱** 
* \*\*\*\*[**Http-equiv**](meta-element-tag.md#httpequiv-de-content-she-ding-shu-xing-you)**，設定網頁文件的狀態** 
  * **Content，設定網頁屬性定義內容**
  * **Charset，設定網頁字元編碼** 

###  **Name常用的屬性：**

* description \(描述，內容的主要描述\)
* keywords \(關鍵字\) 
* author \(作者，標註本網頁作者姓名等資料\)
* copyright \(版權宣告，本網頁由XXX設計， 用來標示網頁的版權或著作權聲明\) 
* generator \(編輯器，編輯器等版本說明\) 

```markup
<meta name="description" content="對網頁的簡短描述">
```

Meta Description\(網頁描述\)是HTML屬性，提供簡短的網頁摘要。通常出現在搜尋引擎結果頁面。

![description&#x63CF;&#x8FF0;&#x7684;&#x6587;&#x5B57;&#x6703;&#x51FA;&#x73FE;&#x5728;&#x641C;&#x5C0B;&#x5F15;&#x64CE;](../.gitbook/assets/image%20%2841%29.png)

![description&#x63CF;&#x8FF0;&#x7684;&#x6587;&#x5B57;](../.gitbook/assets/image%20%2826%29.png)

* Description \(敘述屬性\)，包含頁面內容的簡短和精確的描述，描述頁面的主要內容，幫助用戶判斷是否是他要搜尋的資訊，並著重在提升用戶體驗、點擊率。
* Description 的字數雖然沒有限制，但搜尋引擎會在超過 160 字元 時，把多的字截短，_**理想長度為50-80中字元。**_
* Google 在 2009 就宣布 meta descriptions 和 meta keywords 都不會影響 Google ranking ，只有在 Google 的進階搜尋時才會使用 meta descriptions，也就是說，description 吸引用戶點擊，點擊數才會影響排名。_**\(意思就是文字內容吸不吸引人很重要\)**_

#### Keyword \(關鍵字屬性\)

* Keyword 對 _**SEO 已經沒有效**_
* Keyword 裡面有刻意堆疊過多的關鍵字（比方說裡面塞個20組以上的關鍵字），建議將它移除，避免被搜尋引擎判定我們有意圖作弊的嫌疑。

#### author\(作者\)

```markup
<meta name="author" content="輸入網頁製作者的資料">
```

![](../.gitbook/assets/image%20%2812%29.png)

#### copyright\(版權\)

```markup
<meta name="copyright" content="xx"> <!--代表該網站為xx個人版權所有>-->
```

copyright 這個 meta 已經不常使用了。建議移除它並創建一個專屬版權頁面

#### generator\(網頁製作軟體，標明網頁是什麼軟體做的\)

```markup
<meta name="generator" content="Visual Studio Code">
```

### http-equiv屬性:

相當於HTTP的作用， **http-equiv**屬性為指定所要模擬的標頭欄位的名稱，**content**屬性用來提供值。

```markup
<meta http-equiv="引數" content="具體的描述">
```

* content-type
* content-language
* X-UA-Compatible
* refresh

#### content-Type\(設定網頁字符集Charset\)

```markup
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
```

```markup
<meta charset="UTF-8" />  <!--符合HTML5設定網頁字符集的方式，推薦使用-->
```

將charset縮短成上面那樣，所有的瀏覽器還是會做出相同判定（甚至包括Internet Explorer 6），所以最好用新的寫法

Charset\(字元編碼屬性\)一般使用通用字元集**utf-8**編碼，幾乎任何語言都可用，也代表你的網頁可以顯示處理任何語言

![](../.gitbook/assets/image%20%282%29.png)

#### content-language \(告知搜尋引擎網頁屬於中文網站\)

```markup
<meta http-equiv="content-language" content="zh-tw">
```

 相關 ZH 編碼有，台灣繁體 ZH-tw、香港繁體 ZH-hk、中國簡體 ZH-cn、新加坡簡體 ZH-sg  


#### X-UA-Compatible\(告訴瀏覽器採取何種版本渲染當前頁面，一般都設定為最新模式\)

```markup
<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"/> <!--指定IE和Chrome使用最新版本渲染當前頁>-->
```

#### refresh\(自動重新整理並指向某頁面\)

網頁將在設定的時間內，自動重新整理並調向設定的網址。

```markup
<meta http-equiv="refresh" content="2；URL=https://www.yahoo.com.tw"> <!--意思是2秒後跳轉到yahoo>-->
```

## Open graph的使用方法

Open graph 專門給Facebook用的協議， 它與 meta tag 非常相似，社群媒體有它們自己專用的Meta使用方式，才能讓HTML META 屬性提供網頁的標題、縮圖、描述.....等資訊，呈現在各個平台上。

它和Meta tag 寫法沒有太大差別，只有在Property的值不同而已

```markup
<meta property="fb:app_id" content="APPID">
<meta property="og:url" content="https://xxx.com/page.html">
<meta property="og:type" content="類型"> <!--有article, book, profile, website, music, video等類型，預設是 “website”-->
<meta property="og:title" content="文章標題">
<meta property="og:image" content="https://xxx.com/image.jpg">  <!--預覽圖 URL，必須大於 200x200，建議大小 600 x 314 最適合顯示-->
<meta property="og:description" content="描述簡介或摘要">
<meta property="og:site_name" content="網站名稱">
<meta property="og:locale" content="zh_TW">
```

![](../.gitbook/assets/image%20%2867%29.png)

#### Metadata 的 og:Tag屬性說明

```markup
<meta property="og:title" content="Apple (台灣)">
<meta property="og:description" content="探索 Apple 的創新世界，選購各式 iPhone、iPad、Apple Watch、Mac 與 Apple TV，發現眾多配件、娛樂產品，並取得有關裝置的專家支援服務。">
<meta property="og:image" content="https://www.apple.com/ac/structured-data/images/open_graph_logo.png?201810272230">
```

![](../.gitbook/assets/image%20%2862%29.png)

![og:image&#x6C92;&#x6709;&#x653E;&#x5165;&#x5716;&#x7247;&#x8DEF;&#x5F91;](../.gitbook/assets/image%20%2847%29.png)

![FB&#x5716;&#x7247;&#x5C31;&#x4E0D;&#x6703;&#x51FA;&#x73FE;](../.gitbook/assets/image%20%2870%29.png)

#### 完整的Property屬性設定，就會有良好的網站曝光率及點擊率!!

![](../.gitbook/assets/image%20%2815%29.png)

