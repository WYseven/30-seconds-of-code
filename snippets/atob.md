### atob

------------

Decodes a string of data which has been encoded using base-64 encoding.

Create a `Buffer` for the given string with base-64 encoding and use `Buffer.toString('binary')` to return the decoded string.

------------

解码使用 `base-64` 编码的数据字符串。

使用 `base-64` 编码为给定字符串创建 `Buffer`，并使用 `Buffer.toString（'binary'）` 返回已解码的字符串。

```js
const atob = str => Buffer.from(str, 'base64').toString('binary');
```

```js
atob('Zm9vYmFy'); // 'foobar'
```
