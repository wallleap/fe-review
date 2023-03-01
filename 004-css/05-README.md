## 文本相关的样式

### 颜色

```css
el {
	color: pink;
}
```

[color - CSS：层叠样式表 | MDN (mozilla.org)](https://developer.mozilla.org/zh-CN/docs/Web/CSS/color)

- 色值表示
	- 单词：red、blue、green……
	- 十六进制（hex）：`#ff00ff`、`#f0f`、`#aabbccaa`（十六进制也支持透明色了）
	- 函数：`rgb(255,255,255)`、`rgba(0,0,0,0.2)`（rgb 其实第四个参数也能设置透明度）、`hsl(30, 100%, 50%)`、`hsla(30, 100%, 50%, 0.6)`
	- 关键字：`currentColor`（当前文字继承颜色 一般设置 bg 和 border 色）、`transparent`（完全透明）

### 设置字号大小

```css
el {
	font-size: 16px;
}
```

- Chrome 允许展示的最小字号为 `12px`（0 不算），默认的字号为 `16px`
- 常见单位：
	- `1px` 1 像素，和屏幕分辨率有关
	- `1em` 是自己 `font-size` 的 1 倍（自己没有设置那就是继承来的字号）
	- `1rem` html 根元素 `font-size` 的 1 倍
	- `1vw` 窗口（视窗）宽度的 1%
	- `1vh` 窗口高度的 1%

### 字体

```css
body {
	font-family: -apple-system, "Noto Sans", "Helvetica Neue", Helvetica, "Nimbus Sans L", Arial, "Liberation Sans", "PingFang SC", "Hiragino Sans GB", "Noto Sans CJK SC", "Source Han Sans SC", "Source Han Sans CN", "Microsoft YaHei", "Wenquanyi Micro Hei", "WenQuanYi Zen Hei", "ST Heiti", SimHei, "WenQuanYi Zen Hei Sharp", sans-serif;
}
```

- 先找第一个字体库，找不到再第二个，一次往后……
- 如果都没有就用系统默认的
- 字体里包含空白字符、数字、其他特殊字符最好加引号
- 如果字体是中文名，最好转成 Unicode 写上去

```css
/* 设置自定义字体 */
@font-face {
	font-family: "misans";
	src: url("url");
}
body {
	font-family: misans, "Noto Sans";
}
```

### 斜体

```css
el {
	font-style: italic;
	font-style: normal;
}
```

### 粗细

```css
el {
	font-weight: bold;
	font-weight: 900;
	font-weight: 400;
	font-weight: 100;
	font-weight: normal;
}
```

需要看字体里有没有这种字重，没有的话会往最接近的靠

### 对齐

设置块元素里面的内联元素对齐方式

```css
p {
	text-align: left;
	text-align: center;
	text-align: right;
	text-align: justify;
}
```

### 文字划线

```css
el {
	text-decoration: none;
	text-decoration: underline;
	text-decoration: line-through;
	text-decoration: overline;
	text-decoration: blue wavy underline;
}
```

### 单行文本超出省略号

```css
h2 {
	white-space: nowrap; /* 超出不折行 */
	overflow: hidden; /* 超出隐藏 */
	text-overflow: ellipsis; /* 文本溢出省略号 */
}
```

### 多行文本超出省略号

```css
p {
	overflow: hidden;
	display: -webkit-box;
	-webkit-line-clamp: 2;
	-webkit-box-orient: vertical;
}
```

### 行高

```css
p {
	line-height: 1.5;
}
```

`line-height` 决定一行文字占据的真实高度

- `line-height: 1.5;` 当前元素 `font-size` 的 1.5 倍，后代都是继承 `1.5`
- `line-height: 20px;` 固定行高
- `line-height: 150%;` 当前元素 `font-size` 的 1.5 倍，先计算出具体的值，然后后代继承的是计算出的固定值

### 文字首行缩进

```css
p {
	font-size: 2em;
	text-indent: 2em;
}
```
