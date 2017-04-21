## 1.1 Running Javascript

There are two ways we can try Javascript. Either using a Javascript REPL \(REPL stands for read-eval-print loop, which means a 'shell' or 'console' like interface where you can write code line by line, and the interpreter interprets each line before you move to the next\), or by writing a .js script file, and running it.

### 1.1.1 In a browser

Originally, Javascript was a browser-only language. And all web browsers support executing Javascript. You have two options -

#### REPL

Open the _console_ of your browser. The shortcut would be the following - 

| Browser | Windows / Linux | Mac OS |
| :--- | :--- | :--- |
| Firefox | Ctrl + Shift + K | Cmd + Shift + K |
| Chrome | Ctrl + Shift + J | Cmd + Opt + J |

#### Running a script

In a folder save two files - `index.html` and `script.js`

In the `index.html` file, write the following code - 

```html
<html>
<head>
<script src="script.js"></script>
</head>
</html>
```

Then write your Javascript code in the `script.js` file, and then open the `index.html`   file in a browser. Open the Web console if you want to see the output of your code. 

### 1.1.2 Without a browser \(NodeJS\)

We can also use [Node.JS](http://nodejs.org) to run Javascript directly on a computer without having to use a Browser. Once Nodejs is installed we can do one of the following

#### REPL 

Just enter the following command in your terminal 

```shell
node
```

And that would bring to you the NodeJS REPL.

#### Running a script

Running a script with Nodejs is straight forward. Save your Javascript code in a `script.js` file, and then, from the same folder, in a terminal run - 

```shell
node server.js
```



