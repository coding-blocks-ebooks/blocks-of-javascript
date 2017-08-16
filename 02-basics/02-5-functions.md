## 2.5 Functions

Functions are a very important part of programming languages to run. Functions in programming languages are based on the core concept of functions in mathematics. A function is an operation that takes certain values \(referred to as arguments\) as input, and returns a single value as an output.

$$k = f(x,y)$$

In the above statement, _**k**_ is the returned value, from the function _**f**_ that takes _**x  **and _**y  **as arguments. We could have had defined `f(x,y)` as follows -

$$f(x,y) = x^2 + y^2$$

This would imply that for values 3 and 4 of **x **and **y** respectively, **k ** would be 25.

A similar result can be achieved in Javascript using the following syntax: 

```js
function f (x,y) {
    return x*x + y*y
}

var k = f(3,4)

console.log(k) // 25
```

The syntax to define a function is like this `function funName (arg1, arg2) { /* body */ }`  

### 2.5.1 Function return types

In many languages, functions must have a strictly defined return type. Since Javascript is loosely typed, and we cannot enforce types on variables, thus functions do not have a return type. Which leads us to write code like this - 

```js
function add (a, b) {
    return a + b
}

var p = add(1,2)
var q = add('hello', 'world')

console.log(p) // 3
console.log(q) // "helloworld")
```



