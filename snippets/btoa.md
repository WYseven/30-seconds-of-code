### btoa

Creates a base-64 encoded ASCII string from a String object in which each character in the string is treated as a byte of binary data.

Create a `Buffer` for the given string with binary encoding and use `Buffer.toString('base64')` to return the encoded string.


创建 `base-64` 编码的 `ASCII` 字符串，其中字符串中的每个字符都被视为二进制数据的字节。

使用二进制编码为给定字符串创建 `Buffer`，并使用 `Buffer.toString（'base64'）` 返回编码字符串。

```js
const btoa = str => Buffer.from(str, 'binary').toString('base64');
```

```js
btoa('foobar'); // 'Zm9vYmFy'
```
