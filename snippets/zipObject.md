### zipObject

------------

Given an array of valid property identifiers and an array of values, return an object associating the properties to the values.

Since an object can have undefined values but not undefined property pointers, the array of properties is used to decide the structure of the resulting object using `Array.prototype.reduce()`.

------------

给定一个有效属性标识符数组和一个值数组，返回一个将属性关联到值的对象。

由于对象可以有未定义的值，但不能有未定义的属性名，所以属性数组使用 `array.prototype.reduce()` 来决定结果对象的结构。

```js
const zipObject = (props, values) =>
  props.reduce((obj, prop, index) => ((obj[prop] = values[index]), obj), {});
```

```js
zipObject(['a', 'b', 'c'], [1, 2]); // {a: 1, b: 2, c: undefined}
zipObject(['a', 'b'], [1, 2, 3]); // {a: 1, b: 2}
```
