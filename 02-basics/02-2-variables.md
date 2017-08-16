## 2.2 Variables

The concept of variables is primary to most programming languages. There are hardly any high language that does not deal with variables. This is so because, variables are an important concept of algebra.

Consider the following  mathematical equations - 

$$
x + y = 5
$$

$$
x - y = 1
$$

Trivially we can see that **x** and **y** might be **3** and **2**, but if we had to formally solve this, we can proceed so forth.

$$
\begin{aligned}
x + y = 5; &\ x - y = 1 \\
&=> (x + y) + (x - y) = 5 + 1 \\
&=> 2x = 6 \\
&=> x = 3
\end{aligned}
$$

```
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
{% hint style='working' %}
NOTE the usage of the operator **`=`** here. It works as 'assignment' operator in Javascript \(and most other programming langauges\). **`var a = 10`** means, in english - _**"Let the value of a be 10"**_, and not the statement ~~"The variable a is equal to 10"~~
{% endhint %}

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

### 2.2.2 References

When we create a variable, we have a LHS (Left Hand Side) and a RHS (Right Hand Side). The LHS is the _name of the variable_, and the RHS is the _data contained in the variable_. (In computer science, those are technically called l-value and r-value in fact).
Whenever we write something like `myVar = 10`, we are reassigning the LHS to point to a new RHS.

In Javascript the assignment statements are **value-copy** and not **reference-copy** type.   

```js
var a = 10;
var b = a;
b++;
console.log(b); // 11
console.log(a); // 10 (not 11)
```

In line no. 2 in the snippet above, `b = a`, here's what happens : -
 - Interpreter looks at RHS. Finds `a`
 - Interpreter finds out the _value of `a`_ (i.e. 10)
 - Interpreter assigns this **value** to the LHS, which is `b`
 - Now `b` contains the value `10`, and `a` contains the value `10`
 - At this point, after execution of this line, there is no relationship between b and a anymore.

{% hint style='danger' %}
This behaviour holds true only for variables that have data like `number`, `string` or `boolean`. For other data types like objects and arrays, assignments are reference-copy, and not value-copy. We will see this later
{% endhint %}
