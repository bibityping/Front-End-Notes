# cookies、sessionStorage 和 localStorage 的区别

[English Version](HTML-04-EN.md)

webStorage（localStorage，sessionStorage）是 HTML5 提出来的本地储存功能。

## 相同点

`cookies`,`localStorage`, `sessionStorage`

- 客户端保存数据的解决方案

- 以字符串类型的键值对形式保存数据

## 不同点

- 存储大小：`cookies` 数据大小限制在 4KB；`localStorage` 为 5/10MB；`sessionStorage`为 10MB。

- 随请求发送：`cookies` 的数据每次都会发给服务器端， `localStorage` 和 `sessionStorage` 不和服务端通信。

- 储存位置：`cookies` 存储在浏览器和服务端。`localStorage` 和 `sessionStorage` 只存储在浏览器。

- 访问权限：`cookie` 和 `localStorage` 可访问任意窗口，`sessionStorage` 只能访问当前页面窗口。

- 过期时间：`cookies` 的数据过期时间取决于手动设置的过期日期。`sessionStorage` 的数据储存在当前浏览器关闭后自动删除。`localStorage` 的数据永远不会过期，除非手动删除。

- 浏览器兼容：`cookies` 支持 HTML4，兼容老浏览器、`localStorage` 和`sessionStorage` 支持 HTML5，有些较老的浏览器不支持。

## References

```
https://stackoverflow.com/questions/19867599/what-is-the-difference-between-localstorage-sessionstorage-session-and-cookies
https://www.frontendinterviewhandbook.com/html-questions
https://youtu.be/AwicscsvGLg
https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API
```
