### initial

------------

Returns all the elements of an array except the last one.

Use `arr.slice(0,-1)` to return all but the last element of the array.

------------

返回数组中除最后一个元素外的所有元素。

使用 `arr.slice(0，-1)` 返回数组中除最后一个元素外的所有元素。

```js
const initial = arr => arr.slice(0, -1);
```

```js
initial([1, 2, 3]); // [1,2]
```
