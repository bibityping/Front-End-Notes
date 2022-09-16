# JavaScript Intro

[English Version](Js-Intro-EN.md)

Web 前端三大技术，HTML 构建网页内容结构，CSS 美化网页样式，JavaScript 用来实现网页的动态交互功能。

JavaScript 是一种运行在客户端的动态型（dynamic typed)，弱类型（weakly typed）的编程语言。

#### 弱类型语言特点：

- 声明变量前，无需提前指定数据类型
- 同一个变量可保存不同类型的数据
- 可进行隐式转换

JavaScript 是一种解释型语言，不需要预编译，浏览器直接解释执行。

由于 JavaScript 的特性，它只能用来操作 DOM，所以 JavaScript 是单线程的语言，同一个时间只能做一件事。

JavaScript 除了运行在浏览器中，现在还可以做服务端编程。

## JavaScript 的组成

要学习 JavaScript，要从以下两个方面入手：

- ECMAScript(JS 的基础语法)
- Web API 里包含 BOM(浏览器对象模型）和 DOM（文档对象模型）

## JS 的书写位置

### 1.内部脚本

JavaScript 写在 `<script>` 标签里，可插入到 html 文档的任意位置。

但浏览器会按照文档顺序加载 HTML，建议 JavaScript 代码放在 HTML 之后，写在`</body>`上面。

##### 例如：

```javascript
<!DOCTYPE HTML>
<html>

<body>
  <p>lalala</p>
  <script>
    alert('Hello, JS!');
  </script>
</body>

</html>
```

### 2.外部脚本

和 css 的外部文件引入方法一样，建一个.js 的文件，将 JavaScript 代码全部放在这个文件里。

HTML 文件里需要添加下面这个标签,引入外部的 JS 脚本。

```javascript
<script src="path/to/script.js"></script>
```

### 3.内联 JavaScript

如下代码所示，将代码写在标签内。

```javascript
<button onclick="alert('Download successfully')">Click me<button>
```

在 JS 开发中这种方式不会使用。

## JavaScrip 输入输出语法

### 输出语法

- `document.write('Hi');` 在页面输出内容
- `alert('Hello');` 页面弹出警示框
- `console.log('test');` 控制台输出语法，程序员用来调试的

### 输入语法

- `prompt('What's your name?');` 显示一个对话框，提示用户输入内容

## References

```
http://www.ruanyifeng.com/blog/2014/10/event-loop.html
https://developer.mozilla.org/en-US/docs/Web/JavaScript/JavaScript_technologies_overview
https://www.bilibili.com/video/BV14T4y1a734/?vd_source=00066457aeb1710db6c2235669c69209
https://www.bilibili.com/video/BV1Kq4y1e7d2?p=2&spm_id_from=pageDriver&vd_source=00066457aeb1710db6c2235669c69209
https://javascript.info/hello-world
```
