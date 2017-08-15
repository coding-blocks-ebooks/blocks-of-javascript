## 2.3 Datatypes

Computers store data in binary format - i.e. `0`s and `1`s.  
That is grouped into bytes.

Humans on the other hand, do not understand bytes or binary directly. We  
understand numbers like 1, 20, 42 \(which are whole numbers\), or 23.4, 10/4,  
\(which are decimals or fractions\). We understand letters of the alphabet like  
`A` or `g`, and words formed by these alphabets like `nyan` and `cat`.

Fortunately, most programming platforms, allow us to use datatypes more human-readable  
than plain bits and bytes.

Some common data formats computer programming languages support are -

| Data type | Description | Examples |
| --- | :--- | ---: |
| integer | whole numbers | -1, 0, 15 |
| float | decimal numbers or rational  fractions | -2.5, 0.1, 22.3334 |
| character | a single literal. could be a letter  or a number or a symbol | 'a', 'B', '4', '/' |
| string | a sequence of characters | 'word', 'o em gee' |
| boolean | a 2-value data that can be  truthy or falsy | true, false |
| array | an iterative sequence.  each item of an array could be any  of the above data types | \[1,2,3\], \['a', 'e', 'i'\] |

### 2.3.2 Datatypes in Javascript

In Javascript we have following datatypes -

| Data Type | Description | Examples |
| :--- | :--- | :--- |
| **number** | Any numerical value. Does not distinguish between whole numbers and fractions | 1, 43.22, -0.5 |
| **string** | Any array of characters, \(JS by default supports UTF-8 charset, so all characters of a string must in UTF-8\). There is no _character_ datatype, so single characters are also strings | "hello", "a", "wow !", "this is str 2" |
| **boolean** | A value which is either _**true**_ or _**false**_ | true, false |
| **undefined** | A special datatype in Javascript for 'undefined' data. An undefined type basically means there is no data in it. It is similar \(but not exactly same\) to 'void' datatype in C-like programming languages | undefined |
| **function** | In Javascript functions themselves are first-class objects. So a function is also a variable. The type of such variables which are functions is _**function**_ | function a \(\) {return "a"} |
| **object** | Pretty much everything that can be classified into any of the above datatypes, is an object. All types extend from the _object_ type in Javascript. Arrays and _null_ are also of the type object | {a: 10, b:20},   \[1,3,4\] |

### 2.3.3 Finding Datatype of object in Javscript

We can find the data type of an object in Javascript using the  `typeof` operator. 

```js
var a = 10, 
    b = 'str', 
    c = [3,4,1], 
    d = {P:1, Q:2}, 
    e = null, 
    f = false,
    g = function () { return 0} ;

console.log(typeof a) // "number"
console.log(typeof b) // "string"
console.log(typeof c) // "object"
console.log(typeof d) // "object"
console.log(typeof e) // "object"
console.log(typeof f) // "boolean"
console.log(typeof g) // "function"
console.log(typeof undefined) // "undefined"


```



