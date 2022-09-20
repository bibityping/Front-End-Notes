# What are the differences between variables created using let, var or const?

[中文版本](Js-Declaration.md)

## 📌 Scope

The scope refers to the valid range of the variable.

The scope of a variable declared with `var` is function scope.

```javascript
{
  var foo = 10
}
console.log(foo) // 10
```

When declaring variables with `let` and constants with `const`, the scope is block scoping.

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

## 📌 Hoisting

Variables declared with `var` have hoisting, and can be declared before they are used.

```javascript
console.log(num)
var num = 20

// Hoisting process:

var num
console.log(num)
num = 20

The return result is // undefined
```

When using `let` to declare variables and `const` to declare constants, there is no hoisting and cannot be used before the declaration.

```javascript
console.log(javascript)

let baz = 'javascript'
// Uncaught ReferenceError: javascript is not defined

console.log(foo)

const bar = 'foo'
// Uncaught ReferenceError: foo is not defined
```

## 📌 Re-declared and Updated

Use `var` to declare the same variable repeatedly and can update the value of the variable.

```javascript
var foo = 'foo'
var foo = 'bar'
console.log(foo) // "bar"

var foo = 20
foo = 40
console.log(a) // 40
```

`let` cannot be declared repeatedly in the same scope, but `let` can update the value of a variable.

```javascript
let baz = 'baz'
let baz = 'qux'
console.log(baz) // Uncaught SyntaxError: Identifier 'baz' has already been declared

let foo = 20
foo = 30
console.log(b) // 30
```

`const` is not allowed to be re-declared, and the value of its declared constant cannot be changed.

```javascript
const foo = 20
const foo = 30
console.log(foo) // Identifier 'foo' has already been declared

const baz = 10
baz = 20
console.log(baz) //Uncaught TypeError: Assignment to constant variable.
```

## References

```text
https://javascript.info/var
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const
https://es6.ruanyifeng.com/#docs/let
https://www.frontendinterviewhandbook.com/javascript-questions#what-are-the-differences-between-variables-created-using-let-var-or-const
```
