# H5 新特性有哪些？webSocket 是什么？

[English Version](HTML-03-EN.md)

- Geolocation (获取地理位置)

- canvas 和 svg 绘图元素

- 语义化标签，如 header,footer,nav,article,section 等

- 音频（audio）和视频（video）标签

- 拖拽 API

- 新表单控件，比如 date、time、email、url 等

- localStorage、sessionStorage(本地离线存储)

- 多线程技术 web worker ，可执行复杂的数据操作，不影响主程序的运行。

- HTML5 History 新增了`history.pushState`和 `history.replaceState`。这两个 API 在操作浏览器历史记录时，不会引起页面刷新。

- 新增了即时通讯 WebSocket

WebSocket 使用 ws 或 wss 协议，服务器网址就是 URL。

HTTP 协议服务器不能主动向客户端推送信息。而 WebSocket API 允许服务器和客户端在给定的时间范围内的任意时刻，相互推送信息。

```javascript
// 创建一个Socket实例
var socket = new WebSocket('ws://localhost:8080')
// 打开Socket
socket.onopen = function (event) {
  // 发送一个初始化消息
  socket.send("I am the client and I'm listening!")
  // 监听消息
  socket.onmessage = function (event) {
    console.log('Client received a message', event)
  }
  // 监听Socket的关闭
  socket.onclose = function (event) {
    console.log('Client notified socket has closed', event)
  }
  // 关闭Socket....
  //socket.close()
}
```

# References

```
https://html.spec.whatwg.org/
https://interview2.poetries.top/docs/excellent-docs/
https://www.ruanyifeng.com/blog/2017/05/websocket.html

```
