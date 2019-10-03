# 漸層背景

### Linear 線性漸層

![](../.gitbook/assets/image%20%286%29.png)

### Radial 放射狀漸層

![](../.gitbook/assets/image%20%282%29.png)

若漸層是設在背景，要加入`background-attachment: fixed;` 語法，讓漸層背景延伸固定

### 漸層背景屬性

background: linear-gradient\(顏色漸變方向&lt;開始方向    結束方向&gt;, 色碼1 位置1,色碼2 位置2,....\)

* 顏色漸變方向，預設值為由上而下   **`linear-gradient(yellow,red);`**
* 由左而右的線性漸層效果   **`background: linear-gradient(to right,yellow,red);`**
* 對角線的線性漸層效果（由左下向右上） **`background: linear-gradient(to bottom right,yellow,red);`**
* 角度調整的線性漸層效果  **`background: linear-gradient(90deg,yellow,red);`**

### 線上漸層工具

### [Css Gradient](https://cssgradient.io)

![](../.gitbook/assets/image%20%2822%29.png)

