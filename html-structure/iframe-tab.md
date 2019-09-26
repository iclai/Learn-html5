# iFrame標籤

iframe標籤，可以將影片或是網頁嵌入到自己的網頁中。常常看到網頁中會有Google Map就是運用iFrame 原理。

iframe這個詞是 **`inline frame`** 的縮寫

![](../.gitbook/assets/image%20%28119%29.png)

```markup
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d14563.016505140535!2d120.68530421716306!3d24.145271433951766!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x34693d68cf62e061%3A0x7091dd73273f6236!2z5ZyL56uL6Ie65Lit56eR5oqA5aSn5a24!5e0!3m2!1szh-TW!2stw!4v1569311131898!5m2!1szh-TW!2stw" 
    width="600" 
    height="450" 
    frameborder="0" 
    style="border:0;" 
    allowfullscreen="">
</iframe>
```

### iframe屬性

* **`frameborder`**是否顯示邊框，**`1(yes), 0(no)`**
* **`height:height`**屬性指定 iframe 的像素高度，建議使用css設置。
* **`width:width`**屬性指定 iframe 的像素寬度，建議使用css設置。
* **`name`**iframe的名稱，**`window.frames[name]`** 時專用的屬性。
* **`scrolling`**設定iframe視窗是否可以捲動。**`yes, no, auto`**。
* **`src`**  iframe的網址。
* **`sandbox`**控制iframe 內的權限\(html5新功能\)。\([解說資料在此](https://msdn.microsoft.com/en-us/hh563496.aspx)\)

{% hint style="info" %}
HTML5 不推薦使用Frames,而不支持iFrames。
{% endhint %}

### iframe缺點

網頁盡量少用iframe

* iframe會阻礙主頁面的Onload事件
* 搜索引擎的檢索程序無法解讀這種頁面，對SEO排名不利。
* iframe和主頁面共享連接池，而瀏覽器對同域的連接有限制，所以會影響網頁的並行加載。

> 並行加載，意思是同一個時間，針對同一個域名下的請求。 一般情況，iframe和所有頁面在同一個網域下，瀏覽器的同時加載數量是有限制的。

所以，在使用iframe時，最好要先考慮到以上幾個缺點，如果真的需要，最好透過**`JavaScript`**動態給iframe添加**`src`**屬性，這樣可以避開同時加載的所產生的問題。

```javascript
<iframe id="fram"></iframe>
document.getelementbyid("fram").src="XXX.html"
```

### 嵌入youtube

![](../.gitbook/assets/image%20%2855%29.png)

![](../.gitbook/assets/image%20%2844%29.png)

![&#x8907;&#x88FD;youtube &#x8A9E;&#x6CD5;](../.gitbook/assets/image%20%2858%29.png)

![&#x7DB2;&#x9801;&#x5D4C;&#x5165;&#x5F71;&#x7247;](../.gitbook/assets/image%20%2813%29.png)

