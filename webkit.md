---
description: 搭配瀏覽器寫CSS網頁才會正常
---

# 不同瀏覽器呈現不同CSS屬性

使用css3.0時，要知道瀏覽器前綴字\(Vender Prefixes\)觀念，因為有些瀏覽器階段功能還不支援一些新的css語法，如: 圖形圓角、 漸層、陰影........等。勢必要加上前綴字，效果才能生效。

![](.gitbook/assets/image%20%2830%29.png)

Firefox 用來顯示圓角的語法

```css
-moz-border-radius:25px; /*四個角一起設定*/
```

 **Google Chrome, Safari** 用來顯示圓角的語法

```css
webkit-border-radius:25px;
```

 **IE**

```css
border-radius: 15px;
/* Opera, 以及IE瀏覽器 */
-ms-border-radius: 15px; /* 針對IE9*/
```

###  [Can I use](https://caniuse.com/)

![](.gitbook/assets/image%20%2835%29.png)

#### 若要支援到很早期的瀏覽器，請務必將4組瀏覽器的前綴字全部寫出，但以目前現今的瀏覽器支援情況都已經很普及了，幾乎都只會寫到-webkit-就可以了。

