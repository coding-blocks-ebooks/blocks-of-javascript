## 2.4 Equality

Like other programming languages, Javascript supports a simple and easy way to check if two variables contain the same data.  
We use the `==` operator to check if the LHS and the RHS are equal to each other. The output of the equality check is either `true`  or `false`  

```js
var a = 10;
var x = 10;
console.log(a == x) // true
var p = 20;
console.log(p == x) // false
```

### 2.4.1 Strict and non-strict equality

Javascript can check for equality using `==` as well as `===` operator. The difference between the two is that the double-equals operator does a non-strict equality check. If the LHS or the RHS, can be cast to a different data type that is equal to the other side, the `==` operator would still return true. Whereas, the `===` operator will check for the LHS and the RHS to be of the _same datatype_ **and **having _the same value._

```js
10 == '10'  // true
10 === '10' // false 
```



