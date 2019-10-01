# CSS 套用方法

如何將CSS 套用進HTML 裡面?

#### 有以下4種方式:

![](.gitbook/assets/image%20%284%29.png)

###  **行內\(inline\)套用**

直接在 HTML 標籤中使用 style 屬性指定 CSS 樣式。

```markup
<h2 style="color: blue; font-size:50px;">這是主標題</h2>
```

![](.gitbook/assets/image%20%286%29.png)

這寫法很直覺，但如果HTML很多行，你每一行都都單獨設定CSS樣式，到時後要修改或是維護會很麻煩，所以不建議將CSS樣式寫在HTML行內裡。

###  **HTML 內部載入**

將CSS寫在HTML文件的頭部&lt;head&gt;元素中。

```markup
<head>
  <style>
    h2 {
      color: #f00909;
      font-size: 50px;
    }
  </style>
  </head>
```

```markup
<h2>這是主標題</h2>
```

![](.gitbook/assets/image%20%288%29.png)

將CSS寫在HTML的&lt;head&gt;中，雖然是有將CSS和HTML分開，但寫在單獨這一頁的CSS就只能給這一頁的HTML用而已，其他的HTML頁面無法共用，除非是這一頁獨有樣式，才會這樣寫，所以也不建議這種編寫方式。

### 載入外部 CSS

將CSS另外存成一個 .CSS檔案，並從HTML的&lt;head&gt;引入進來， 引入的方法有2種方式。

* **link 元素**
* **＠import**

### 載入link

```css
.title {
  color: #11b843;
  font-size: 50px;
}
```

```markup
<h2 class="title">這是主標題</h2>
```

![](.gitbook/assets/s.jpg)



