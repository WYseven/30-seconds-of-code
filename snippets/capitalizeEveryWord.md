### capitalizeEveryWord

Capitalizes the first letter of every word in a string.

Use `String.prototype.replace()` to match the first character of each word and `String.prototype.toUpperCase()` to capitalize it.

将字符串中每个单词的第一个字母大写。

使用 `String.prototype.replace()` 匹配每个单词的第一个字符，并使用 `String.prototype.toUpperCase()` 将其大写。


```js
const capitalizeEveryWord = str => str.replace(/\b[a-z]/g, char => char.toUpperCase());
```

```js
capitalizeEveryWord('hello world!'); // 'Hello World!'
```
