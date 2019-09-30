# CSS基本選擇器

![](../.gitbook/assets/image%20%285%29.png)

### 選擇器\(Selector\)：

CSS選擇器最常用的幾種如下

選擇器\(Selector\)：是一種模式，用於選擇你要添加的HTML 樣式元素。種類分成以下幾種

### Class \(類別選擇器\)

Class，「類別」選擇器，使用「.」開頭，Class名稱可自訂，一個class屬性值可以用在多個網頁上，**名稱大小寫也代表不一樣的Class**。

Class宣告的方法:  .Class屬性名稱

```css
/**Class選擇器**/
.TitleBanner{
width:100%;
height:50%;
background-color:#fd7676;
}
```

```markup
<!--將以上樣式套用在 HTML 內-->
<div class="TitleBanner">此段會套用Class</div>
```

### ID 選擇器

ID 選擇器，使用「\#」開頭，Class名稱也可以自訂，但一個ID名稱，只能在一個網頁文件上**使用一次**。且ID命名**不能有空格，名稱大小寫也代表不一樣的ID**。

_ID宣告的方法: \# id名稱_

```markup
#TitleBanner 和 #tablebanner 兩個名稱代表不同ID
```

```css
/**ID選擇器，**/
#TitleBanner{
width:100%;
height:50%;
background-color:#fd7676;
}
```

```markup
<!--將以上樣式套用在 HTML 內-->
<div id="TitleBanner">此段會套用Class</div>
```

### element selector\(元素選擇器\)

設定在HTML的屬性標籤上，一旦設定，全站往網頁都會套用。

```css
h1 {color:red;}
p {color:black;font-size:25px;}
```

### Universal selector（屬性選擇器）

使用字元「**\***」，整個網頁下的所有元素都會套用。

```css
* {color:red;}
```

### Attribute selectors（屬性選擇器）

屬性選擇器優點是不需要額外替這些網頁元素設定ID或是Class就可以選擇設定它。

常見的 CSS Attribute Selectors 語法有：

* **`[attr]`**  用於選取 **帶有指定屬性** 的元素。
* **`[attr=value]`**  用於選取 **帶有指定屬性和值** 的元素。
* **`[attr~=value]`**  用於選取 **屬性值中包含指定詞彙** 的元素。
* **`[attr|=value]`**  用於選取 **帶有以指定值開頭的屬性值** 的元素，該值必須是整個單詞。
* **`[attr^=value]`**  匹配 **屬性值以指定值開頭** 的每個元素。
* **`[attr$=value]`**  匹配 **屬性值以指定值結尾** 的每個元素。
* **`[attr*=value]`**  匹配 **屬性值中包含指定值** 的每個元素。

####  **\[attr\]**

```css
/**此語法意思是要選擇網頁中的圖片元素(img)，而且圖片要有標示title屬性的
才會被選取，沒有標示tiltle圖片屬性的就不會被選取。被選取到的圖片都會被加
上一個1px 的灰色 邊框**/
img[title] {
border: 1px gray solid;
}
```

####  **\[attr=value\]**

```css
/**此語法代表被選擇的網頁中圖片有title屬性且屬性的值是photo的圖片，沒有
photo的圖片就不會被選取**/
img[title="photo"] {
border: 1px gray solid;
}
```

 **\[attribute~=value\]**

```css
img[title~="photo1"] {
border: 1px gray solid;
}
```

```markup
<img src="圖片" title="photo1 good">
<img src="圖片" title="photo2 good">
```

