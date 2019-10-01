# CSS 按鈕

### `<a>`的連結的顏色設定

![](.gitbook/assets/image%20%289%29.png)

```css
<!-- CSS 滑鼠效果設定-->
a {text-decoration: none;}

/* 有連結功能的顏色 */
a:link {color: rgb(7, 118, 245);}

/* 網址有被滑鼠點擊連結過的顏色 */
a:visited {color: rgb(102, 102, 102);}

/* 滑鼠滑過連結的顏色 */
a:hover {color: rgb(255, 72, 0);}

/* 滑鼠點擊選擇的連結 */
a:active {color: darkorchid;}
```

```markup
<h1>我的菜單食譜</h1>
  <ul>
    <li><a href="https://tw.yahoo.com/" target="_black">紅酒燉牛肉食譜</a></li>
    <li><a href="#">紅燒牛肉食譜</a></li>
    <li><a href="#">蔥爆牛肉食譜</a></li>
    <li><a href="https://www.momoshop.com.tw/" target="_black">沙茶青椒牛肉食譜</a></li>
  </ul>
```

![](.gitbook/assets/image%20%2810%29.png)

### 清單按鈕

清單連結CSS設定

![](.gitbook/assets/image%20%2817%29.png)

```css
/* 單獨設定第二個按鈕 */
    li a span {
      border: 2px dotted #ce1625;
      width: 198px;
      height: 28px;
      display: block;
    }
```

```markup
<h1>我的菜單食譜</h1>
  <ul class="menu">
    <li><a href="https://tw.yahoo.com/" target="_black">紅酒燉牛肉食譜</a></li>
    <li><a href="#"><span>紅燒牛肉食譜</span></a></li>
    <li><a href="#">蔥爆牛肉食譜</a></li>
    <li><a href="https://www.momoshop.com.tw/" target="_black">沙茶青椒牛肉食譜</a></li>
  </ul>
```

![](.gitbook/assets/image%20%2815%29.png)

