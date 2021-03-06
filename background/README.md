---
description: 常用的網頁背景(Background)設定寫法
---

# 背景設定

background背景如果將CSS下在&lt;body&gt;上，預設會主動填滿背景，如是使用照片做背景也會不斷重複直到填滿背景，除非有下 `no-repeat` 圖片就不會重複填滿。

### 填滿背景色

![](../.gitbook/assets/image%20%2823%29.png)

```css
background-color: orange;
```

### 填滿漸層色

![](../.gitbook/assets/image%20%2811%29.png)

```css
background: radial-gradient(yellow, red);
```

### **background-repeat** 背景圖是否要重複

* repeat 背景圖在水平與垂直重複 \(此為預設值\)。
* repeat-x 背景圖只在水平重複。
* repeat-y 背景圖只在垂直重複。
* no-repeat 背景圖不重複，只排列一次。

### 圖片當背景

![](../.gitbook/assets/image%20%2837%29.png)

```css
 background: url("../images/superwoman.jpg") no-repeat;
```

### 填滿圖片背景

![](../.gitbook/assets/image%20%2836%29.png)

```css
background-image: url("../images/hart.jpg");
```

### 文字壓在背景上

![](../.gitbook/assets/image%20%2822%29.png)

## 使整張圖片不重複

![](../.gitbook/assets/b01.jpg)

背景從手機畫面呈現，會維持原始比例。

![](../.gitbook/assets/image%20%2840%29.png)

###  [imgur 線上免費圖床](https://imgur.com/)

 imgur 是一個老牌的圖片上傳空間，imgur 沒有空間限制，不註冊也可以使用。

imgur 支援 JPEG, PNG, GIF, APNG, TIFF, BMP, PDF, XCF \(GIMP\) 等圖片格式，TIFF, BMP, PDF 和 XCF \(GIMP\) 會自動被轉為 PNG 上傳。圖片大小限制為 10 MB。

但是圖片在 6 個月內都沒有任何人檢視，就會自動從系統中移除。

![](../.gitbook/assets/image%20%2826%29.png)

