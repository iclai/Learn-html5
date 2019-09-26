# 相對路徑和絕對路徑

### 絕對路徑

絕對路徑就是以網站的根目錄為參考，是一個絕對的位置，檔案在本機端或是網路端位置都是一樣的，不會隨著目錄改變而改變。



### 相對路徑

桌面上的網頁路徑，如果網頁要使用 `img01.jpg` 這張圖片，照片在images子目錄下。

![](../.gitbook/assets/image%20%28100%29.png)

![](../.gitbook/assets/image%20%28106%29.png)

```markup
img src="images/img01.jpg" 
```

現在資料夾中，又多了一個object資料夾，裡面有一個object.html 網頁

![](../.gitbook/assets/image%20%2871%29.png)

我要將img01.jpg 照片設定連結至object.html

```markup
 <!--相對路徑2-->
 <a href="./object/object.html">
    <img src="images/img01.jpg" alt="圖片01" width="300">
  </a>
```

object.html 中的照片要連結回 img.html 

```markup
<a href="../img.html"><img src="../images/img02.jpg" alt="圖片01" width="300"></a>
```

![](../.gitbook/assets/image%20%2894%29.png)

#### 相對路徑有幾個類別:

* **`XXX.html`** \(表示XXX.html在同一層資料夾目錄中\)
* **`images/XXX.html`** \(表示在同一層的image目錄下的XXX.html
* **`./XXX.html`** \(表示在同一層目錄中的XXX.html\)
* **`../XXX.html`** \(表示在上一層目錄中XXX.html檔案\)
* **`../object/XXX.html`** \(表示在上一層的目錄object資料夾中的object.html檔案\)

{% hint style="info" %}
通常用一個點 ．代表現在的目錄，用兩個點 ．．代表上一層目錄
{% endhint %}

使用相對路徑，目錄即使轉移，也不需要大幅修改網址。  
[https://lotus-seed.000webhostapp.com/my\_web/img.html](https://lotus-seed.000webhostapp.com/my_web/img.html)  

![&#x7DB2;&#x9801;&#x4E0A;&#x50B3;&#x81F3;&#x7DB2;&#x8DEF;&#x7A7A;&#x9593;](../.gitbook/assets/image%20%2889%29.png)



