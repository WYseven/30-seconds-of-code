### reject

------------

Takes a predicate and array, like `Array.prototype.filter()`, but only keeps `x` if `pred(x) === false`.

------------

注：过滤掉符合断言函数条件的值

接受断言函数和数组，使用 `array .prototype.filter()` ，但仅当 `pred(x) === false` 时才保留 `x` 。

```js
const reject = (pred, array) => array.filter((...args) => !pred(...args));
```

```js
reject(x => x % 2 === 0, [1, 2, 3, 4, 5]); // [1, 3, 5]
reject(word => word.length > 4, ['Apple', 'Pear', 'Kiwi', 'Banana']); // ['Pear', 'Kiwi']
```
