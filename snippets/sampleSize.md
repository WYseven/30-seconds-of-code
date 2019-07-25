### sampleSize

------------

Gets `n` random elements at unique keys from `array` up to the size of `array`.

Shuffle the array using the [Fisher-Yates algorithm](https://github.com/30-seconds/30-seconds-of-code#shuffle).
Use `Array.prototype.slice()` to get the first `n` elements.
Omit the second argument, `n` to get only one element at random from the array.

------------

从 `array` 中获取 `n` 个唯一键随机元素。

使用 [Fisher-Yates algorithm](https://github.com/30-seconds/30-seconds-of-code#shuffle)算法 对数组进行打乱。 使用`Array.prototype.slice()` 获取 `n` 个元素。 
省略第二个参数 `n`， 从数组中随机获取 1 个元素。

```js
const sampleSize = ([...arr], n = 1) => {
  let m = arr.length;
  while (m) {
    const i = Math.floor(Math.random() * m--);
    [arr[m], arr[i]] = [arr[i], arr[m]];
  }
  return arr.slice(0, n);
};
```

```js
sampleSize([1, 2, 3], 2); // [3,1]
sampleSize([1, 2, 3], 4); // [2,3,1]
```
