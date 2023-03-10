# 初学 web

## 搜索技巧

- 使用 Google 或者 Bing
- web 相关知识可以搜索**关键词 mdn**

## 如何提问

1. 期望是什么，现在是怎样
2. 提供完整代码、截图、报错

> 可以按照这个文档进行提问：[如何提问](https://www.yuque.com/jrg-share/peo6xt/sow9s3)

## 如何写笔记/博客

- 笔记写重点：例如上面的 mdn、提问的链接
- 笔记也可以使用思维导图记下关键点
- 写博客是写给别人看的，需要自己先理解，不懂的会先去查资料
- 在哪写：语雀、掘金、知乎、CSDN 等
- 如何写：遵循文章基本格式（标题、段落、列表、代码）

## Markdown 写文章

常用语法：

````markdown
# 标题（一个井号是一级标题，依次可以增加到六个井号）注意空格
## 这是二级标题，六级标题重要性依次降低
常规段落直接书写，可以在后面打两个空格或者回车形成新段落
![图片描述](图片链接)
[链接文字](链接地址)
> 引用文字在尖括号后面
> 可以有多行、多段
- 无序列表
- 无序列表
- 无序列表
1. 有序列表
2. 有序列表
3. 有序列表
段落文字之中可以有 `div` 代码、**加粗**、*倾斜*、***加粗且倾斜***等等
分割线可以是三个短横线、星号、加号：
---
代码块：
```语言
代码片段
```
````

> 表格建议直接复制，不要自己打

## 学习教程

- 现代 JavaScript 教程（https://zh.javascript.com）
- 阮一峰 JavaScript 教程（https://javascript.ruanyifeng.com）
- 阮一峰 ES6 教程（https://es6.ruanyifeng.com）
- JavaScript 秘密花园
- MDN CSS 官方教程
- 饥人谷 wiki（https://wiki.jirengu.com）
- 饥人谷前端学习指南知乎专栏

## 环境搭建

### 浏览器

- Chrome
- **Edge**
- Firefox

## 编辑器

- **[VS Code](https://code.visualstudio.com)**
	- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) 插件
	- [Live Preview](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server) 插件
	- 其他插件需要用的时候再进行安装

## HTML 标签

### 重要块级标签

- `<div>`
- `<h1>` ~ `<h6>`
- `<p>`
- `<header>`
- `<main>`
- `<aside>`
- `<article>`
- `<section>`
- `<nav>`
- `<footer>`

### 重要行级标签

- 链接：`<a href="https://qq.com">QQ</a>`
- 图片：`<img alt="描述" src="">`
- span：`<span></span>`

### 块与行

- 块级元素会独占一行
- 行级元素只占自身空间

## 页面分块

合理分块有助于写 HTML 结构

## Emmet 语法

可以加快编写代码的速度，只输入几个字母和符号按 <kbd>Tab</kbd>

- `div.class`
- `div#id`
- `div>ul>li`
- `ul>li*3`
- `ul>li*3>{$}`
- `header+main+footer`

文档：<https://docs.emmet.io>

代码嵌套建议缩进两个空格
