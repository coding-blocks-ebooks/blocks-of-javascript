# 3. Strings

{% youtube src="https://www.youtube.com/watch?v=qGQmj86A3q4" %}
{% endyoutube %}

A `string` in Javascript is, simply put, a sequence of characters. 

## 3.1 Declaring Strings

We can declare strings just like any other variables. We can use either single quote `'` or double quote `"` \(they are completely interchangable\). 

```
let aString = "this is a string"
let oString = 'this is other string'
```



## 3.2 Escape Notation

Besides normal characters we can use in a string, some characters, which are either not printable, or not 'type'able can be put into a string using `\` \(backward slash\) escape sequences.   


| Code | Output |
| :--- | :--- |
| `\0` | the NULL character |
| `\'` | single quote |
| `\"` | double quote |
| `\\` | backslash |
| `\n` | new line |
| `\r` | carriage return |
| `\v` | vertical tab |
| `\t` | tab |
| `\b` | backspace |
| `\f` | form feed |
| `\uXXXX` | unicode codepoint |
| `\u{X}` ... `\u{XXXXXX}` | unicode codepoint |
| `\xXX` | the Latin-1 character |

An example, if you want to use this as a string - `He said, "I am Iron Man"`you can declare it as follows

```
let speech = "He said, \" I am Iron Man\""
```

## 3.3 Template Strings 

{% hint style='working' %}
Note: This is something that was introduced in ECMAScript 2015, so you'd need browsers / NodeJS editions released mostly after mid-2016 for these to work.
{% endhint %}



