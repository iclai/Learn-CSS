# CSS基本選擇器\(一\)

![](../.gitbook/assets/image%20%285%29.png)

### 

### 選擇器\(Selector\)：

選擇器\(Selector\)：是一種模式，用於選擇你要添加的HTML 樣式元素。種類分成以下幾種

### Class \(類別選擇器\)

Class，「類別」選擇器，使用「.」開頭，Class名稱可自訂，一個class屬性值可以用在多個網頁上。

```css
/**Class選擇器**/
.TitleBanner{
width:100%;
height:50%;
background-color:#fd7676;
}
```

```markup
<div class="TitleBanner">此段會套用Class</div>
```

### ID 選擇器

ID 選擇器，使用「\#」開頭，Class名稱也可以自訂，但一個ID名稱，只能在一個網頁文件上**使用一次**。且ID命名**不能有空格**。

```css
/**ID選擇器**/
#TitleBanner{
width:100%;
height:50%;
background-color:#fd7676;
}
```

```markup
<div id ="TitleBanner">此段會套用Class</div>
```

### Type selectors（型態選取器）

設定在HTML的屬性標籤上，一旦設定，全站往網頁都會套用。

```css
h1 {color:red;}
p {color:black;font-size:25px;}
```

### Universal selector（通用選取器）

使用字元「**\***」，整個網頁下的所有元素都會套用。

```css
* {color:red;}
```

### Attribute selectors（屬性選取器）

屬性選擇器優點是不需要額外替這些網頁元素設定ID或是Class就可以選擇設定它。

常見的 CSS Attribute Selectors 語法有：

* **`[attribute]`**  用於選取 **帶有指定屬性** 的元素。
* **`[attribute=value]`**  用於選取 **帶有指定屬性和值** 的元素。
* **`[attribute~=value]`**
* **`[attribute|=value]`**
* **`[attribute^=value]`**
* **`[attribute$=value]`**
* **`[attribute*=value]`**

####  **\[attribute\]**

```css
/**此語法意思是要選擇網頁中的圖片元素(img)，而且圖片要有標示title屬性的
才會被選取，沒有標示tiltle圖片屬性的就不會被選取。被選取到的圖片都會被加
上一個1px 的灰色 邊框**/
img[title] {
border: 1px gray solid;
}
```

####  **\[attribute=value\]**

```css
/**此語法代表被選擇的網頁中圖片有title屬性且屬性的值是photo的圖片，沒有
photo的圖片就不會被選取**/
img[title="photo"] {
border: 1px gray solid;
}
```

