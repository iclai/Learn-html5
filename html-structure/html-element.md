---
description: html 元素介紹
---

# Html element

## html 元素

html 元素內容，會有一個起始標籤，和結束標籤

起始標籤 **\(opening tag\)**包含了**&lt;   &gt;**   這兩個符號，元素名稱就寫在**&lt;  &gt; 符號**裡面。

結束標籤 **\(closing tag\)**和起始標籤長的差不多，只是多了一個 **/ 斜線。**

html標籤通常都是對稱的，有開始就會有結束標籤，成對出現。

 **內容\(content\):** 就是元素的內容。如下圖。

**起始標籤 + 結束標籤 + 內容 = 就是元素**

![](../.gitbook/assets/image%20%2828%29.png)

### 元素屬性 \(element attribute\)

* 元素可以加入 屬性
* 屬性包含 【名稱】、【值】
* 可以利用屬性設定這個元素的色彩、對齊方式、圖表的格線等等。

![](../.gitbook/assets/image%20%2833%29.png)

#### 屬性的組成包含:

* 元素名稱和屬性之間有一個空格  如上方 **`<p style="......."> p和style中間有空一格`**
* 屬性名稱後面接著等於符號**`「=」`**
* 屬性包在起始標籤裡面

```markup
<p style="color:#0987b5;">這是我第一個網頁</p>
```

![](../.gitbook/assets/image%20%2829%29.png)

### 巢狀元素（nesting element）

* 元素裡面可以在放進元素，稱之為「巢狀元素（nesting element）」
* 標籤巢狀元素，若你想強調「第一個」，就把「第一個」這三個字自成一個顯示為粗體的元素 
* HTML 標籤不分英文大小寫。也就是說，它們可以寫成英文全大寫、全小寫、或是混在一起。像是 &lt;title&gt; 能寫成 &lt;Title&gt;、&lt;TiTle&gt;

![](../.gitbook/assets/image%20%2848%29.png)

### 空元素（empty elements）

在HTML中有些元素沒有內容，組合沒有語意上的意義，稱為「空元素（empty elements）」。

在HTML中。空元素上使用結束標籤通常是無效的，例如: 

```markup
<input type="text"></input>
```

在 HTML 中的空元素：

```markup
<base>
<br>
<col>
<colgroup>
<command>
<embed>
<hr>
<img>
<input>
<keygen>
<link> 
<meta>
<param>
<source>
<track>
<wbr>
```

![&#x4EE5;&#x9019;&#x500B;&#x5716;&#x7247;&#x5143;&#x7D20; &amp;lt;img&amp;gt;&#x70BA;&#x4F8B;](../.gitbook/assets/image%20%2854%29.png)

```markup
<img src="https://i.imgur.com/ttAYRxX.gif" alt="小小兵">
```

它有兩個屬性，但是沒有結束標籤，也沒有裡面的內容。因為圖片元素是直接把圖檔嵌在 HTML 網頁上。

![](../.gitbook/assets/image%20%2843%29.png)

### 圖片 <a id="&#x5716;&#x7247;"></a>

#### img元素

 圖片是直接把圖檔嵌入在HTML網頁裡面，它是透過圖片來源（`src` ，source）這個屬性，提供了連到圖片檔案的路徑。

alt屬性，是運用在當網頁瀏覽者，無法正確看到圖片時，用說明文字來代替圖片，通常會用在

* 視障者網頁，視障者會使用Screen Readers工具讀出網頁，所以圖片說明文字就可以幫助他們了解網頁內容。
* 假設你誤植了圖片路徑來源，網頁無法顯示圖片時，說明文字就會顯示。

title屬性，當滑鼠滑過圖片上方時，會顯示圖片文字標示，可以增加瀏覽者對該張圖片的辨識。

![](../.gitbook/assets/image%20%2860%29.png)

