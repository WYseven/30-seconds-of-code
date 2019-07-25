### mapObject

------------

Maps the values of an array to an object using a function, where the key-value pairs consist of the stringified value as the key and the mapped value.

Use an anonymous inner function scope to declare an undefined memory space, using closures to store a return value. Use a new `Array` to store the array with a map of the function over its data set and a comma operator to return a second step, without needing to move from one context to another (due to closures and order of operations).

------------

使用一个函数将数组的值映射到对象，在键值对中，原始值作为键，映射值作为值。

使用一个匿名的内部函数作用域来声明一个 undefined 的内存空间，使用闭包来存储返回值。 使用一个新的 `Array` 来存储带有函数映射的数组和一个逗号运算符来返回第二个步骤，而不需要从一个上下文移动到另一个上下文（由于闭包和操作顺序）。

```js
const mapObject = (arr, fn) =>
  (a => (
    (a = [arr, arr.map(fn)]), a[0].reduce((acc, val, ind) => ((acc[val] = a[1][ind]), acc), {})
  ))();
```

```js
const squareIt = arr => mapObject(arr, a => a * a);
squareIt([1, 2, 3]); // { 1: 1, 2: 4, 3: 9 }
```
