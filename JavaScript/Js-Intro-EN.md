# JavaScript Intro

[中文版本](Js-Intro.md)

The three main technologies of Web front-end, HTML to build content structure, CSS to beautify the style, and JavaScript to realize the dynamic interactive functions of web pages.

JavaScript is a dynamically typed, weakly typed programming language that runs on the client side.

#### Characteristics of weakly typed languages：

- No need to specify data types in advance before declaring variables
- Different types of data can be stored in the same variable
- Implicit conversion is possible

Because of the characteristics of JavaScript, it can only be used to manipulate the DOM, so JavaScript is a single-threaded language that can only do one thing at a time.

JavaScript can now do server-side programming in addition to running in the browser.

## Composition of JavaScript

To learn JavaScript, start with two things：

- ECMAScript (the basic syntax of JS)
- The Web API contains BOM (Browser Object Model) and DOM (Document Object Model)

## JavaScript writing position

### 1.Internal Script

JavaScript is written in the `<script>` tag and can be inserted anywhere in the html document.

However, browsers load HTML in document order, so it is recommended that the JavaScript code be placed after the HTML and written above `</body>`.

#### For example：

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

### 2.External Scripts

和 css 的外部文件引入方法一样，建一个.js 的文件，将 JavaScript 代码全部放在这个文件里。

HTML 文件里需要添加下面这个标签,引入外部的 JS 脚本。

```javascript
<script src="path/to/script.js"></script>
```

### 3.Inline JavaScript

Write the code inside the tag as shown in the code below：

```javascript
<button onclick="alert('Download successfully')">Click me<button>
```

This is not used in JS development.

## JavaScript Input and Output Syntax

### Output syntax

- `document.write('Hi');` Output content on the page
- `alert('Hello');` The page pops up with an alert box
- `console.log('test');` Console output syntax, used by programmers to debug code

### Input syntax

- `prompt('What's your name?');` Display a dialog box that prompts the user for input

## References

```
http://www.ruanyifeng.com/blog/2014/10/event-loop.html
https://developer.mozilla.org/en-US/docs/Web/JavaScript/JavaScript_technologies_overview
https://www.bilibili.com/video/BV14T4y1a734/?vd_source=00066457aeb1710db6c2235669c69209
https://www.bilibili.com/video/BV1Kq4y1e7d2?p=2&spm_id_from=pageDriver&vd_source=00066457aeb1710db6c2235669c69209
https://javascript.info/hello-world
```
