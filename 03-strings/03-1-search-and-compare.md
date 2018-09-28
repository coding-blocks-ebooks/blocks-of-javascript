## 3.1 Search and Compare

### 3.1.1 Accessing characters

We can use 'chatAt()' to find characters in a String

```js
let str = "Awesome String"
console.log(str.charAt(2)) // e
```

Since ECMAScript 2015, we can also tread a string like a character array and
access characters using the `obj[N]` syntax like normal arrays.

```js
let str = "Awesome String"
console.log(str[2]) // e
```

### 3.1.2 Searching characters

We can search for characters and other strings inside a string using `indexOf()` method
While this only returns the first instance of the occurence, we can search for next occurence
by passing a _search from_ index in the second parameter of `indexOf()`. See example -

```js
let str = "Potato potato"
str.indexOf("o") //1
str.indexOf("to") //4
str.indexOf("to", 5) //11
str.indexOf("o", str.indexOf("o") + 1) //5
```

As seen above we can recurse on the result of `indexOf()` to get second instance too.

Javascript allows searching from the other end too, simply using `lastIndexOf()`

```js
let str = "Potato potato"
str.lastIndexOf("o") //12
str.lastIndexOf("to", 10) //4
```
