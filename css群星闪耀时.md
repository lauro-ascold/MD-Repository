## 选择器

### :empty

可以用来处理“暂无数据”

### :invalid / :valid

表示任意内容未/通过验证的 `input` 或其他 `form` 元素

### :focus-within 

表示一个元素获得焦点，或该元素的后代元素获得焦点，就会匹配上

### 优先级

元素的`class`属性中如果声明有多个`class`，那么在css文件中后声明的`class`优先级更高，而不是在元素`class`属性中后声明的优先级更高。

<!DOCTYPE html>
<html>
<head>
    <style>
        .test2 {color: green;}
        .testl {color: blue;}
    </style>
</head>
<body>
	<p class="testl test2">Hello World!</p>
</body>
</html>

这里的 Hello World!的字体颜色是蓝色，而不是绿色



## 属性



## 单位

### vmin vmax

vw&vh中的最小/大值，桌面兼容性很好甚至 safari 6 可支持，移动端受vh影响不一定准确

## 图像效果

### background-clip: text 

以文字为蒙板，实现带背景的文字效果

### mix-blend-mode:difference

元素的内容应该与元素的直系父元素的内容和元素的背景如何混合

### [CSS Painting API](https://mp.weixin.qq.com/s/ixMp0Jqc_sfNMPDrCYnPPw)

可以实现复杂如波浪的样式，性能和效果优秀，但chrome 64-、edge18-、Firefox & safari不支持

## at-rule

### [@page - CSS: Cascading Style Sheets | MDN (mozilla.org)](https://developer.mozilla.org/zh-CN/docs/Web/CSS/@page)

在打印文档时修改某些 CSS 属性，右派浏览器不支持



## [容器查询 CSS Container Queries](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Container_Queries)

chrome105+、safari16+可用，没有兼容性，[容器查询 (qq.com)](https://mp.weixin.qq.com/s/MdxqFPNNXIDtA-WQ4p2stQ)