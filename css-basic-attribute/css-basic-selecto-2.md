# CSS基本選擇器\(二\)

### Attribute selectors（屬性選擇器）

屬性選擇器優點是不需要額外替這些網頁元素設定ID或是Class就可以選擇設定它。

 CSS Attribute Selectors 語法有：

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
/**屬性值錢面加了一個~符號，表示要選擇的是網頁中圖片有 title 屬性，而且屬性值
必須是有空格分開的字串，其中還必須有一個是 photo1，這樣才會被選取**/
img[title~="photo1"] {
border: 1px gray solid;
}
```

```markup
<img src="圖片" title="photo1 good">
<img src="圖片" title="photo2 good">
```

 **\[attribute\|=value\]**

```css
/**表示只會選擇 span 元素中有 title 屬性，且 title 屬性值中必須包含至少一個
T1 或 T1 後連接著一個水平橫線符號（-），所以範例的第一個 span 與第二個 span 
都會被選取，第三個 span 則不會被選取。**/
span[title|="T1"] {
color:blue;
}
```

```markup
<span title="T1">這段文字將會變成藍色的</span><br>
<span title="T1-22">這段文字將會變成藍色的</span><br>
<span title="T2">這段文字將維持原本的黑色</span>
```

 **\[attribute^=value\]**

```css
/**只會選擇 title 屬性值中的字串開頭包含有 T1 的 span 元素，無論 T1 後還有沒有
其它的字符都會被選取，但如果不包含 T1 或 T1 不在字串的開頭都不會被選取。**/
span[title^="T1"] {
color:red;
}
```

```markup
<span title="T1">這段文字將會變成紅色的</span><br>
<span title="T12">這段文字將會變成紅色的</span><br>
<span title="T2">這段文字將會維持原本的黑色</span>
```

 **\[attribute$=value\]**

```css
/**選擇 title 屬性值中的字串尾含有 T1 的 span 元素，例如第一個 span 與第二個
 span 的 title 屬性值字尾都有 T1，所以會被選取，而第三個 span 的 title 屬性值
 字尾並沒有 T1，所以不會被選取。**/
span[title$="T1"] {
color:green;
}
```

```markup
<span title="ABC-T1">這段文字將會變成綠色的</span><br>
<span title="DEF-T1">這段文字將會變成綠色的</span><br>
<span title="DEF-T2">這段文字將會維持原本的黑色</span>
```

 **\[attribute\*=value\]**

```css
/**選擇 title 屬性值中含有 T1 字符的 span 元素，無論 T1 在 title 屬性值中的
哪個部份，所以範例中的第一個 span 與第二個 span 都會被選取，而第三個 span 的 
title 屬性值不包含 T1，所以不會被選取。**/
span[title$="T1"] {
color:orange;
}
```

```markup
<span title="ABC-T1-23">這段文字會變成橘色的</span><br>
<span title="DEF-T122">這段文字會變成橘色的</span><br>
<span title="DEF-T2">這段文字會維持原本的黑色</span>
```

