# What are the new features of H5 ？what is WebSocket?

[中文版本](HTML-03.md)

- Geolocation （Get geolocation）

- canvas and svg drawing elements

- semantic tags such as header,footer,nav,article,section etc

- audio and video tags

- Drag and Drop API

— New form controls such as date, time, email, url, etc.

- localStorage、sessionStorage（For local offline storage）

- Multi-threaded technology web worker that can perform complex data operations without affecting the operation of the main application

- HTML5 History adds `history.pushState` and `history.replaceState`. These two APIs do not cause a page refresh when manipulating the browser history.

- Added WebSocket

WebSocket uses the ws or wss protocol.

HTTP protocol servers cannot actively push information to the client. The WebSocket API allows the server and client to push messages to each other at any time within a given time frame.

```javascript
// Create a Socket instance
var socket = new WebSocket('ws://localhost:8080')
// Open Socket
socket.onopen = function (event) {
  // Send an initialization message
  socket.send("I am the client and I'm listening!")
  // Listening to messages
  socket.onmessage = function (event) {
    console.log('Client received a message', event)
  }
  // Listening for socket closure
  socket.onclose = function (event) {
    console.log('Client notified socket has closed', event)
  }
  // Close Socket....
  //socket.close()
}
```

# References

```
https://html.spec.whatwg.org/
https://interview2.poetries.top/docs/excellent-docs/
https://www.ruanyifeng.com/blog/2017/05/websocket.html

```
