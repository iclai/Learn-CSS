---
description: 背景圖片大小設定
---

# background-size背景圖片大小

#### 指定背景圖片大小

```css
background-size: auto | length | percentage | cover | contain
```

* **auto** 為預設值，就是背景圖片原始長寬。
* **length** 指定圖片具體大小長寬的數值，**不允許負值**。
* **percentage** 以背景圖元素的百分比指定背景圖大小，**不允許負值**。
* **cover** 主要用於背景圖小於所在的容器，而背景圖又不適合使用 **repeat**，此時就可以採用 **cover** 的方式，使背景圖放大至容器的大小，但此方法容易使背景圖因放大而失真。
* **contain** 與 **cover** 正好相反，主要用於背景圖大於所在容器，但卻需要將背景圖完整呈現，此時就可採用 **contain** 的方式，使背景圖縮小至容器的大小。

![](../.gitbook/assets/b03.jpg)

