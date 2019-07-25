### shuffle

------------

Randomizes the order of the values of an array, returning a new array.

Uses the [Fisher-Yates algorithm](https://github.com/30-seconds/30-seconds-of-code#shuffle) to reorder the elements of the array.

------------

随机排列指定数组元素的顺序，返回一个新的数组。

使用 [Fisher-Yates algorithm](https://github.com/30-seconds/30-seconds-of-code#shuffle) 算法 对数组元素进行重新排序。

```js
const shuffle = ([...arr]) => {
  let m = arr.length;
  while (m) {
    const i = Math.floor(Math.random() * m--);
    [arr[m], arr[i]] = [arr[i], arr[m]];
  }
  return arr;
};
```

```js
const foo = [1, 2, 3];
shuffle(foo); // [2, 3, 1], foo = [1, 2, 3]
```
