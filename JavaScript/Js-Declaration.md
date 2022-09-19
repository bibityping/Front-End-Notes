# 使用 `let`、`var` 和 `const` 创建变量的区别

### 📌 作用域

作用域指变量的有效范围。

使用 `var` 声明的变量，其作用域为函数作用域。

```javascript
{
  var foo = 10
}
console.log(foo) // 10
```

使用 `let` 声明变量和 `const` 声明常量时，其作用域为块级作用域。

```javascript
{
  let abc = 10
}
console.log(abc) // Uncaught ReferenceError: abc is not defined

{
  const abc = 10
}
console.log(abc) // Uncaught ReferenceError: abc is not defined
```

### 📌 变量提升

使用 `var` 声明的变量，存在变量提升的情况，可以先声明再使用。

```javascript
console.log(num)
var num = 20

变量提升过程：
var num
console.log(num)
num = 20

返回结果为 // undefined
```

使用 `let` 声明变量和 `const` 声明常量时，不存在变量提升，不能在声明之前使用。

```javascript
console.log(javascript)

let baz = 'javascript'
// Uncaught ReferenceError: javascript is not defined

console.log(foo)

const bar = 'foo'
// Uncaught ReferenceError: foo is not defined
```

### 📌 重复声明和修改变量

使用 `var` 可以重复声明同一个变量，也可以更新变量的值。

```javascript
var foo = 'foo'
var foo = 'bar'
console.log(foo) // "bar"

var foo = 20
foo = 40
console.log(a) // 40
```

`let`在相同作用域内不可以重复声明，但 `let` 可以更新变量的值。

```javascript
let baz = 'baz'
let baz = 'qux'
console.log(baz) // Uncaught SyntaxError: Identifier 'baz' has already been declared

let foo = 20
foo = 30
console.log(b) // 30
```

`const` 不允许重复声明，其声明的常量的值不可改变。

```javascript
const foo = 20
const foo = 30
console.log(foo) // Identifier 'foo' has already been declared

const baz = 10
baz = 20
console.log(baz) //Uncaught TypeError: Assignment to constant variable.
```

References

```text
https://javascript.info/var
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const
https://es6.ruanyifeng.com/#docs/let
https://www.frontendinterviewhandbook.com/javascript-questions#what-are-the-differences-between-variables-created-using-let-var-or-const
```
