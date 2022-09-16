# HTML Intro

[English Version](HTML-Intro-EN.md)

HTML 是超文本标记语言(Hypertext Markup Language)的简写。它不是编程语言，而是用来构建网页内容结构的标记语言。

HTML 的作用就如同建一座没有装修的毛坯房或者只有骨架的房子。

<img src="https://cdn.pixabay.com/photo/2018/05/03/10/18/housebuilding-3370969_1280.jpg" alt="House framing">

## HTML 元素

📎HTML 文档由众多元素构成。

📎HTML 元素的内容写在开始标签和结束标签里。

以段落`<p>`元素为例,开头的`<p>`标签为开始标签，最后的`</p>`标签为结束标签，元素的内容“I am a Front-end Engineer”写在这两个标签之间。

```html
<p>I am a Front-end Engineer</p>
```

元素的开始标签内可以添加属性，属性为 HTML 提供了附加的信息，并不会显示在网页中。

以锚点标签`<a>`为例，在开始标签中添加`href`属性，该属性会在用户点击后跳转到指定的网页。

```html
<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a"
  >The Anchor element</a
>
```

## HTML 空元素

并不是所有的 HTML 元素都有结束标签。

##### 例如：

`<br>`
`<hr>`
`<input>`
`<img>`
`<meta>`
`<link>`

## HTML 基本格式

HTML 文档有标准的 html 书写规范。

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Frontend Tutorial</title>
  </head>
  <body>
    <h1>HTML</h1>
  </body>
</html>
```

#### 剖析代码：

- `<!DOCTYPE html>`定义该文档书写的是 HTML5 规范的语法
- `<html>`是根元素，包裹页面所有内容,其中`lang`属性指定元素内容的语言
- `<head>`包含 HTML 页面的元数据，不会显示在页面
- `<meta charset="UTF-8">` 设置 UTF-8 字符集
- `<title>`为页面的标题,出现在浏览器标签上
- ` <body>` HTML 页面显示的所有内容都在这个标签内
- `<h1>`是一个标题标签

## References

```

https://developer.mozilla.org/en-US/docs/Web/HTML


```
