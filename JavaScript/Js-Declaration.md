# 使用 let、var 和 const 创建变量的区别

# 📌 作用域

作用域指变量的有效范围。

使用 `var`声明的变量，其作用域为函数作用域。

使用 let 声明变量和 const 声明常量时，其作用域为块级作用域。

```javascript

```

# 📌 变量提升

使用 `var`声明的变量，存在变量提升的情况，可以先声明再使用。

```javascript
console.log(num)
var num = 20

变量提升过程：
var num
console.log(num)
num = 20

返回结果为 // undefined
```

使用 let 声明变量和 const 声明常量时，不存在变量提升，不能在声明之前使用。

```javascript

```

# 📌 更改变量

使用 `var` 可以多次声明一个变量，
