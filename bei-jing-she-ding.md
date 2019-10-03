---
description: 常用的網頁背景(Background)設定寫法
---

# 背景設定

background背景如果將CSS下在&lt;body&gt;上，預設會主動填滿背景，如是使用照片做背景也會不斷重複直到填滿背景，除非有下 `no-repeat` 圖片就不會重複填滿

![](.gitbook/assets/image%20%2815%29.png)

```css
background-color: orange;
```

![](.gitbook/assets/image%20%286%29.png)

```css
background: radial-gradient(yellow, red);
```

![](.gitbook/assets/image%20%2824%29.png)

```css
 background: url("../images/superwoman.jpg") no-repeat;
```

![](.gitbook/assets/image%20%2823%29.png)

```css
background-image: url("../images/hart.jpg");
```

文字壓在背景上

![](.gitbook/assets/image%20%2814%29.png)

