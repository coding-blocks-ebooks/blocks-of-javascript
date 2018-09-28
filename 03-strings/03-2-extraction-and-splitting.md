## 3.2 Extraction and Splitting

{% youtube src="https://www.youtube.com/watch?v=5v_A1P8cytY" %}
{% endyoutube %}

We have a lot of ways to extract sub-parts of a string or split it up.

### 3.2.1 `substr`, `substring` and  `slice`
All these methods are used to cut a part of a string out of a larger string.
Their behaviours are similar, but slightly different from each other

#### 3.2.1.1 `"string".substr(from[, length])`

```js
let str = "this be a long string"
str.substr(3) //"s be a long string"
str.substr(3,6) //"s be a"
str.substr(-4) //"ring"
str.substr(-10, 6) //"ong st"
```

The first argument gives the position from where we start, and the _optional_ second
argument tells us how many characters are in the new substring. If not provided, we go
all the way upto the end of the original string.
Additionally, as we see, it also takes negative parameters for the `from` argument.
Negative position is counted from the end of the string.

#### 3.2.1.2 `"string".substring(from[, end])`

```js
let str = "this be a long string"
str.substring(5) //"be a long string"
str.substring(5,7) //"be"
```

`substring` takes `from` and `to` as parameters, creating a sub string as per the given
positions. If the second argument is not provided, it goes all the way to the end.
_**Note that substring does not allow negative parameters**_

#### 3.2.1.3 `"string".slice(from[, to])`

```js
let str = "this be a long string"
str.slice(5) //"be a long string"
str.slice(5,9) //"be a"
str.slice(-10) //"ong string"
str.slice(-10, -5) //"ong s"
```

As the example shows, `slice` is very similar to `substring`, only differing in that
it can also accept negative values for the `from` and `to` arguments.
Negative values are counted from end of the string.

_**Note that when using both negative and positive values, the second argument must be larger
than (to the right of) the first argument**_ Javascript cannot slice, substring or substr from right
to left.

### 3.2.2 `split`ting a string

Strings have a `split()` method that takes a _regular expression_ (regexp) argument. It splits the string
into an array of strings at every occurence of the given regexp. The regexp can just be simple string,
or it can use full RegExp powers to split a string at each **'&lt;space&gt;sh' or '&lt;space&gt;s'** as shown below

```js
let str = "she sells sea shells on the sea shore"
str.split('a')
//['she sells se', 'shells on the se', 'shore']
str.split(' ')
//[she,sells,sea,shells,on,the,sea,shore]
str.split('')
//[s,h,e, ,s,e,l,l,s, ,s,e,a, ,s,h,e,l,l,s, ,o,n, ,t,h,e, ,s,e,a, ,s,h,o,r,e]
str.split(/[ sh, s]/)
//[,,e,,ell,,,ea,,,ell,,on,t,e,,ea,,,ore]
```

As seen, we can split a string with `''`, i.e. an _empty string_ which basically turns the string
into an array of its individual characters.
