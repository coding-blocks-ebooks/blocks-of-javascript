## 2.1 Basic Syntax

Javascript is _interpreted_ line by line. Each line written is read and the interpreter 'executes' the line before moving on to read the _next line_. The meaning of a **line** to the Javascript interpreter is not the same as what a line means to a text editor. A "line of code" could be more or less than a "line of text".  Lines can be optionally terminated with `;`\(semicolon\) in Javascript. 

The following, although written in one line, is technically two lines for the interpreter.

```js
var a = 10; window.alert(a);
```

Similarly the following declaration of function, although takes 3 lines, will be just a single line when the interpreter goes through it for the first time

```js
function myFun () {
    window.alert('hello')
}
```

### 2.1.1 Comments



