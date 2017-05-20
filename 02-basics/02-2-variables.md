## 2.2 Variables

The concept of variables is primary to most programming languages. There are hardly any high language that does not deal with variables. This is so because, variables are an important concept of algebra.

Consider the following  mathematical equations -

```math
x + y = 5;
x - y = 1;
```

Trivially we can see that **x** and **y** might be **3** and **2**, but if we had to formally solve this, we can proceed so forth.

```math
x + y = 5, and x - y = 1;
=> (x + y) + (x - y) = 5 + 1
=> 2x = 6
=> x = 3

Now using the resolved value of x,
   3 + y = 5
=> y = 2
```

During the entire process, what you possibly realised is that, what **x** really is, is a container / wrapper for the integer **3.**

In computer programming, variables work similarly.

### 2.2.1 Declaring and Using Variables

The way to declare and store data in variables, and use them is as follows -

```js
var a = 10;
var b = 11;
var c = b - a;
console.log(c); // Output: 1
```

**NOTE the usage of the operator **`=`** here. It works as 'assignment' operator in Javascript \(and most other programming langauges\). **`var a = 10`** means, in english - "**_**Let the value of a be 10**_**", and not the statement **~~**"**_**The variable a is equal to 10**_**"**~~

#### 2.2.1.1 Mutability

The mutability of a variable says whether we can change the value of a  variable once it has been declared. There are 3 variable declaration keywords - `var`, `let` and `const`

And this how `var` and `let` work.

```js
var a = 10;
a = 12; //value can be changed
let b = 20;
b = 0; // value can be changed
```

It may appear to not be any different, but `var` and `let` have different scopes \(we are soon going to cover that\).

And this is how `const` works -

```js
const k = 123;
k = 0; // Error: Because we cannot change value of const.
```



