# The difference between cookies, sessionStorage and localStorage

[中文版本](HTML-04.md)

webStorage (localStorage, sessionStorage) is a local storage feature introduced by HTML5.

## Similarities

`cookies`,`localStorage`, `sessionStorage`

- Client-side solution for saving data

- Save data as a key-value pair of string type

## Differences

- Storage size: `cookies` data size is limited to 4KB; `localStorage` is 5MB/10MB `sessionStorage` is 5MB.

- Sent with request: `cookies` data is sent to the server side every time, `localStorage` and `sessionStorage` do not communicate with the server side.

- Storage location: `cookies` are stored on the browser and server side. `localStorage` and `sessionStorage` are stored in the browser only.

- Access rights: `cookie` and `localStorage` can access any window, `sessionStorage` can only access the current page window.

- Expiration time: The data expiration time of `cookies` depends on the manually set expiration date. The data stored in `sessionStorage` is automatically deleted when the current browser is closed. The data in `localStorage` never expires, unless it is manually deleted.

- Browser compatibility: `cookies` supports HTML4, which is compatible with older browsers. `localStorage` and `sessionStorage` support HTML5, some older browsers do not support them.

## References

```
https://stackoverflow.com/questions/19867599/what-is-the-difference-between-localstorage-sessionstorage-session-and-cookies
https://www.frontendinterviewhandbook.com/html-questions
https://youtu.be/AwicscsvGLg
https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API
```
