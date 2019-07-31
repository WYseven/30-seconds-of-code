[![Logo](/logo.png)](https://30secondsofcode.org/)

# 30 seconds of code

[![License](https://img.shields.io/badge/license-CC0--1.0-blue.svg)](https://github.com/WYseven/30-seconds-of-code/blob/master/LICENSE) [![npm Downloads](https://img.shields.io/npm/dt/30-seconds-of-code.svg)](https://www.npmjs.com/package/30-seconds-of-code) [![npm Version](https://img.shields.io/npm/v/30-seconds-of-code.svg)](https://www.npmjs.com/package/30-seconds-of-code) [![Known Vulnerabilities](https://snyk.io/test/github/30-seconds/30-seconds-of-code/badge.svg?targetFile=package.json)](https://snyk.io/test/github/30-seconds/30-seconds-of-code?targetFile=package.json) <br/> 
[![Travis Build](https://travis-ci.com/30-seconds/30-seconds-of-code.svg?branch=master)](https://travis-ci.com/30-seconds/30-seconds-of-code) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/6ab7791fb1ea40b4a576d658fb96807f)](https://www.codacy.com/app/Chalarangelo/30-seconds-of-code?utm_source=github.com&utm_medium=referral&utm_content=30-seconds/30-seconds-of-code&utm_campaign=Badge_Grade) [![js-semistandard-style](https://img.shields.io/badge/code%20style-semistandard-brightgreen.svg)](https://github.com/Flet/semistandard) <br/>
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![ProductHunt](https://img.shields.io/badge/producthunt-vote-orange.svg)](https://www.producthunt.com/posts/30-seconds-of-code) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

> 精选有用的JavaScript代码片段，您可以在30秒或更短的时间内理解它们。

* 使用 <kbd>Ctrl</kbd> + <kbd>F</kbd> 或者 <kbd>command</kbd> + <kbd>F</kbd> 搜索你需要的代码片段
* 欢迎投稿, 请阅读投稿指南 [投稿指南](CONTRIBUTING.md).
* 代码段是在 ES6 中编写的, 请使用 [Babel transpiler](https://babeljs.io/) 确保向后兼容。
* 你可以把代码片段导入到 `Vscode` 中，点击查看操作指南[这里](https://github.com/WYseven/30-seconds-of-code/tree/master/vscode_snippets).
* 您可以使用CLI应用程序从终端搜索、查看和复制这些代码片段 [查看这个仓库](https://github.com/sQVe/30s)。

> 原文：[https://github.com/30-seconds/30-seconds-of-code](https://github.com/30-seconds/30-seconds-of-code)
> 原作者：[Chalarangelo](https://github.com/Chalarangelo)
> 翻译地址地址：[https://wyseven.github.io/30-seconds-of-code/](https://wyseven.github.io/30-seconds-of-code/)
> 译者：[戎马](https://github.com/WYseven)

本文翻译为译者所有，如有需要转载，请详细注明以上信息，谢谢合作。

#### 相关项目

* [30 Seconds of CSS](https://30-seconds.github.io/30-seconds-of-css/)
* [30 Seconds of Interviews](https://30secondsofinterviews.org/)
* [30 Seconds of React](https://github.com/30-seconds/30-seconds-of-react)
* [30 Seconds of Python](https://github.com/30-seconds/30-seconds-of-python-code)
* [30 Seconds of PHP](https://github.com/30-seconds/30-seconds-of-php-code)
* [30 Seconds of Knowledge](https://chrome.google.com/webstore/detail/30-seconds-of-knowledge/mmgplondnjekobonklacmemikcnhklla)
* [30 Seconds of Kotlin](https://github.com/IvanMwiruki/30-seconds-of-kotlin) _(unofficial)_

#### Package

⚠️ **NOTICE:** 我们的一些代码片段还没有针对生产环境进行优化(请参阅个别代码片段问题的免责声明).

您可以找到一个包含所有代码片段的包 [npm](https://www.npmjs.com/package/30-seconds-of-code).

```bash
# With npm
npm install 30-seconds-of-code

# With yarn
yarn add 30-seconds-of-code
```

[CDN link](https://unpkg.com/30-seconds-of-code/)

<details>
<summary>使用细节</summary>

**Browser**

```html
<script src="https://unpkg.com/30-seconds-of-code@1/dist/_30s.es5.min.js"></script>
<script>
  _30s.average(1, 2, 3);
</script>
```

**Node 中使用**

```js
// CommonJS
const _30s = require('30-seconds-of-code');
_30s.average(1, 2, 3);

// ES Modules
import _30s from '30-seconds-of-code';
_30s.average(1, 2, 3);
```

</details>

## 内容

### 🔌 Adapter

<details>
<summary>View contents</summary>

* [`ary`](#ary)
* [`call`](#call)
* [`collectInto`](#collectinto)
* [`flip`](#flip)
* [`over`](#over)
* [`overArgs`](#overargs)
* [`pipeAsyncFunctions`](#pipeasyncfunctions)
* [`pipeFunctions`](#pipefunctions)
* [`promisify`](#promisify)
* [`rearg`](#rearg)
* [`spreadOver`](#spreadover)
* [`unary`](#unary)

</details>

### 📚 Array

<details>
<summary>View contents</summary>

* [`all`](#all)
* [`allEqual`](#allequal)
* [`any`](#any)
* [`arrayToCSV`](#arraytocsv)
* [`bifurcate`](#bifurcate)
* [`bifurcateBy`](#bifurcateby)
* [`chunk`](#chunk)
* [`compact`](#compact)
* [`countBy`](#countby)
* [`countOccurrences`](#countoccurrences)
* [`deepFlatten`](#deepflatten)
* [`difference`](#difference)
* [`differenceBy`](#differenceby)
* [`differenceWith`](#differencewith)
* [`drop`](#drop)
* [`dropRight`](#dropright)
* [`dropRightWhile`](#droprightwhile)
* [`dropWhile`](#dropwhile)
* [`everyNth`](#everynth)
* [`filterFalsy`](#filterfalsy)
* [`filterNonUnique`](#filternonunique)
* [`filterNonUniqueBy`](#filternonuniqueby)
* [`findLast`](#findlast)
* [`findLastIndex`](#findlastindex)
* [`flatten`](#flatten)
* [`forEachRight`](#foreachright)
* [`groupBy`](#groupby)
* [`head`](#head)
* [`indexOfAll`](#indexofall)
* [`initial`](#initial)
* [`initialize2DArray`](#initialize2darray)
* [`initializeArrayWithRange`](#initializearraywithrange)
* [`initializeArrayWithRangeRight`](#initializearraywithrangeright)
* [`initializeArrayWithValues`](#initializearraywithvalues)
* [`initializeNDArray`](#initializendarray)
* [`intersection`](#intersection)
* [`intersectionBy`](#intersectionby)
* [`intersectionWith`](#intersectionwith)
* [`isSorted`](#issorted)
* [`join`](#join)
* [`JSONtoCSV`](#jsontocsv-)
* [`last`](#last)
* [`longestItem`](#longestitem)
* [`mapObject`](#mapobject-)
* [`maxN`](#maxn)
* [`minN`](#minn)
* [`none`](#none)
* [`nthElement`](#nthelement)
* [`offset`](#offset)
* [`partition`](#partition)
* [`permutations`](#permutations-)
* [`pull`](#pull)
* [`pullAtIndex`](#pullatindex-)
* [`pullAtValue`](#pullatvalue-)
* [`pullBy`](#pullby-)
* [`reducedFilter`](#reducedfilter)
* [`reduceSuccessive`](#reducesuccessive)
* [`reduceWhich`](#reducewhich)
* [`reject`](#reject)
* [`remove`](#remove)
* [`sample`](#sample)
* [`sampleSize`](#samplesize)
* [`shank`](#shank)
* [`shuffle`](#shuffle)
* [`similarity`](#similarity)
* [`sortedIndex`](#sortedindex)
* [`sortedIndexBy`](#sortedindexby)
* [`sortedLastIndex`](#sortedlastindex)
* [`sortedLastIndexBy`](#sortedlastindexby)
* [`stableSort`](#stablesort-)
* [`symmetricDifference`](#symmetricdifference)
* [`symmetricDifferenceBy`](#symmetricdifferenceby)
* [`symmetricDifferenceWith`](#symmetricdifferencewith)
* [`tail`](#tail)
* [`take`](#take)
* [`takeRight`](#takeright)
* [`takeRightWhile`](#takerightwhile)
* [`takeWhile`](#takewhile)
* [`toHash`](#tohash)
* [`union`](#union)
* [`unionBy`](#unionby)
* [`unionWith`](#unionwith)
* [`uniqueElements`](#uniqueelements)
* [`uniqueElementsBy`](#uniqueelementsby)
* [`uniqueElementsByRight`](#uniqueelementsbyright)
* [`uniqueSymmetricDifference`](#uniquesymmetricdifference)
* [`unzip`](#unzip)
* [`unzipWith`](#unzipwith-)
* [`without`](#without)
* [`xProd`](#xprod)
* [`zip`](#zip)
* [`zipObject`](#zipobject)
* [`zipWith`](#zipwith-)

</details>

### 🌐 Browser

<details>
<summary>View contents</summary>

* [`arrayToHtmlList`](#arraytohtmllist)
* [`bottomVisible`](#bottomvisible)
* [`copyToClipboard`](#copytoclipboard-)
* [`counter`](#counter-)
* [`createElement`](#createelement)
* [`createEventHub`](#createeventhub-)
* [`currentURL`](#currenturl)
* [`detectDeviceType`](#detectdevicetype)
* [`elementContains`](#elementcontains)
* [`elementIsVisibleInViewport`](#elementisvisibleinviewport-)
* [`formToObject`](#formtoobject)
* [`getImages`](#getimages)
* [`getScrollPosition`](#getscrollposition)
* [`getStyle`](#getstyle)
* [`hasClass`](#hasclass)
* [`hashBrowser`](#hashbrowser-)
* [`hide`](#hide)
* [`httpsRedirect`](#httpsredirect)
* [`insertAfter`](#insertafter)
* [`insertBefore`](#insertbefore)
* [`isBrowserTabFocused`](#isbrowsertabfocused)
* [`nodeListToArray`](#nodelisttoarray)
* [`observeMutations`](#observemutations-)
* [`off`](#off)
* [`on`](#on)
* [`onUserInputChange`](#onuserinputchange-)
* [`prefix`](#prefix)
* [`recordAnimationFrames`](#recordanimationframes)
* [`redirect`](#redirect)
* [`runAsync`](#runasync-)
* [`scrollToTop`](#scrolltotop)
* [`serializeForm`](#serializeform)
* [`setStyle`](#setstyle)
* [`show`](#show)
* [`smoothScroll`](#smoothscroll)
* [`toggleClass`](#toggleclass)
* [`triggerEvent`](#triggerevent)
* [`UUIDGeneratorBrowser`](#uuidgeneratorbrowser)

</details>

### ⏱️ Date

<details>
<summary>View contents</summary>

* [`dayOfYear`](#dayofyear)
* [`formatDuration`](#formatduration)
* [`getColonTimeFromDate`](#getcolontimefromdate)
* [`getDaysDiffBetweenDates`](#getdaysdiffbetweendates)
* [`getMeridiemSuffixOfInteger`](#getmeridiemsuffixofinteger)
* [`isAfterDate`](#isafterdate)
* [`isBeforeDate`](#isbeforedate)
* [`isSameDate`](#issamedate)
* [`isWeekday`](#isweekday)
* [`isWeekend`](#isweekend)
* [`maxDate`](#maxdate)
* [`minDate`](#mindate)
* [`tomorrow`](#tomorrow)
* [`yesterday`](#yesterday)

</details>

### 🎛️ Function

<details>
<summary>View contents</summary>

* [`attempt`](#attempt)
* [`bind`](#bind)
* [`bindKey`](#bindkey)
* [`chainAsync`](#chainasync)
* [`checkProp`](#checkprop)
* [`compose`](#compose)
* [`composeRight`](#composeright)
* [`converge`](#converge)
* [`curry`](#curry)
* [`debounce`](#debounce)
* [`defer`](#defer)
* [`delay`](#delay)
* [`functionName`](#functionname)
* [`hz`](#hz)
* [`memoize`](#memoize-)
* [`negate`](#negate)
* [`once`](#once)
* [`partial`](#partial)
* [`partialRight`](#partialright)
* [`runPromisesInSeries`](#runpromisesinseries)
* [`sleep`](#sleep)
* [`throttle`](#throttle-)
* [`times`](#times)
* [`uncurry`](#uncurry)
* [`unfold`](#unfold)
* [`when`](#when)

</details>

### ➗ Math

<details>
<summary>View contents</summary>

* [`approximatelyEqual`](#approximatelyequal)
* [`average`](#average)
* [`averageBy`](#averageby)
* [`binomialCoefficient`](#binomialcoefficient)
* [`clampNumber`](#clampnumber)
* [`degreesToRads`](#degreestorads)
* [`digitize`](#digitize)
* [`distance`](#distance)
* [`elo`](#elo-)
* [`factorial`](#factorial)
* [`fibonacci`](#fibonacci)
* [`gcd`](#gcd)
* [`geometricProgression`](#geometricprogression)
* [`hammingDistance`](#hammingdistance)
* [`inRange`](#inrange)
* [`isDivisible`](#isdivisible)
* [`isEven`](#iseven)
* [`isNegativeZero`](#isnegativezero)
* [`isPrime`](#isprime)
* [`lcm`](#lcm)
* [`luhnCheck`](#luhncheck-)
* [`mapNumRange`](#mapnumrange)
* [`maxBy`](#maxby)
* [`median`](#median)
* [`midpoint`](#midpoint)
* [`minBy`](#minby)
* [`percentile`](#percentile)
* [`powerset`](#powerset)
* [`primes`](#primes)
* [`radsToDegrees`](#radstodegrees)
* [`randomIntArrayInRange`](#randomintarrayinrange)
* [`randomIntegerInRange`](#randomintegerinrange)
* [`randomNumberInRange`](#randomnumberinrange)
* [`round`](#round)
* [`sdbm`](#sdbm)
* [`standardDeviation`](#standarddeviation)
* [`sum`](#sum)
* [`sumBy`](#sumby)
* [`sumPower`](#sumpower)
* [`toSafeInteger`](#tosafeinteger)
* [`vectorDistance`](#vectordistance)

</details>

### 📦 Node

<details>
<summary>View contents</summary>

* [`atob`](#atob)
* [`btoa`](#btoa)
* [`colorize`](#colorize)
* [`createDirIfNotExists`](#createdirifnotexists)
* [`hasFlags`](#hasflags)
* [`hashNode`](#hashnode)
* [`isDuplexStream`](#isduplexstream)
* [`isReadableStream`](#isreadablestream)
* [`isStream`](#isstream)
* [`isTravisCI`](#istravisci)
* [`isWritableStream`](#iswritablestream)
* [`JSONToFile`](#jsontofile)
* [`readFileLines`](#readfilelines)
* [`untildify`](#untildify)
* [`UUIDGeneratorNode`](#uuidgeneratornode)

</details>

### 🗃️ Object

<details>
<summary>View contents</summary>

* [`bindAll`](#bindall)
* [`deepClone`](#deepclone)
* [`deepFreeze`](#deepfreeze)
* [`deepGet`](#deepget)
* [`deepMapKeys`](#deepmapkeys-)
* [`defaults`](#defaults)
* [`dig`](#dig)
* [`equals`](#equals-)
* [`findKey`](#findkey)
* [`findLastKey`](#findlastkey)
* [`flattenObject`](#flattenobject)
* [`forOwn`](#forown)
* [`forOwnRight`](#forownright)
* [`functions`](#functions)
* [`get`](#get)
* [`invertKeyValues`](#invertkeyvalues)
* [`lowercaseKeys`](#lowercasekeys)
* [`mapKeys`](#mapkeys)
* [`mapValues`](#mapvalues)
* [`matches`](#matches)
* [`matchesWith`](#matcheswith)
* [`merge`](#merge)
* [`nest`](#nest)
* [`objectFromPairs`](#objectfrompairs)
* [`objectToPairs`](#objecttopairs)
* [`omit`](#omit)
* [`omitBy`](#omitby)
* [`orderBy`](#orderby)
* [`pick`](#pick)
* [`pickBy`](#pickby)
* [`renameKeys`](#renamekeys)
* [`shallowClone`](#shallowclone)
* [`size`](#size)
* [`transform`](#transform)
* [`truthCheckCollection`](#truthcheckcollection)
* [`unflattenObject`](#unflattenobject-)

</details>

### 📜 String

<details>
<summary>View contents</summary>

* [`byteSize`](#bytesize)
* [`capitalize`](#capitalize)
* [`capitalizeEveryWord`](#capitalizeeveryword)
* [`compactWhitespace`](#compactwhitespace)
* [`CSVToArray`](#csvtoarray)
* [`CSVToJSON`](#csvtojson-)
* [`decapitalize`](#decapitalize)
* [`escapeHTML`](#escapehtml)
* [`escapeRegExp`](#escaperegexp)
* [`fromCamelCase`](#fromcamelcase)
* [`indentString`](#indentstring)
* [`isAbsoluteURL`](#isabsoluteurl)
* [`isAnagram`](#isanagram)
* [`isLowerCase`](#islowercase)
* [`isUpperCase`](#isuppercase)
* [`mapString`](#mapstring)
* [`mask`](#mask)
* [`pad`](#pad)
* [`palindrome`](#palindrome)
* [`pluralize`](#pluralize)
* [`removeNonASCII`](#removenonascii)
* [`reverseString`](#reversestring)
* [`sortCharactersInString`](#sortcharactersinstring)
* [`splitLines`](#splitlines)
* [`stringPermutations`](#stringpermutations-)
* [`stripHTMLTags`](#striphtmltags)
* [`toCamelCase`](#tocamelcase)
* [`toKebabCase`](#tokebabcase)
* [`toSnakeCase`](#tosnakecase)
* [`toTitleCase`](#totitlecase)
* [`truncateString`](#truncatestring)
* [`unescapeHTML`](#unescapehtml)
* [`URLJoin`](#urljoin-)
* [`words`](#words)

</details>

### 📃 Type

<details>
<summary>View contents</summary>

* [`getType`](#gettype)
* [`is`](#is)
* [`isArrayLike`](#isarraylike)
* [`isBoolean`](#isboolean)
* [`isEmpty`](#isempty)
* [`isFunction`](#isfunction)
* [`isNil`](#isnil)
* [`isNull`](#isnull)
* [`isNumber`](#isnumber)
* [`isObject`](#isobject)
* [`isObjectLike`](#isobjectlike)
* [`isPlainObject`](#isplainobject)
* [`isPrimitive`](#isprimitive)
* [`isPromiseLike`](#ispromiselike)
* [`isString`](#isstring)
* [`isSymbol`](#issymbol)
* [`isUndefined`](#isundefined)
* [`isValidJSON`](#isvalidjson)

</details>

### 🔧 Utility

<details>
<summary>View contents</summary>

* [`castArray`](#castarray)
* [`cloneRegExp`](#cloneregexp)
* [`coalesce`](#coalesce)
* [`coalesceFactory`](#coalescefactory)
* [`extendHex`](#extendhex)
* [`getURLParameters`](#geturlparameters)
* [`hexToRGB`](#hextorgb-)
* [`httpGet`](#httpget)
* [`httpPost`](#httppost)
* [`isBrowser`](#isbrowser)
* [`mostPerformant`](#mostperformant)
* [`nthArg`](#ntharg)
* [`parseCookie`](#parsecookie)
* [`prettyBytes`](#prettybytes-)
* [`randomHexColorCode`](#randomhexcolorcode)
* [`RGBToHex`](#rgbtohex)
* [`serializeCookie`](#serializecookie)
* [`timeTaken`](#timetaken)
* [`toCurrency`](#tocurrency)
* [`toDecimalMark`](#todecimalmark)
* [`toOrdinalSuffix`](#toordinalsuffix)
* [`validateNumber`](#validatenumber)
* [`yesNo`](#yesno)

</details>


---

## 🔌 Adapter

### ary



创建一个函数，该函数接受最多 `n` 个参数，忽略任何其他参数。

调用提供的函数 `fn`，参数最多为 `n`个，使用 `Array.prototype.slice(0,n)` 和 spread 操作符(`...`)提取并传入参数。


```js
const ary = (fn, n) => (...args) => fn(...args.slice(0, n));
```

<details>
<summary>Examples</summary>

```js
const firstTwoMax = ary(Math.max, 2);
[[2, 6, 'a'], [8, 4, 6], [10]].map(x => firstTwoMax(...x)); // [6, 8, 10]
```

</details>

<br>[⬆ Back to top](#contents)

### call



给定一个 `key` 和一组参数，在给定上下文时调用它们。主要用于函数组合。

使用闭包以存储的参数调用存储的 `key`。

```js
const call = (key, ...args) => context => context[key](...args);
```

<details>
<summary>Examples</summary>

```js
Promise.resolve([1, 2, 3])
  .then(call('map', x => 2 * x))
  .then(console.log); // [ 2, 4, 6 ]
const map = call.bind(null, 'map');
Promise.resolve([1, 2, 3])
  .then(map(x => 2 * x))
  .then(console.log); // [ 2, 4, 6 ]
```

</details>

<br>[⬆ Back to top](#contents)

### collectInto

------------

Changes a function that accepts an array into a variadic function.

Given a function, return a closure that collects all inputs into an array-accepting function.

------------

将接受数组的函数改变为接收可变参数函数。

给定一个函数，返回一个闭包，该闭包将所有输入收集到一个接受数组的函数中。

```js
const collectInto = fn => (...args) => fn(args);
```

<details>
<summary>Examples</summary>

```js
const Pall = collectInto(Promise.all.bind(Promise));
let p1 = Promise.resolve(1);
let p2 = Promise.resolve(2);
let p3 = new Promise(resolve => setTimeout(resolve, 2000, 3));
Pall(p1, p2, p3).then(console.log); // [1, 2, 3] (after about 2 seconds)
```

</details>

<br>[⬆ Back to top](#contents)

### flip



接受一个函数作为参数，然后将该函数第一个参数作为最后一个参数。（注：翻转参数）

返回一个接受可变参数输入的闭包，并且在应用其余参数之前将最后一个参数作为第一个参数。


```js
const flip = fn => (first, ...rest) => fn(...rest, first);
```

<details>
<summary>Examples</summary>

```js
let a = { name: 'John Smith' };
let b = {};
const mergeFrom = flip(Object.assign);
let mergePerson = mergeFrom.bind(null, a);
mergePerson(b); // == b
b = {};
Object.assign(b, a); // == b
```

</details>

<br>[⬆ Back to top](#contents)

### over



创建一个函数，该函数使用接收到的参数调用所提供的每个函数并返回结果。

使用 `Array.prototype.map()` 和 `Function.prototype.apply()` 将每个函数应用于给定的参数。

```js
const over = (...fns) => (...args) => fns.map(fn => fn.apply(null, args));
```

<details>
<summary>Examples</summary>

```js
const minMax = over(Math.min, Math.max);
minMax(1, 2, 3, 4, 5); // [1,5]
```

</details>

<br>[⬆ Back to top](#contents)

### overArgs



创建一个函数，该函数调用所提供的函数并对传入的参数进行转换。

使用 `Array.prototype.map()` 将 `transform` 应用于 `args` ，并结合扩展操作符 (`...`) 将转换后的参数传递给 `fn` 。

```js
const overArgs = (fn, transforms) => (...args) => fn(...args.map((val, i) => transforms[i](val)));
```

<details>
<summary>Examples</summary>

```js
const square = n => n * n;
const double = n => n * 2;
const fn = overArgs((x, y) => [x, y], [square, double]);
fn(9, 3); // [81, 6]
```

</details>

<br>[⬆ Back to top](#contents)

### pipeAsyncFunctions



为返回的异步函数，从左到右依次执行函数组合。

使用 `Array.prototype.reduce()` 和扩展操作符 (`...`) ，并结合`Promise.then()`，从左到右依次执行函数组合。
函数的返回值，可以是:简单值、`Promise`对象，或者可以定义为 `async` ，通过 `wait` 返回值。

```js
const pipeAsyncFunctions = (...fns) => arg => fns.reduce((p, f) => p.then(f), Promise.resolve(arg));
```

<details>
<summary>Examples</summary>

```js
const sum = pipeAsyncFunctions(
  x => x + 1,
  x => new Promise(resolve => setTimeout(() => resolve(x + 2), 1000)),
  x => x + 3,
  async x => (await x) + 4
);
(async() => {
  console.log(await sum(5)); // 15 (after one second)
})();
```

</details>

<br>[⬆ Back to top](#contents)

### pipeFunctions



从左到右执行函数组合。

使用 `Array.prototype.reduce()` 和扩展操作符 (`...`) 来执行从左到右的函数组合。
第一个(最左边)函数可以接受一个或多个参数;其余的函数只接受一个参数。

```js
const pipeFunctions = (...fns) => fns.reduce((f, g) => (...args) => g(f(...args)));
```

<details>
<summary>Examples</summary>

```js
const add5 = x => x + 5;
const multiply = (x, y) => x * y;
const multiplyAndAdd5 = pipeFunctions(multiply, add5);
multiplyAndAdd5(5, 2); // 15
```

</details>

<br>[⬆ Back to top](#contents)

### promisify



将异步函数转换后，返回成 `Promise` 对象。

使用柯里化函数，返回调用原始函数的 `Promise` 对象。
使用的 `...rest` 操作符传入所有参数。

*在 Node 8+中，你可以使用 [`util.promisify`](https://nodejs.org/api/util.html#util_util_promisify_original)*

```js
const promisify = func => (...args) =>
  new Promise((resolve, reject) =>
    func(...args, (err, result) => (err ? reject(err) : resolve(result)))
  );
```

<details>
<summary>Examples</summary>

```js
const delay = promisify((d, cb) => setTimeout(cb, d));
delay(2000).then(() => console.log('Hi!')); // // Promise resolves after 2s
```

</details>

<br>[⬆ Back to top](#contents)

### rearg



创建一个函数，该函数调用提供的函数，并根据指定的索引排列参数。

使用 `Array.prototype.map()` 根据 `indexes` 和扩展操作符 (`...`) 对参数重新排序，将转换后的参数传递给 `fn` 。

```js
const rearg = (fn, indexes) => (...args) => fn(...indexes.map(i => args[i]));
```

<details>
<summary>Examples</summary>

```js
var rearged = rearg(
  function(a, b, c) {
    return [a, b, c];
  },
  [2, 0, 1]
);
rearged('b', 'c', 'a'); // ['a', 'b', 'c']
```

</details>

<br>[⬆ Back to top](#contents)

### spreadOver

------------

Takes a variadic function and returns a closure that accepts an array of arguments to map to the inputs of the function.

Use closures and the spread operator (`...`) to map the array of arguments to the inputs of the function.

------------

接受一个可变参数的函数并返回一个闭包函数，该闭包函数接受要映射到函数的参数数组。

使用闭包和扩展操作符 (`...`) 将参数数组一一映射为函数的参数。

```js
const spreadOver = fn => argsArr => fn(...argsArr);
```

<details>
<summary>Examples</summary>

```js
const arrayMax = spreadOver(Math.max);
arrayMax([1, 2, 3]); // 3
```

</details>

<br>[⬆ Back to top](#contents)

### unary



创建一个函数，该函数最多只接受一个参数，忽略其他的参数。

调用提供的函数 `fn`，只需要给第一个参数即可。

```js
const unary = fn => val => fn(val);
```

<details>
<summary>Examples</summary>

```js
['6', '8', '10'].map(unary(parseInt)); // [6, 8, 10]
```

</details>

<br>[⬆ Back to top](#contents)


---

## 📚 Array

### all



如果提供的断言函数（predicate function）对集合中所有的元素测试都返回 `true`，那么 `all` 方法就返回 `true`。否则，返回 `false`。

使用 `Array.prototype.every()` 测试集合中的所有元素是否基于 `fn` 返回 `true`。
省略第二个参数`fn`，使用 `Boolean` 作为默认值。

```js
const all = (arr, fn = Boolean) => arr.every(fn);
```

<details>
<summary>Examples</summary>

```js
all([4, 2, 3], x => x > 1); // true
all([1, 2, 3]); // true
```

</details>

<br>[⬆ Back to top](#contents)

### allEqual



检查数组中的所有元素是否相等。

使用 `Array.prototype.every()` 检查数组中的所有元素是否与第一个元素相同。
使用严格比较运算符比较数组中的元素，该运算符不考虑 `NaN` 与自己不相等的情况。

```js
const allEqual = arr => arr.every(val => val === arr[0]);
```

<details>
<summary>Examples</summary>

```js
allEqual([1, 2, 3, 4, 5, 6]); // false
allEqual([1, 1, 1, 1]); // true
```

</details>

<br>[⬆ Back to top](#contents)

### any



如果提供的断言函数（predicate function）对集合中所有的元素测试，至少有一个返回 `true`，那么 `any` 方法就返回 `true`。否则，返回 `false`。

使用 `Array.prototype.some()` 测试集合中的所有元素是否基于 `fn` 返回 `true`。
省略第二个参数`fn`，使用 `Boolean` 作为默认值。

```js
const any = (arr, fn = Boolean) => arr.some(fn);
```

<details>
<summary>Examples</summary>

```js
any([0, 1, 2, 0], x => x >= 2); // true
any([0, 0, 1, 0]); // true
```

</details>

<br>[⬆ Back to top](#contents)

### arrayToCSV



将二维数组转换为逗号分隔值（CSV）字符串。

使用 `Array.prototype.map()` 和 `Array.prototype.join(delimiter)` 将单个一维数组(行)组合成字符串。
使用 `Array.prototype.join('\n')` 将所有行组合成 CSV 字符串，用换行符分隔每一行。
省略第二个参数 `delimiter` ，以使用'，'的默认分隔符。

```js
const arrayToCSV = (arr, delimiter = ',') =>
  arr
    .map(v => v.map(x => (isNaN(x) ? `"${x.replace(/"/g, '""')}"` : x)).join(delimiter))
    .join('\n');
```

<details>
<summary>Examples</summary>

```js
arrayToCSV([['a', 'b'], ['c', 'd']]); // '"a","b"\n"c","d"'
arrayToCSV([['a', 'b'], ['c', 'd']], ';'); // '"a";"b"\n"c";"d"'
arrayToCSV([['a', '"b" great'], ['c', 3.1415]]); // '"a","""b"" great"\n"c",3.1415'
```

</details>

<br>[⬆ Back to top](#contents)

### bifurcate



将值分成两组，如果 `filter` 中的元素为 `true`，则集合中对应的元素属于第一组;否则，它属于第二组。

基于 `filter`，使用 `Array.prototype.reduce()` 和 `Array.prototype.push()` 向组添加元素。

```js
const bifurcate = (arr, filter) =>
  arr.reduce((acc, val, i) => (acc[filter[i] ? 0 : 1].push(val), acc), [[], []]);
```

<details>
<summary>Examples</summary>

```js
bifurcate(['beep', 'boop', 'foo', 'bar'], [true, true, false, true]); // [ ['beep', 'boop', 'bar'], ['foo'] ]
```

</details>

<br>[⬆ Back to top](#contents)

### bifurcateBy



根据断言函数（predicate function）会将值分成两组，集合中的元素输入到断言函数中后，来确定元素属于哪一组。如果断言函数返回一个真值，则集合元素属于第一组;否则，它属于第二组。

```js
const bifurcateBy = (arr, fn) =>
  arr.reduce((acc, val, i) => (acc[fn(val, i) ? 0 : 1].push(val), acc), [[], []]);
```

<details>
<summary>Examples</summary>

```js
bifurcateBy(['beep', 'boop', 'foo', 'bar'], x => x[0] === 'b'); // [ ['beep', 'boop', 'bar'], ['foo'] ]
```

</details>

<br>[⬆ Back to top](#contents)

### chunk



将数组分块成指定大小的较小数组。

使用 `array.from()` 创建一个新的数组，该数组的长度就是将要生成的块（chunk）的个数。
使用 `array.prototype.slice()` 将新数组的每个元素映射为一个长度为 `size` 的块（chunk）。
如果原始数组不能被平均分割，那么最后的块（chunk）将包含剩余的元素。

```js
const chunk = (arr, size) =>
  Array.from({ length: Math.ceil(arr.length / size) }, (v, i) =>
    arr.slice(i * size, i * size + size)
  );
```

<details>
<summary>Examples</summary>

```js
chunk([1, 2, 3, 4, 5], 2); // [[1,2],[3,4],[5]]
```

</details>

<br>[⬆ Back to top](#contents)

### compact



从数组中删除为 `false` 的值。

使用 `Array.prototype.filter()` 过滤掉数组中所有为假值的元素 (`false`, `null`, `0`, `""`, `undefined`, 和 `NaN`)。

```js
const compact = arr => arr.filter(Boolean);
```

<details>
<summary>Examples</summary>

```js
compact([0, 1, false, 2, '', 3, 'a', 'e' * 23, NaN, 's', 34]); // [ 1, 2, 3, 'a', 's', 34 ]
```

</details>

<br>[⬆ Back to top](#contents)

### countBy



根据给定函数对数组的元素进行分组，并返回每个组中的元素数量。

使用 `array .prototype.map()` 将数组的值映射到函数或属性名称。
使用 `Array.prototype.reduce()` 创建一个对象，其中键（`key`）是从映射的结果中产生的。

```js
const countBy = (arr, fn) =>
  arr.map(typeof fn === 'function' ? fn : val => val[fn]).reduce((acc, val) => {
    acc[val] = (acc[val] || 0) + 1;
    return acc;
  }, {});
```

<details>
<summary>Examples</summary>

```js
countBy([6.1, 4.2, 6.3], Math.floor); // {4: 1, 6: 2}
countBy(['one', 'two', 'three'], 'length'); // {3: 2, 5: 1}
```

</details>

<br>[⬆ Back to top](#contents)

### countOccurrences



计算数组中值的出现次数。

每次在数组中遇到指定的值时，使用 `array. prototype.reduce()` 递增计数器。

```js
const countOccurrences = (arr, val) => arr.reduce((a, v) => (v === val ? a + 1 : a), 0);
```

<details>
<summary>Examples</summary>

```js
countOccurrences([1, 1, 2, 1, 2, 3], 1); // 3
```

</details>

<br>[⬆ Back to top](#contents)

### deepFlatten



深度平铺一个数组。

使用递归。
使用 `array. prototype.concat()` 和空数组( `[]` )，结合 spread 操作符('...')将数组平铺。
递归平铺数组中的每个元素。

```js
const deepFlatten = arr => [].concat(...arr.map(v => (Array.isArray(v) ? deepFlatten(v) : v)));
```

<details>
<summary>Examples</summary>

```js
deepFlatten([1, [2], [[3], 4], 5]); // [1,2,3,4,5]
```

</details>

<br>[⬆ Back to top](#contents)

### difference



返回两个数组之间的差异。

根据数组 `b` 创建一个 `Set` 对象，然后在数组 `a` 上使用 `Array.filter()` 方法，过滤出数组 `b` 中不包含的值。

```js
const difference = (a, b) => {
  const s = new Set(b);
  return a.filter(x => !s.has(x));
};
```

<details>
<summary>Examples</summary>

```js
difference([1, 2, 3], [1, 2, 4]); // [3]
```

</details>

<br>[⬆ Back to top](#contents)

### differenceBy



将提供的函数应用于两个数组的每个数组元素后，返回两个数组之间的差值。

将 `fn` 处理数组 `b` 中的每个元素后创建 `Set`，然后使用 `Array.prototype.map（）` 映射 `fn` 处理数组 `a` 中的每个元素，最后应用`Array.prototype.filter（）` 进行过滤。

```js
const differenceBy = (a, b, fn) => {
  const s = new Set(b.map(fn));
  return a.map(fn).filter(el => !s.has(el));
};
```

<details>
<summary>Examples</summary>

```js
differenceBy([2.1, 1.2], [2.3, 3.4], Math.floor); // [1]
differenceBy([{ x: 2 }, { x: 1 }], [{ x: 1 }], v => v.x); // [2]
```

</details>

<br>[⬆ Back to top](#contents)

### differenceWith



过滤出数组中比较函数不返回 `true` 的所有值。

使用 `Array.prototype.filter()` 和 `Array.prototype.findIndex()` 查找合适的值。

```js
const differenceWith = (arr, val, comp) => arr.filter(a => val.findIndex(b => comp(a, b)) === -1);
```

<details>
<summary>Examples</summary>

```js
differenceWith([1, 1.2, 1.5, 3, 0], [1.9, 3, 0], (a, b) => Math.round(a) === Math.round(b)); // [1, 1.2]
```

</details>

<br>[⬆ Back to top](#contents)

### drop



返回从左侧开始删除 `n` 个元素的新数组。

使用 `Array.prototype.slice()` 从左边删除指定数量的元素。

```js
const drop = (arr, n = 1) => arr.slice(n);
```

<details>
<summary>Examples</summary>

```js
drop([1, 2, 3]); // [2,3]
drop([1, 2, 3], 2); // [3]
drop([1, 2, 3], 42); // []
```

</details>

<br>[⬆ Back to top](#contents)

### dropRight



返回从右侧开始删除 `n` 个元素的新数组。

使用 `Array.prototype.slice()` 从右侧删除指定数量的元素。

```js
const dropRight = (arr, n = 1) => arr.slice(0, -n);
```

<details>
<summary>Examples</summary>

```js
dropRight([1, 2, 3]); // [1,2]
dropRight([1, 2, 3], 2); // [1]
dropRight([1, 2, 3], 42); // []
```

</details>

<br>[⬆ Back to top](#contents)

### dropRightWhile



从数组末尾移除元素，直到传递的函数返回 `true` 。返回数组中剩余的元素。

从数组的末尾开始循环遍历数组，使用 `array.prototype.slice()` 删除数组中第一个遇到函数返回的值为 `true` 位置的元素。
返回数组中剩余的元素。

```js
const dropRightWhile = (arr, func) => {
  let rightIndex = arr.length;
  while (rightIndex-- && !func(arr[rightIndex]));
  return arr.slice(0, rightIndex + 1);
};
```

<details>
<summary>Examples</summary>

```js
dropRightWhile([1, 2, 3, 4], n => n < 3); // [1, 2]
```

</details>

<br>[⬆ Back to top](#contents)

### dropWhile



移除数组中的元素，直到传递的函数返回 `true` 。 返回数组中剩余的元素。

循环遍历数组，使用 `array.prototype.slice()` 删除数组中第一个遇到函数返回的值为 `true` 位置的元素。
返回数组中剩余的元素。

```js
const dropWhile = (arr, func) => {
  while (arr.length > 0 && !func(arr[0])) arr = arr.slice(1);
  return arr;
};
```

<details>
<summary>Examples</summary>

```js
dropWhile([1, 2, 3, 4], n => n >= 3); // [3,4]
```

</details>

<br>[⬆ Back to top](#contents)

### everyNth

Returns every nth element in an array.

Use `Array.prototype.filter()` to create a new array that contains every nth element of a given array.



```js
const everyNth = (arr, nth) => arr.filter((e, i) => i % nth === nth - 1);
```

<details>
<summary>Examples</summary>

```js
everyNth([1, 2, 3, 4, 5, 6], 2); // [ 2, 4, 6 ]
```

</details>

<br>[⬆ Back to top](#contents)

### filterFalsy

------------

Filters out the falsy values in an array.

Use `Array.prototype.filter()` to get an array containing only truthy values.

------------

过滤数组中为假值（falsy）的元素。

使用 `array .prototype.filter()` 过滤后，数组中只包含为真值（truthy）的元素。

```js
const filterFalsy = arr => arr.filter(Boolean);
```

<details>
<summary>Examples</summary>

```js
filterFalsy(['', true, {}, false, 'sample', 1, 0]); // [true, {}, 'sample', 1]
```

</details>

<br>[⬆ Back to top](#contents)

### filterNonUnique



过滤掉数组中的非唯一值。

使用 `Array.prototype.filter()` 过滤非唯一值后，返回只包含唯一值的数组。

```js
const filterNonUnique = arr => arr.filter(i => arr.indexOf(i) === arr.lastIndexOf(i));
```

<details>
<summary>Examples</summary>

```js
filterNonUnique([1, 2, 2, 3, 4, 4, 5]); // [1, 3, 5]
```

</details>

<br>[⬆ Back to top](#contents)

### filterNonUniqueBy



根据提供的比较器（comparator）函数，过滤数组中的非唯一值。

基于比较器函数 `fn` ，使用 `array .prototype.filter()` 和 `array .prototype.every()` 对数组过滤后，数组中只包含唯一值。

比较器函数接受四个参数:正在比较的两个元素的值及其索引。

```js
const filterNonUniqueBy = (arr, fn) =>
  arr.filter((v, i) => arr.every((x, j) => (i === j) === fn(v, x, i, j)));
```

<details>
<summary>Examples</summary>

```js
filterNonUniqueBy(
  [
    { id: 0, value: 'a' },
    { id: 1, value: 'b' },
    { id: 2, value: 'c' },
    { id: 1, value: 'd' },
    { id: 0, value: 'e' }
  ],
  (a, b) => a.id == b.id
); // [ { id: 2, value: 'c' } ]
```

</details>

<br>[⬆ Back to top](#contents)

### findLast



通过提供的函数返回值为真值（truthy）过滤数组，返回这个数组最后一个元素。

使用 `Array.prototype.filter()` 过滤掉 `fn` 返回假值（falsy）的元素， 用 `Array.prototype.pop()` 获取最后一个值。

```js
const findLast = (arr, fn) => arr.filter(fn).pop();
```

<details>
<summary>Examples</summary>

```js
findLast([1, 2, 3, 4], n => n % 2 === 1); // 3
```

</details>

<br>[⬆ Back to top](#contents)

### findLastIndex



通过提供的函数返回值为真值（truthy）过滤数组，返回这个数组最后一个元素的下标。

使用 `array.prototype.map()` 将每个元素映射到具有其索引和值的数组。
使用 `Array.prototype.filter()` 过滤掉 `fn` 返回假值（falsy）的元素， 用 `Array.prototype.pop()` 获取最后一个值。

```js
const findLastIndex = (arr, fn) =>
  arr
    .map((val, i) => [i, val])
    .filter(([i, val]) => fn(val, i, arr))
    .pop()[0];
```

<details>
<summary>Examples</summary>

```js
findLastIndex([1, 2, 3, 4], n => n % 2 === 1); // 2 (index of the value 3)
```

</details>

<br>[⬆ Back to top](#contents)

### flatten



将数组展平到指定的深度。

使用递归，为每个深度级别 `depth` 递减 `1`。 使用 `Array.prototype.reduce()` 和 `Array.prototype.concat()` 来合并元素或数组。 基本情况下，`depth` 等于 `1` 停止递归。 省略第二个参数，`depth` 只能平铺到 `1` 层(单层平铺) 的深度。

```js
const flatten = (arr, depth = 1) =>
  arr.reduce((a, v) => a.concat(depth > 1 && Array.isArray(v) ? flatten(v, depth - 1) : v), []);
```

<details>
<summary>Examples</summary>

```js
flatten([1, [2], 3, 4]); // [1, 2, 3, 4]
flatten([1, [2, [3, [4, 5], 6], 7], 8], 2); // [1, 2, 3, [4, 5], 6, 7, 8]
```

</details>

<br>[⬆ Back to top](#contents)

### forEachRight



从数组的最后一个元素开始，为每个数组元素执行一次提供的函数。

使用 `Array.prototype.slice(0)` 克隆给定的数组，`Array.prototype.reverse()` 反转数组，`Array.prototype.forEach()` 遍历这个反转的数组。

```js
const forEachRight = (arr, callback) =>
  arr
    .slice(0)
    .reverse()
    .forEach(callback);
```

<details>
<summary>Examples</summary>

```js
forEachRight([1, 2, 3, 4], val => console.log(val)); // '4', '3', '2', '1'
```

</details>

<br>[⬆ Back to top](#contents)

### groupBy



根据给定的函数对数组的元素进行分组。

使用 `Array.prototype.map()` 将数组的值映射到函数或属性名称。使用 `Array.prototype.reduce()` 来创建一个对象，其中的 `key` 是从映射结果中产生。

```js
const groupBy = (arr, fn) =>
  arr.map(typeof fn === 'function' ? fn : val => val[fn]).reduce((acc, val, i) => {
    acc[val] = (acc[val] || []).concat(arr[i]);
    return acc;
  }, {});
```

<details>
<summary>Examples</summary>

```js
groupBy([6.1, 4.2, 6.3], Math.floor); // {4: [4.2], 6: [6.1, 6.3]}
groupBy(['one', 'two', 'three'], 'length'); // {3: ['one', 'two'], 5: ['three']}
```

</details>

<br>[⬆ Back to top](#contents)

### head



返回数组的第一个元素。

使用 `arr[0]` 返回传递数组的第一个元素。

```js
const head = arr => arr[0];
```

<details>
<summary>Examples</summary>

```js
head([1, 2, 3]); // 1
```

</details>

<br>[⬆ Back to top](#contents)

### indexOfAll



返回数组中 `val` 的所有索引。如果在数组中没找到 `val`，则返回 `[]` 。

使用 `Array.prototype.reduce()` 循环元素并存储匹配元素的索引。
返回索引数组。

```js
const indexOfAll = (arr, val) => arr.reduce((acc, el, i) => (el === val ? [...acc, i] : acc), []);
```

<details>
<summary>Examples</summary>

```js
indexOfAll([1, 2, 3, 1, 2, 3], 1); // [0,3]
indexOfAll([1, 2, 3], 4); // []
```

</details>

<br>[⬆ Back to top](#contents)

### initial



返回数组中除最后一个元素外的所有元素。

使用 `arr.slice(0，-1)` 返回数组中除最后一个元素外的所有元素。

```js
const initial = arr => arr.slice(0, -1);
```

<details>
<summary>Examples</summary>

```js
initial([1, 2, 3]); // [1,2]
```

</details>

<br>[⬆ Back to top](#contents)

### initialize2DArray



初始化一个给定行数和列数，以及值的二维数组。

使用 `array.prototype.map()` 生成 `h` 行，其中每一行都是长度为 `w` 的新数组。如果没有提供值 `val`，则默认为 `null`。


```js
const initialize2DArray = (w, h, val = null) =>
  Array.from({ length: h }).map(() => Array.from({ length: w }).fill(val));
```

<details>
<summary>Examples</summary>

```js
initialize2DArray(2, 2, 0); // [[0,0], [0,0]]
```

</details>

<br>[⬆ Back to top](#contents)

### initializeArrayWithRange



初始化一个数组，该数组包含指定范围 `start` 到 `end` 内的数字，可设置间隔 `step`。

使用 `Array.from()` 创建一个所需长度为 `(end - start + 1)/step` 的数组，并填充给定范围内要求的值。
你可以省略 `start` 来使用默认值 `0`。 
你可以省略 `step` 使用默认值 `1`。

```js
const initializeArrayWithRange = (end, start = 0, step = 1) =>
  Array.from({ length: Math.ceil((end - start + 1) / step) }, (v, i) => i * step + start);
```

<details>
<summary>Examples</summary>

```js
initializeArrayWithRange(5); // [0,1,2,3,4,5]
initializeArrayWithRange(7, 3); // [3,4,5,6,7]
initializeArrayWithRange(9, 0, 2); // [0,2,4,6,8]
```

</details>

<br>[⬆ Back to top](#contents)

### initializeArrayWithRangeRight
[待翻译]


初始化一个数组，该数组包含指定范围 `start` 到 `end` 内的数字（反向），可设置间隔 `step`。

使用 `array.from(Math.ceil((end+1-start)/step)` 来创建所需长度的数组(元素的数量等于 `(end-start)/step` 或 `(end+1-start)/step` ，包含结束数字)， 使用 `array.prototype.map()` 来填充范围中所需要的值。

```js
const initializeArrayWithRangeRight = (end, start = 0, step = 1) =>
  Array.from({ length: Math.ceil((end + 1 - start) / step) }).map(
    (v, i, arr) => (arr.length - i - 1) * step + start
  );
```

<details>
<summary>Examples</summary>

```js
initializeArrayWithRangeRight(5); // [5,4,3,2,1,0]
initializeArrayWithRangeRight(7, 3); // [7,6,5,4,3]
initializeArrayWithRangeRight(9, 0, 2); // [8,6,4,2,0]
```

</details>

<br>[⬆ Back to top](#contents)

### initializeArrayWithValues



使用指定的值初始化和填充数组。

使用 `Array(n)` 创建所需长度的数组，使用 `fill(v)` 填充所需的值。 你可以忽略 `val` ，使用默认值 `0`。


```js
const initializeArrayWithValues = (n, val = 0) => Array(n).fill(val);
```

<details>
<summary>Examples</summary>

```js
initializeArrayWithValues(5, 2); // [2, 2, 2, 2, 2]
```

</details>

<br>[⬆ Back to top](#contents)

### initializeNDArray



创建一个具有给定值的 `n` 维数组。

使用递归。
使用 `array.prototype.map()` 生成行，其中每个行都是使用 `initializeNDArray` 初始化的新数组。

```js
const initializeNDArray = (val, ...args) =>
  args.length === 0
    ? val
    : Array.from({ length: args[0] }).map(() => initializeNDArray(val, ...args.slice(1)));
```

<details>
<summary>Examples</summary>

```js
initializeNDArray(1, 3); // [1,1,1]
initializeNDArray(5, 2, 2, 2); // [[[5,5],[5,5]],[[5,5],[5,5]]]
```

</details>

<br>[⬆ Back to top](#contents)

### intersection



返回两个数组中都存在的元素列表。

根据数组 `b` 创建一个 `Set` 对象，然后在数组 `a` 上使用 `Array.prototype.filter()` 方法，只保留数组 `b` 中也包含的值。

```js
const intersection = (a, b) => {
  const s = new Set(b);
  return a.filter(x => s.has(x));
};
```

<details>
<summary>Examples</summary>

```js
intersection([1, 2, 3], [4, 3, 2]); // [2, 3]
```

</details>

<br>[⬆ Back to top](#contents)

### intersectionBy



将提供的函数应用于两个数组的每个数组元素后，返回两个数组中存在的元素列表。

将 `fn` 应用于 `b` 中的所有元素来创建 `Set` 对象 ，然后在 `a` 上使用 `Array.prototype.filter()`，只保留调用 `fn` 应用于每个元素后，同时在 `b` 中存在的元素。

```js
const intersectionBy = (a, b, fn) => {
  const s = new Set(b.map(fn));
  return a.filter(x => s.has(fn(x)));
};
```

<details>
<summary>Examples</summary>

```js
intersectionBy([2.1, 1.2], [2.3, 3.4], Math.floor); // [2.1]
```

</details>

<br>[⬆ Back to top](#contents)

### intersectionWith



使用提供的比较器（comparator）函数，返回两个数组中存在的元素列表。

使用 `Array.prototype.filter()` 和 `Array.prototype.findIndex()` 结合比较器（comparator）函数来确定交叉值。

```js
const intersectionWith = (a, b, comp) => a.filter(x => b.findIndex(y => comp(x, y)) !== -1);
```

<details>
<summary>Examples</summary>

```js
intersectionWith([1, 1.2, 1.5, 3, 0], [1.9, 3, 0, 3.9], (a, b) => Math.round(a) === Math.round(b)); // [1.5, 3, 0]
```

</details>

<br>[⬆ Back to top](#contents)

### isSorted



如果数组按升序排序，返回 `1` ;如果按降序排序，返回 `-1` ;如果没有排序，返回 `0` 。

计算前两个元素的顺序 `direction`。
使用 `Object.entries()` 对数组对象进行循环并对它们进行比较。
如果 `direction` 改变了，返回 `0`;如果循环直到最后一个元素，`direction` 没有改变，则返回 `direction`。

```js
const isSorted = arr => {
  let direction = -(arr[0] - arr[1]);
  for (let [i, val] of arr.entries()) {
    direction = !direction ? -(arr[i - 1] - arr[i]) : direction;
    if (i === arr.length - 1) return !direction ? 0 : direction;
    else if ((val - arr[i + 1]) * direction > 0) return 0;
  }
};
```

<details>
<summary>Examples</summary>

```js
isSorted([0, 1, 2, 2]); // 1
isSorted([4, 3, 2]); // -1
isSorted([4, 3, 5]); // 0
```

</details>

<br>[⬆ Back to top](#contents)

### join



将数组的所有元素拼接成一个字符串并返回此字符串。 使用分隔符和结束分隔符。

使用 `Array.prototype.reduce()` 将元素拼接成一个字符串。 省略第二个参数 `separator` ，则默认使用分隔符','。 省略第三个参数 `end` ，默认使用与 `separator` 相同的值。

```js
const join = (arr, separator = ',', end = separator) =>
  arr.reduce(
    (acc, val, i) =>
      i === arr.length - 2
        ? acc + val + end
        : i === arr.length - 1
          ? acc + val
          : acc + val + separator,
    ''
  );
```

<details>
<summary>Examples</summary>

```js
join(['pen', 'pineapple', 'apple', 'pen'], ',', '&'); // "pen,pineapple,apple&pen"
join(['pen', 'pineapple', 'apple', 'pen'], ','); // "pen,pineapple,apple,pen"
join(['pen', 'pineapple', 'apple', 'pen']); // "pen,pineapple,apple,pen"
```

</details>

<br>[⬆ Back to top](#contents)

### JSONtoCSV ![advanced](/advanced.svg)



将对象数组转换为仅包含指定的 `columns` 的逗号分隔值(CSV)字符串。

使用 `Array.prototype.join(delimiter)` 结合 `columns` 中的所有名称以创建第一行。
使用 `Array.prototype.map()` 和 `Array.prototype.reduce()` 为每个对象创建一行映射到 `columns` 中的值，用空字符串替换不存在的值。
使用 `Array.prototype.join('\n')` 将所有行组合成一个字符串。
省略第三个参数 `delimiter` ，使用 `,` 为默认的分隔符。

```js
const JSONtoCSV = (arr, columns, delimiter = ',') =>
  [
    columns.join(delimiter),
    ...arr.map(obj =>
      columns.reduce(
        (acc, key) => `${acc}${!acc.length ? '' : delimiter}"${!obj[key] ? '' : obj[key]}"`,
        ''
      )
    )
  ].join('\n');
```

<details>
<summary>Examples</summary>

```js
JSONtoCSV([{ a: 1, b: 2 }, { a: 3, b: 4, c: 5 }, { a: 6 }, { b: 7 }], ['a', 'b']); // 'a,b\n"1","2"\n"3","4"\n"6",""\n"","7"'
JSONtoCSV([{ a: 1, b: 2 }, { a: 3, b: 4, c: 5 }, { a: 6 }, { b: 7 }], ['a', 'b'], ';'); // 'a;b\n"1";"2"\n"3";"4"\n"6";""\n"";"7"'
```

</details>

<br>[⬆ Back to top](#contents)

### last



返回数组中的最后一个元素。

使用 `arr.length - 1` 来计算给定数组的最后一个元素的索引并返回。

```js
const last = arr => arr[arr.length - 1];
```

<details>
<summary>Examples</summary>

```js
last([1, 2, 3]); // 3
```

</details>

<br>[⬆ Back to top](#contents)

### longestItem



获取任何数量的可迭代对象或具有 `length` 属性的对象，并返回其中长度最长的一个。
如果多个对象具有相同的长度，则返回第一个对象。
如果没有提供参数，则返回 `undefined` 。

使用 `Array.prototype.reduce()` ，比较对象的 `length` 以找到长度最长的对象。

```js
const longestItem = (...vals) => vals.reduce((a, x) => (x.length > a.length ? x : a));
```

<details>
<summary>Examples</summary>

```js
longestItem('this', 'is', 'a', 'testcase'); // 'testcase'
longestItem(...['a', 'ab', 'abc']); // 'abc'
longestItem(...['a', 'ab', 'abc'], 'abcd'); // 'abcd'
longestItem([1, 2, 3], [1, 2], [1, 2, 3, 4, 5]); // [1, 2, 3, 4, 5]
longestItem([1, 2, 3], 'foobar'); // 'foobar'
```

</details>

<br>[⬆ Back to top](#contents)

### mapObject ![advanced](/advanced.svg)



使用一个函数将数组的值映射到对象，在键值对中，原始值作为键，映射值作为值。

使用一个匿名的内部函数作用域来声明一个 undefined 的内存空间，使用闭包来存储返回值。 使用一个新的 `Array` 来存储带有函数映射的数组和一个逗号运算符来返回第二个步骤，而不需要从一个上下文移动到另一个上下文（由于闭包和操作顺序）。

```js
const mapObject = (arr, fn) =>
  (a => (
    (a = [arr, arr.map(fn)]), a[0].reduce((acc, val, ind) => ((acc[val] = a[1][ind]), acc), {})
  ))();
```

<details>
<summary>Examples</summary>

```js
const squareIt = arr => mapObject(arr, a => a * a);
squareIt([1, 2, 3]); // { 1: 1, 2: 4, 3: 9 }
```

</details>

<br>[⬆ Back to top](#contents)

### maxN



从提供的数组中返回 `n` 个最大值元素。
如果 `n` 大于或等于提供的数组长度，则返回原始数组(按降序排列)。

使用 `array.prototype.sort()` 和 展开操作符 (`...`) 对数组进行浅克隆，并按降序排序。
使用 `Array.prototype.slice()` 获取指定数量的元素。
省略第二个参数 `n` ，获得只有一个元素的数组。

```js
const maxN = (arr, n = 1) => [...arr].sort((a, b) => b - a).slice(0, n);
```

<details>
<summary>Examples</summary>

```js
maxN([1, 2, 3]); // [3]
maxN([1, 2, 3], 2); // [3,2]
```

</details>

<br>[⬆ Back to top](#contents)

### minN



从提供的数组中返回 `n` 个最小值元素。
如果 `n` 大于或等于提供的数组长度，则返回原始数组(按升序排列)。

使用 `array.prototype.sort()` 和 展开操作符 (`...`) 对数组进行浅克隆，并按升序排序。
使用 `Array.prototype.slice()` 获取指定数量的元素。
省略第二个参数 `n` ，获得只有一个元素的数组。

```js
const minN = (arr, n = 1) => [...arr].sort((a, b) => a - b).slice(0, n);
```

<details>
<summary>Examples</summary>

```js
minN([1, 2, 3]); // [1]
minN([1, 2, 3], 2); // [1,2]
```

</details>

<br>[⬆ Back to top](#contents)

### none



如果提供的断言（predicate）函数处理集合中的所有元素都返回 `false` ，则返回 `true` ，否则返回 `false` 。

使用 `Array.prototype.some()` 测试集合中的任何元素是否基于 `fn` 返回 `true` 。
省略第二个参数 `fn` ，使用 `Boolean` 作为默认值。

```js
const none = (arr, fn = Boolean) => !arr.some(fn);
```

<details>
<summary>Examples</summary>

```js
none([0, 1, 3, 0], x => x == 2); // true
none([0, 0, 0]); // true
```

</details>

<br>[⬆ Back to top](#contents)

### nthElement



返回数组的第 `n` 个元素。

使用 `array .prototype.slice()` 首先获得一个包含第 n 个元素的数组。
如果索引超出界限，返回 `undefined` 。
省略第二个参数 `n` ，获得数组的第一个元素。

```js
const nthElement = (arr, n = 0) => (n === -1 ? arr.slice(n) : arr.slice(n, n + 1))[0];
```

<details>
<summary>Examples</summary>

```js
nthElement(['a', 'b', 'c'], 1); // 'b'
nthElement(['a', 'b', 'b'], -3); // 'a'
```

</details>

<br>[⬆ Back to top](#contents)

### offset



将指定数量的元素移动到数组的末尾。

两次使用 `Array.prototype.slice()` 来获取指定索引之后的元素和指定索引之前的元素。
使用展开操作符(`...`)将两个数组合成一个数组。
如果 `offset` 为负数，元素将从结束移动到开始位置。

```js
const offset = (arr, offset) => [...arr.slice(offset), ...arr.slice(0, offset)];
```

<details>
<summary>Examples</summary>

```js
offset([1, 2, 3, 4, 5], 2); // [3, 4, 5, 1, 2]
offset([1, 2, 3, 4, 5], -2); // [4, 5, 1, 2, 3]
```

</details>

<br>[⬆ Back to top](#contents)

### partition



根据提供的函数对每个元素进行迭代，将元素分组为两个数组。

使用 `array.prototype.reduce()` 创建一个由两个数组组成的数组。
使用 `array.prototype.push()` 将 `fn` 返回 `true` 的元素添加到第一个数组，而 `fn` 返回 `false` 的元素添加到第二个数组。

```js
const partition = (arr, fn) =>
  arr.reduce(
    (acc, val, i, arr) => {
      acc[fn(val, i, arr) ? 0 : 1].push(val);
      return acc;
    },
    [[], []]
  );
```

<details>
<summary>Examples</summary>

```js
const users = [{ user: 'barney', age: 36, active: false }, { user: 'fred', age: 40, active: true }];
partition(users, o => o.active); // [[{ 'user': 'fred',    'age': 40, 'active': true }],[{ 'user': 'barney',  'age': 36, 'active': false }]]
```

</details>

<br>[⬆ Back to top](#contents)

### permutations ![advanced](/advanced.svg)

⚠️ **WARNING**: This function's execution time increases exponentially with each array element. Anything more than 8 to 10 entries will cause your browser to hang as it tries to solve all the different combinations.

Generates all permutations of an array's elements (contains duplicates).

Use recursion.
For each element in the given array, create all the partial permutations for the rest of its elements.
Use `Array.prototype.map()` to combine the element with each partial permutation, then `Array.prototype.reduce()` to combine all permutations in one array.
Base cases are for array `length` equal to `2` or `1`.

```js
const permutations = arr => {
  if (arr.length <= 2) return arr.length === 2 ? [arr, [arr[1], arr[0]]] : arr;
  return arr.reduce(
    (acc, item, i) =>
      acc.concat(
        permutations([...arr.slice(0, i), ...arr.slice(i + 1)]).map(val => [item, ...val])
      ),
    []
  );
};
```

<details>
<summary>Examples</summary>

```js
permutations([1, 33, 5]); // [ [ 1, 33, 5 ], [ 1, 5, 33 ], [ 33, 1, 5 ], [ 33, 5, 1 ], [ 5, 1, 33 ], [ 5, 33, 1 ] ]
```

</details>

<br>[⬆ Back to top](#contents)

### pull



改变原始数组，过滤掉指定的值。

使用 `Array.prototype.filter()` 和 `array.prototype.include()` 过滤指定的值。
使用 `Array.prototype.length = 0` 通过将数组的长度重置为0来清空数组，并使用 `array.prototype.push()` 把提取的值重新填充数组。

_(对于不改变原始数组的代码片段，请参阅 [`without`](#without))_

```js
const pull = (arr, ...args) => {
  let argState = Array.isArray(args[0]) ? args[0] : args;
  let pulled = arr.filter((v, i) => !argState.includes(v));
  arr.length = 0;
  pulled.forEach(v => arr.push(v));
};
```

<details>
<summary>Examples</summary>

```js
let myArray = ['a', 'b', 'c', 'a', 'b', 'c'];
pull(myArray, 'a', 'c'); // myArray = [ 'b', 'b' ]
```

</details>

<br>[⬆ Back to top](#contents)

### pullAtIndex ![advanced](/advanced.svg)



改变原始数组，过滤掉指定索引的值。

使用 `Array.prototype.filter()` 和 `array.prototype.include()` 过滤指定的值。
使用 `Array.prototype.length = 0` 通过将数组的长度重置为0来清空数组，并使用 `array.prototype.push()` 把提取的值重新填充数组。
使用 `Array.prototype.push()` 跟踪提取的值。


```js
const pullAtIndex = (arr, pullArr) => {
  let removed = [];
  let pulled = arr
    .map((v, i) => (pullArr.includes(i) ? removed.push(v) : v))
    .filter((v, i) => !pullArr.includes(i));
  arr.length = 0;
  pulled.forEach(v => arr.push(v));
  return removed;
};
```

<details>
<summary>Examples</summary>

```js
let myArray = ['a', 'b', 'c', 'd'];
let pulled = pullAtIndex(myArray, [1, 3]); // myArray = [ 'a', 'c' ] , pulled = [ 'b', 'd' ]
```

</details>

<br>[⬆ Back to top](#contents)

### pullAtValue ![advanced](/advanced.svg)



修改原始数组，过滤掉指定的值。返回删除的元素。

使用 `Array.prototype.filter()` 和 `array.prototype.include()` 过滤指定的值。
使用 `Array.prototype.length = 0` 通过将数组的长度重置为0来清空数组，并使用 `array.prototype.push()` 把提取的值重新填充数组。
使用 `Array.prototype.push()` 跟踪提取的值。

```js
const pullAtValue = (arr, pullArr) => {
  let removed = [],
    pushToRemove = arr.forEach((v, i) => (pullArr.includes(v) ? removed.push(v) : v)),
    mutateTo = arr.filter((v, i) => !pullArr.includes(v));
  arr.length = 0;
  mutateTo.forEach(v => arr.push(v));
  return removed;
};
```

<details>
<summary>Examples</summary>

```js
let myArray = ['a', 'b', 'c', 'a', 'b', 'c'];
let pulled = pullAtValue(myArray, ['b', 'd']); // myArray = [ 'a', 'c' ] , pulled = [ 'b', 'd' ]
```

</details>

<br>[⬆ Back to top](#contents)

### pullBy ![advanced](/advanced.svg)




根据给定的迭代器（iterator）函数，修改原始数组，过滤掉指定的值。

检查函数中是否提供了最后一个参数。
使用 `array.prototype.map()` 将迭代器函数 `fn` 应用于所有数组元素。
使用 `Array.prototype.filter()` 和 `array.prototype.include()` 过滤指定的值。
使用 `Array.prototype.length = 0` 通过将数组的长度重置为0来清空数组，并使用 `array.prototype.push()` 把提取的值重新填充数组。

```js
const pullBy = (arr, ...args) => {
  const length = args.length;
  let fn = length > 1 ? args[length - 1] : undefined;
  fn = typeof fn == 'function' ? (args.pop(), fn) : undefined;
  let argState = (Array.isArray(args[0]) ? args[0] : args).map(val => fn(val));
  let pulled = arr.filter((v, i) => !argState.includes(fn(v)));
  arr.length = 0;
  pulled.forEach(v => arr.push(v));
};
```

<details>
<summary>Examples</summary>

```js
var myArray = [{ x: 1 }, { x: 2 }, { x: 3 }, { x: 1 }];
pullBy(myArray, [{ x: 1 }, { x: 3 }], o => o.x); // myArray = [{ x: 2 }]
```

</details>

<br>[⬆ Back to top](#contents)

### reducedFilter



根据条件过滤一个对象数组，同时过滤掉未指定的键。

使用 `array.prototype.filter()` 根据断言函数 `fn` 对数组进行过滤，返回条件为真值（truthy）的对象。
在经过过滤后的数组上，使用 `array.prototype.map()` 和 `array.prototype.reduce()` 过滤掉在 `keys` 参数中未提供的键。

```js
const reducedFilter = (data, keys, fn) =>
  data.filter(fn).map(el =>
    keys.reduce((acc, key) => {
      acc[key] = el[key];
      return acc;
    }, {})
  );
```

<details>
<summary>Examples</summary>

```js
const data = [
  {
    id: 1,
    name: 'john',
    age: 24
  },
  {
    id: 2,
    name: 'mike',
    age: 50
  }
];

reducedFilter(data, ['id', 'name'], item => item.age > 24); // [{ id: 2, name: 'mike'}]
```

</details>

<br>[⬆ Back to top](#contents)

### reduceSuccessive
【待翻译】


对数组中的每个元素（从左到右）都应用累加器（accumulator）函数，返回依次减少一个值的数组。

使用 `array.prototype.reduce()` 将给定函数应用于给定数组，存储每个得到的新结果。

```js
const reduceSuccessive = (arr, fn, acc) =>
  arr.reduce((res, val, i, arr) => (res.push(fn(res.slice(-1)[0], val, i, arr)), res), [acc]);
```

<details>
<summary>Examples</summary>

```js
reduceSuccessive([1, 2, 3, 4, 5, 6], (acc, val) => acc + val, 0); // [0, 1, 3, 6, 10, 15, 21]
```


</details>

<br>[⬆ Back to top](#contents)

### reduceWhich



将提供的函数设置比较规则后应用于数组，返回数组的最小/最大值。

使用 `array.prototype.reduce()` 结合 `comparator` 函数来获取数组中合适的元素。
您可以省略第二个参数 `comparator` ，默认返回数组中最小的元素。

```js
const reduceWhich = (arr, comparator = (a, b) => a - b) =>
  arr.reduce((a, b) => (comparator(a, b) >= 0 ? b : a));
```

<details>
<summary>Examples</summary>

```js
reduceWhich([1, 3, 2]); // 1
reduceWhich([1, 3, 2], (a, b) => b - a); // 3
reduceWhich(
  [{ name: 'Tom', age: 12 }, { name: 'Jack', age: 18 }, { name: 'Lucy', age: 9 }],
  (a, b) => a.age - b.age
); // {name: "Lucy", age: 9}
```

</details>

<br>[⬆ Back to top](#contents)

### reject



注：过滤掉符合断言函数条件的值

接受断言函数和数组，使用 `array .prototype.filter()` ，但仅当 `pred(x) === false` 时才保留 `x` 。

```js
const reject = (pred, array) => array.filter((...args) => !pred(...args));
```

<details>
<summary>Examples</summary>

```js
reject(x => x % 2 === 0, [1, 2, 3, 4, 5]); // [1, 3, 5]
reject(word => word.length > 4, ['Apple', 'Pear', 'Kiwi', 'Banana']); // ['Pear', 'Kiwi']
```

</details>

<br>[⬆ Back to top](#contents)

### remove



从数组中移除给定函数返回 `false` 的元素。

使用 `Array.prototype.filter()`  和 `Array.prototype.reduce()` 来查找数组中返回真值的元素，使用 `Array.prototype.splice()` 来移除元素。 `func` 有三个参数 (`value, index, array`)。

```js
const remove = (arr, func) =>
  Array.isArray(arr)
    ? arr.filter(func).reduce((acc, val) => {
      arr.splice(arr.indexOf(val), 1);
      return acc.concat(val);
    }, [])
    : [];
```

<details>
<summary>Examples</summary>

```js
remove([1, 2, 3, 4], n => n % 2 === 0); // [2, 4]
```

</details>

<br>[⬆ Back to top](#contents)

### sample



从数组中返回一个随机元素。

使用 `Math.random()` 生成随机数，将其乘以 `length` ，并使用 `Math.floor()` 将其四舍五入到最近的整数。
这个方法也适用于字符串。


```js
const sample = arr => arr[Math.floor(Math.random() * arr.length)];
```

<details>
<summary>Examples</summary>

```js
sample([3, 7, 9, 11]); // 9
```

</details>

<br>[⬆ Back to top](#contents)

### sampleSize



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

<details>
<summary>Examples</summary>

```js
sampleSize([1, 2, 3], 2); // [3,1]
sampleSize([1, 2, 3], 4); // [2,3,1]
```

</details>

<br>[⬆ Back to top](#contents)

### shank



具有与[`Array.prototype.splice()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice)相同的功能，但是 `Array.prototype.splice()` 返回一个新数组，而不是修改原始数组。

在删除现有元素 和/或 添加新元素之后，使用 `array.prototype.slice()` 和 `array.prototype.concat()` 获得一个包含新内容的新数组。
省略第二个参数 `index` ，下标从 `0` 开始。
省略第三个参数 `delCount` ，删除 `0` 个元素。
省略第四个参数 `elements` ，不添加任何新元素。

```js
const shank = (arr, index = 0, delCount = 0, ...elements) =>
  arr
    .slice(0, index)
    .concat(elements)
    .concat(arr.slice(index + delCount));
```

<details>
<summary>Examples</summary>

```js
const names = ['alpha', 'bravo', 'charlie'];
const namesAndDelta = shank(names, 1, 0, 'delta'); // [ 'alpha', 'delta', 'bravo', 'charlie' ]
const namesNoBravo = shank(names, 1, 1); // [ 'alpha', 'charlie' ]
console.log(names); // ['alpha', 'bravo', 'charlie']
```

</details>

<br>[⬆ Back to top](#contents)

### shuffle



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

<details>
<summary>Examples</summary>

```js
const foo = [1, 2, 3];
shuffle(foo); // [2, 3, 1], foo = [1, 2, 3]
```

</details>

<br>[⬆ Back to top](#contents)

### similarity



返回两个数组的交集。

使用 `Array.prototype.filter()` 移除不属于 `values` 中的值，这些值由 `array .prototype.include()` 来确定。

```js
const similarity = (arr, values) => arr.filter(v => values.includes(v));
```

<details>
<summary>Examples</summary>

```js
similarity([1, 2, 3], [1, 2, 4]); // [1, 2]
```

</details>

<br>[⬆ Back to top](#contents)

### sortedIndex



返回指定值插入到数组中的最小索引位置，以保持其排序顺序。

检查数组是否按降序（松散地）排序。 使用 `Array.prototype.findIndex()` 找到元素应该被插入的合适的索引位置。


```js
const sortedIndex = (arr, n) => {
  const isDescending = arr[0] > arr[arr.length - 1];
  const index = arr.findIndex(el => (isDescending ? n >= el : n <= el));
  return index === -1 ? arr.length : index;
};
```

<details>
<summary>Examples</summary>

```js
sortedIndex([5, 3, 2, 1], 4); // 1
sortedIndex([30, 50], 40); // 1
```

</details>

<br>[⬆ Back to top](#contents)

### sortedIndexBy



返回根据提供的迭代器函数，将指定值插入到数组中的最小索引位置，以保持其排序顺序。

检查数组是否按降序(松散地)排序。
使用 `Array.prototype.findIndex()` 根据迭代器函数 `fn` 查找应该插入元素的适当索引。

```js
const sortedIndexBy = (arr, n, fn) => {
  const isDescending = fn(arr[0]) > fn(arr[arr.length - 1]);
  const val = fn(n);
  const index = arr.findIndex(el => (isDescending ? val >= fn(el) : val <= fn(el)));
  return index === -1 ? arr.length : index;
};
```

<details>
<summary>Examples</summary>

```js
sortedIndexBy([{ x: 4 }, { x: 5 }], { x: 4 }, o => o.x); // 0
```

</details>

<br>[⬆ Back to top](#contents)

### sortedLastIndex



返回指定值插入到数组中的最大索引位置，以保持其排序顺序。

检查数组是否按降序(松散地)排序。
使用 `Array.prototype.reverse()` 和 ` Array.prototype.findIndex()` 查找应该插入元素的最后一个适当的索引。

```js
const sortedLastIndex = (arr, n) => {
  const isDescending = arr[0] > arr[arr.length - 1];
  const index = arr.reverse().findIndex(el => (isDescending ? n <= el : n >= el));
  return index === -1 ? 0 : arr.length - index;
};
```

<details>
<summary>Examples</summary>

```js
sortedLastIndex([10, 20, 30, 30, 40], 30); // 4
```

</details>

<br>[⬆ Back to top](#contents)

### sortedLastIndexBy



返回根据提供的迭代器函数，将指定值插入到数组中的最大索引位置，以保持其排序顺序。

检查数组是否按降序(松散地)排序。
使用 `array.prototype.map()` 将迭代器函数应用于数组的所有元素。
使用 `Array.prototype.reverse()` 和 ` Array.prototype.findIndex()` 根据提供的迭代器函数，查找应该插入元素的最后一个适当的索引。


```js
const sortedLastIndexBy = (arr, n, fn) => {
  const isDescending = fn(arr[0]) > fn(arr[arr.length - 1]);
  const val = fn(n);
  const index = arr
    .map(fn)
    .reverse()
    .findIndex(el => (isDescending ? val <= el : val >= el));
  return index === -1 ? 0 : arr.length - index;
};
```

<details>
<summary>Examples</summary>

```js
sortedLastIndexBy([{ x: 4 }, { x: 5 }], { x: 4 }, o => o.x); // 1
```

</details>

<br>[⬆ Back to top](#contents)

### stableSort ![advanced](/advanced.svg)



对数组执行稳定排序，值相同时保留其初始索引。
不改变原始数组，而是返回新数组。

使用 `array.prototype.map()` 将输入数组的每个元素与其对应的索引配对。
使用 `Array.prototype.sort()` 和 `compare` 函数对列表进行排序，如果比较的值相等，则保留它们的初始顺序。
使用 `array.prototype.map()` 将其转换回初始数组项。

```js
const stableSort = (arr, compare) =>
  arr
    .map((item, index) => ({ item, index }))
    .sort((a, b) => compare(a.item, b.item) || a.index - b.index)
    .map(({ item }) => item);
```

<details>
<summary>Examples</summary>

```js
const arr = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const stable = stableSort(arr, () => 0); // [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

</details>

<br>[⬆ Back to top](#contents)

### symmetricDifference



返回两个数组之间的差集，而不过滤重复的值。

根据每个数组创建一个 `Set` ，然后在每个数组上使用 `array.prototype.filter()` ，只保留不包含在另一个数组中的值。

```js
const symmetricDifference = (a, b) => {
  const sA = new Set(a),
    sB = new Set(b);
  return [...a.filter(x => !sB.has(x)), ...b.filter(x => !sA.has(x))];
};
```

<details>
<summary>Examples</summary>

```js
symmetricDifference([1, 2, 3], [1, 2, 4]); // [3, 4]
symmetricDifference([1, 2, 2], [1, 3, 1]); // [2, 2, 3]
```

</details>

<br>[⬆ Back to top](#contents)

### symmetricDifferenceBy



将提供的函数应用于两个数组的每个元素后，返回两个数组之间的差集。

根据每个数组创建一个 `Set` ，然后在每个数组上使用 `array.prototype.filter()` ，只保留不包含在另一个数组中的值。

```js
const symmetricDifferenceBy = (a, b, fn) => {
  const sA = new Set(a.map(v => fn(v))),
    sB = new Set(b.map(v => fn(v)));
  return [...a.filter(x => !sB.has(fn(x))), ...b.filter(x => !sA.has(fn(x)))];
};
```

<details>
<summary>Examples</summary>

```js
symmetricDifferenceBy([2.1, 1.2], [2.3, 3.4], Math.floor); // [ 1.2, 3.4 ]
```

</details>

<br>[⬆ Back to top](#contents)

### symmetricDifferenceWith



使用提供的函数作为比较器，返回两个数组之间的差集。

使用 `Array.prototype.filter()` 和 `Array.prototype.findIndex()` 查找合适的值。

```js
const symmetricDifferenceWith = (arr, val, comp) => [
  ...arr.filter(a => val.findIndex(b => comp(a, b)) === -1),
  ...val.filter(a => arr.findIndex(b => comp(a, b)) === -1)
];
```

<details>
<summary>Examples</summary>

```js
symmetricDifferenceWith(
  [1, 1.2, 1.5, 3, 0],
  [1.9, 3, 0, 3.9],
  (a, b) => Math.round(a) === Math.round(b)
); // [1, 1.2, 3.9]
```

</details>

<br>[⬆ Back to top](#contents)

### tail



返回数组中除第一个元素外的所有元素。

如果数组的 `length` 大于 `1`, ，则返回 `Array.prototype.slice(1)`，否则返回整个数组。

```js
const tail = arr => (arr.length > 1 ? arr.slice(1) : arr);
```

<details>
<summary>Examples</summary>

```js
tail([1, 2, 3]); // [2,3]
tail([1]); // [1]
```

</details>

<br>[⬆ Back to top](#contents)

### take



返回从开头开始提取 `n` 个元素的数组。

使用 `array.prototype.slice()` 创建数组的一个切片，其中包含从开头开始提取的 `n` 个元素。

```js
const take = (arr, n = 1) => arr.slice(0, n);
```

<details>
<summary>Examples</summary>

```js
take([1, 2, 3], 5); // [1, 2, 3]
take([1, 2, 3], 0); // []
```

</details>

<br>[⬆ Back to top](#contents)

### takeRight



返回从结尾开始向前提取 `n` 个元素的数组。

使用 `array.prototype.slice()` 创建数组的一个切片，其中包含从结尾开始向前提取的 `n` 个元素。

```js
const takeRight = (arr, n = 1) => arr.slice(arr.length - n, arr.length);
```

<details>
<summary>Examples</summary>

```js
takeRight([1, 2, 3], 2); // [ 2, 3 ]
takeRight([1, 2, 3]); // [3]
```

</details>

<br>[⬆ Back to top](#contents)

### takeRightWhile



从数组末尾移除元素，直到传递的函数返回“true”。返回删除的元素。

```js
const takeRightWhile = (arr, func) =>
  arr.reduceRight((acc, el) => (func(el) ? acc : [el, ...acc]), []);
```

<details>
<summary>Examples</summary>

```js
takeRightWhile([1, 2, 3, 4], n => n < 3); // [3, 4]
```

</details>

<br>[⬆ Back to top](#contents)

### takeWhile



从数组的开头开始删除数组中的元素，直到传递的函数返回 `true` 。返回删除的元素。

循环遍历数组，使用 `for...of` 循环 `Array.prototype.entries()` 拿到的值， 直到函数返回的值为 `true` 为止。
使用 `Array.prototype.slice()` 返回删除的元素。

```js
const takeWhile = (arr, func) => {
  for (const [i, val] of arr.entries()) if (func(val)) return arr.slice(0, i);
  return arr;
};
```

<details>
<summary>Examples</summary>

```js
takeWhile([1, 2, 3, 4], n => n >= 3); // [1, 2]
```

</details>

<br>[⬆ Back to top](#contents)

### toHash



将给定的类数组简化为值哈希（value hash）(有键的数据存储)。

给定一个可迭代的类数组结构，在提供的对象上调用 `Array.prototype.reduce.call()` 逐个处理元素，并返回一个对象，该对象由键引用一个值。

```js
const toHash = (object, key) =>
  Array.prototype.reduce.call(
    object,
    (acc, data, index) => ((acc[!key ? index : data[key]] = data), acc),
    {}
  );
```

<details>
<summary>Examples</summary>

```js
toHash([4, 3, 2, 1]); // { 0: 4, 1: 3, 2: 2, 3: 1 }
toHash([{ a: 'label' }], 'a'); // { label: { a: 'label' } }
// A more in depth example:
let users = [{ id: 1, first: 'Jon' }, { id: 2, first: 'Joe' }, { id: 3, first: 'Moe' }];
let managers = [{ manager: 1, employees: [2, 3] }];
// We use function here because we want a bindable reference, but a closure referencing the hash would work, too.
managers.forEach(
  manager =>
    (manager.employees = manager.employees.map(function(id) {
      return this[id];
    }, toHash(users, 'id')))
);
managers; // [ { manager:1, employees: [ { id: 2, first: "Joe" }, { id: 3, first: "Moe" } ] } ]
```

</details>

<br>[⬆ Back to top](#contents)

### union



返回两个数组的并集，相同的元素只出现一次。

基于 `a` 和 `b` 创建一个 `Set` 对象，返回转换后的数组。

```js
const union = (a, b) => Array.from(new Set([...a, ...b]));
```

<details>
<summary>Examples</summary>

```js
union([1, 2, 3], [4, 3, 2]); // [1,2,3,4]
```

</details>

<br>[⬆ Back to top](#contents)

### unionBy



将所提供的函数应用于两个数组的每个元素之后，返回两个数组的并集，相同的元素只出现一次。

在 `fn` 应用于 `a` 的所有元素后创建一个 `Set`，并在 `b` 中过滤已经在集合中存在的元素。
最后返回一个转换为数组的集合。

```js
const unionBy = (a, b, fn) => {
  const s = new Set(a.map(fn));
  return Array.from(new Set([...a, ...b.filter(x => !s.has(fn(x)))]));
};
```

<details>
<summary>Examples</summary>

```js
unionBy([2.1], [1.2, 2.3], Math.floor); // [2.1, 1.2]
```

</details>

<br>[⬆ Back to top](#contents)

### unionWith



使用提供的比较器函数，返回两个数组的并集，相同的元素只出现一次。

用 `Array.prototype.findIndex()` 使用提供的比较器函数后，在 `b` 中查找没有在 `a` 中匹配的值。

```js
const unionWith = (a, b, comp) =>
  Array.from(new Set([...a, ...b.filter(x => a.findIndex(y => comp(x, y)) === -1)]));
```

<details>
<summary>Examples</summary>

```js
unionWith([1, 1.2, 1.5, 3, 0], [1.9, 3, 0, 3.9], (a, b) => Math.round(a) === Math.round(b)); // [1, 1.2, 1.5, 3, 0, 3.9]
```

</details>

<br>[⬆ Back to top](#contents)

### uniqueElements



返回去重后的数组。

使用 ES6 的 `Set` 和 `...rest` 运算符去除所有重复的值。

```js
const uniqueElements = arr => [...new Set(arr)];
```

<details>
<summary>Examples</summary>

```js
uniqueElements([1, 2, 2, 3, 4, 4, 5]); // [1, 2, 3, 4, 5]
```

</details>

<br>[⬆ Back to top](#contents)

### uniqueElementsBy



根据提供的比较器函数，返回去重后的数组。

根据比较器函数 `fn`， 使用 `Array.prototype.reduce()` 和 `Array.prototype.some()` 去除重复的值，只保留重复值中第一个出现的值。
比较器（comparator）函数接受两个参数：正在比较的两个元素的值。

```js
const uniqueElementsBy = (arr, fn) =>
  arr.reduce((acc, v) => {
    if (!acc.some(x => fn(v, x))) acc.push(v);
    return acc;
  }, []);
```

<details>
<summary>Examples</summary>

```js
uniqueElementsBy(
  [
    { id: 0, value: 'a' },
    { id: 1, value: 'b' },
    { id: 2, value: 'c' },
    { id: 1, value: 'd' },
    { id: 0, value: 'e' }
  ],
  (a, b) => a.id == b.id
); // [ { id: 0, value: 'a' }, { id: 1, value: 'b' }, { id: 2, value: 'c' } ]
```

</details>

<br>[⬆ Back to top](#contents)

### uniqueElementsByRight



根据提供的比较器函数，从右边开始，返回去重后的数组。

根据比较器函数 `fn`， 从右边开始，使用 `Array.prototype.reduceRight()` 和 `Array.prototype.some()` 去除重复的值，只保留重复值中最后一个出现的值。
比较器（comparator）函数接受两个参数：正在比较的两个元素的值。

```js
const uniqueElementsByRight = (arr, fn) =>
  arr.reduceRight((acc, v) => {
    if (!acc.some(x => fn(v, x))) acc.push(v);
    return acc;
  }, []);
```

<details>
<summary>Examples</summary>

```js
uniqueElementsByRight(
  [
    { id: 0, value: 'a' },
    { id: 1, value: 'b' },
    { id: 2, value: 'c' },
    { id: 1, value: 'd' },
    { id: 0, value: 'e' }
  ],
  (a, b) => a.id == b.id
); // [ { id: 0, value: 'e' }, { id: 1, value: 'd' }, { id: 2, value: 'c' } ]
```

</details>

<br>[⬆ Back to top](#contents)

### uniqueSymmetricDifference



返回两个数组的差集，在两个数组中不重复的值。

在每个数组上使用 `array.prototype.filter()` 和 `array .prototype.include()` 来过滤另一个数组中包含的值，然后从结果中创建一个 `Set` ，删除重复的值。

```js
const uniqueSymmetricDifference = (a, b) => [
  ...new Set([...a.filter(v => !b.includes(v)), ...b.filter(v => !a.includes(v))])
];
```

<details>
<summary>Examples</summary>

```js
uniqueSymmetricDifference([1, 2, 3], [1, 2, 4]); // [3, 4]
uniqueSymmetricDifference([1, 2, 2], [1, 3, 1]); // [2, 3]
```

</details>

<br>[⬆ Back to top](#contents)

### unzip



创建一个数组，将 [zip](#zip) 生成的数组中的元素取消分组。

使用 `Math.max.apply()` 获取数组中最长子数组的长度，使用 `Array.prototype.map()` 生成最长长度个数组。
使用 `Array.prototype.reduce()` 和 `Array.prototype.forEach()` 将分组元素映射到对应的数组中。


```js
const unzip = arr =>
  arr.reduce(
    (acc, val) => (val.forEach((v, i) => acc[i].push(v)), acc),
    Array.from({
      length: Math.max(...arr.map(x => x.length))
    }).map(x => [])
  );
```

<details>
<summary>Examples</summary>

```js
unzip([['a', 1, true], ['b', 2, false]]); // [['a', 'b'], [1, 2], [true, false]]
unzip([['a', 1, true], ['b', 2]]); // [['a', 'b'], [1, 2], [true]]
```

</details>

<br>[⬆ Back to top](#contents)

### unzipWith ![advanced](/advanced.svg)



创建一个数组，将 [zip](#zip) 生成的数组中的元素取消分组，并结合提供的函数生成最后的结果。

使用 `Math.max.apply()` 获取数组中最长子数组的长度，使用 `Array.prototype.map()` 生成最长长度个数组。
使用 `Array.prototype.reduce()` 和 `Array.prototype.forEach()` 将分组元素映射到对应的数组中。
使用 `Array.prototype.map()` 和展开操作符 (`...`) 将 `fn` 应用于每一组元素。

```js
const unzipWith = (arr, fn) =>
  arr
    .reduce(
      (acc, val) => (val.forEach((v, i) => acc[i].push(v)), acc),
      Array.from({
        length: Math.max(...arr.map(x => x.length))
      }).map(x => [])
    )
    .map(val => fn(...val));
```

<details>
<summary>Examples</summary>

```js
unzipWith([[1, 10, 100], [2, 20, 200]], (...args) => args.reduce((acc, v) => acc + v, 0)); // [3, 30, 300]
```

</details>

<br>[⬆ Back to top](#contents)

### without



过滤掉数组中具有指定值之一的元素。

使用 `array.prototype.filter()` 创建一个数组，排除(使用 `!array.include()` )所有给定值。

_(改变原始数组，请看 [`pull`](#pull)) 代码片段_

```js
const without = (arr, ...args) => arr.filter(v => !args.includes(v));
```

<details>
<summary>Examples</summary>

```js
without([2, 1, 2, 3], 1, 2); // [3]
```

</details>

<br>[⬆ Back to top](#contents)

### xProd



将两个数组的每个元素两两进行组合，组合出所有的可能对存在数组中，返回一个存在所有可能性对的数组。

使用 `Array.prototype.reduce()`, `Array.prototype.map()` 和 `Array.prototype.concat()` 从两个数组的元素中生成所有可能的对，并将它们保存在一个数组中。

```js
const xProd = (a, b) => a.reduce((acc, x) => acc.concat(b.map(y => [x, y])), []);
```

<details>
<summary>Examples</summary>

```js
xProd([1, 2], ['a', 'b']); // [[1, 'a'], [1, 'b'], [2, 'a'], [2, 'b']]
```

</details>

<br>[⬆ Back to top](#contents)

### zip



创建一个根据原始数组中的位置进行分组的数组。

使用 `Math.max.apply()` 获取参数中最长的数组，创建一个长度为该长度的数组，并使用`Array.from()`  和映射函数（map-function） 来创建一个分组元素数组。 如果参数数组的长度不同，则在未找到值的情况下使用 `undefined` 。

```js
const zip = (...arrays) => {
  const maxLength = Math.max(...arrays.map(x => x.length));
  return Array.from({ length: maxLength }).map((_, i) => {
    return Array.from({ length: arrays.length }, (_, k) => arrays[k][i]);
  });
};
```

<details>
<summary>Examples</summary>

```js
zip(['a', 'b'], [1, 2], [true, false]); // [['a', 1, true], ['b', 2, false]]
zip(['a'], [1, 2], [true, false]); // [['a', 1, true], [undefined, 2, false]]
```

</details>

<br>[⬆ Back to top](#contents)

### zipObject



给定一个有效属性标识符数组和一个值数组，返回一个将属性关联到值的对象。

由于对象可以有未定义的值，但不能有未定义的属性名，所以属性数组使用 `array.prototype.reduce()` 来决定结果对象的结构。

```js
const zipObject = (props, values) =>
  props.reduce((obj, prop, index) => ((obj[prop] = values[index]), obj), {});
```

<details>
<summary>Examples</summary>

```js
zipObject(['a', 'b', 'c'], [1, 2]); // {a: 1, b: 2, c: undefined}
zipObject(['a', 'b'], [1, 2, 3]); // {a: 1, b: 2}
```

</details>

<br>[⬆ Back to top](#contents)

### zipWith ![advanced](/advanced.svg)



创建一个根据原始数组中的位置进行分组的数组，并使用函数作为最后一个参数来指定应如何组合分组中的值。

检查最后提供的参数是否为函数。
使用 `Math.max.apply()` 获取参数中最长的数组，创建一个长度为该长度的数组，并使用`Array.from()`  和映射函数（map-function） 来创建一个分组元素数组。 
如果参数数组的长度不同，则在找不到值的地方使用“undefined”。
最后一个参数提供的函数应用于每个组 `(...group)` 的元素。


```js
const zipWith = (...array) => {
  const fn = typeof array[array.length - 1] === 'function' ? array.pop() : undefined;
  return Array.from(
    { length: Math.max(...array.map(a => a.length)) },
    (_, i) => (fn ? fn(...array.map(a => a[i])) : array.map(a => a[i]))
  );
};
```

<details>
<summary>Examples</summary>

```js
zipWith([1, 2], [10, 20], [100, 200], (a, b, c) => a + b + c); // [111,222]
zipWith(
  [1, 2, 3],
  [10, 20],
  [100, 200],
  (a, b, c) => (a != null ? a : 'a') + (b != null ? b : 'b') + (c != null ? c : 'c')
); // [111, 222, '3bc']
```

</details>

<br>[⬆ Back to top](#contents)


---

## 🌐 Browser

### arrayToHtmlList



将给定的数组元素转换为 `<li>` 标签，并将它们添加到给定 id 的列表中。

使用 `Array.prototype.map()` 、`document.querySelector()` 和内部闭包创建 `html` 标签列表。

```js
const arrayToHtmlList = (arr, listID) =>
  (el => (
    (el = document.querySelector('#' + listID)),
    (el.innerHTML += arr.map(item => `<li>${item}</li>`).join(''))
  ))();
```

<details>
<summary>Examples</summary>

```js
arrayToHtmlList(['item 1', 'item 2'], 'myListID');
```

</details>

<br>[⬆ Back to top](#contents)

### bottomVisible



如果页面底部可见，返回 `true`，否则返回 `false`。
使用 `scrollY`, `scrollHeight` 和 `clientHeight` 来判断页面的底部是否可见。

```js
const bottomVisible = () =>
  document.documentElement.clientHeight + window.scrollY >=
  (document.documentElement.scrollHeight || document.documentElement.clientHeight);
```

<details>
<summary>Examples</summary>

```js
bottomVisible(); // true
```

</details>

<br>[⬆ Back to top](#contents)

### copyToClipboard ![advanced](/advanced.svg)

⚠️ **NOTICE:** The same functionality can be easily implemented by using the new asynchronous Clipboard API, which is still experimental but should be used in the future instead of this snippet. Find out more about it [here](https://github.com/w3c/clipboard-apis/blob/master/explainer.adoc#writing-to-the-clipboard).

Copy a string to the clipboard. 
Only works as a result of user action (i.e. inside a `click` event listener).

Create a new `<textarea>` element, fill it with the supplied data and add it to the HTML document.
Use `Selection.getRangeAt()`to store the selected range (if any).
Use `document.execCommand('copy')` to copy to the clipboard.
Remove the `<textarea>` element from the HTML document.
Finally, use `Selection().addRange()` to recover the original selected range (if any).

```js
const copyToClipboard = str => {
  const el = document.createElement('textarea');
  el.value = str;
  el.setAttribute('readonly', '');
  el.style.position = 'absolute';
  el.style.left = '-9999px';
  document.body.appendChild(el);
  const selected =
    document.getSelection().rangeCount > 0 ? document.getSelection().getRangeAt(0) : false;
  el.select();
  document.execCommand('copy');
  document.body.removeChild(el);
  if (selected) {
    document.getSelection().removeAllRanges();
    document.getSelection().addRange(selected);
  }
};
```

<details>
<summary>Examples</summary>

```js
copyToClipboard('Lorem ipsum'); // 'Lorem ipsum' copied to clipboard.
```

</details>

<br>[⬆ Back to top](#contents)

### counter ![advanced](/advanced.svg)

Creates a counter with the specified range, step and duration for the specified selector.

Check if `step` has the proper sign and change it accordingly.
Use `setInterval()` in combination with `Math.abs()` and `Math.floor()` to calculate the time between each new text draw.
Use `document.querySelector().innerHTML` to update the value of the selected element.
Omit the fourth parameter, `step`, to use a default step of `1`.
Omit the fifth parameter, `duration`, to use a default duration of `2000`ms.

```js
const counter = (selector, start, end, step = 1, duration = 2000) => {
  let current = start,
    _step = (end - start) * step < 0 ? -step : step,
    timer = setInterval(() => {
      current += _step;
      document.querySelector(selector).innerHTML = current;
      if (current >= end) document.querySelector(selector).innerHTML = end;
      if (current >= end) clearInterval(timer);
    }, Math.abs(Math.floor(duration / (end - start))));
  return timer;
};
```

<details>
<summary>Examples</summary>

```js
counter('#my-id', 1, 1000, 5, 2000); // Creates a 2-second timer for the element with id="my-id"
```

</details>

<br>[⬆ Back to top](#contents)

### createElement

Creates an element from a string (without appending it to the document). 
If the given string contains multiple elements, only the first one will be returned.

Use `document.createElement()` to create a new element.
Set its `innerHTML` to the string supplied as the argument. 
Use `ParentNode.firstElementChild` to return the element version of the string.

```js
const createElement = str => {
  const el = document.createElement('div');
  el.innerHTML = str;
  return el.firstElementChild;
};
```

<details>
<summary>Examples</summary>

```js
const el = createElement(
  `<div class="container">
    <p>Hello!</p>
  </div>`
);
console.log(el.className); // 'container'
```

</details>

<br>[⬆ Back to top](#contents)

### createEventHub ![advanced](/advanced.svg)

Creates a pub/sub ([publish–subscribe](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern)) event hub with `emit`, `on`, and `off` methods.

Use `Object.create(null)` to create an empty `hub` object that does not inherit properties from `Object.prototype`.
For `emit`, resolve the array of handlers based on the `event` argument and then run each one with `Array.prototype.forEach()` by passing in the data as an argument.
For `on`, create an array for the event if it does not yet exist, then use `Array.prototype.push()` to add the handler
to the array.
For `off`, use `Array.prototype.findIndex()` to find the index of the handler in the event array and remove it using `Array.prototype.splice()`.

```js
const createEventHub = () => ({
  hub: Object.create(null),
  emit(event, data) {
    (this.hub[event] || []).forEach(handler => handler(data));
  },
  on(event, handler) {
    if (!this.hub[event]) this.hub[event] = [];
    this.hub[event].push(handler);
  },
  off(event, handler) {
    const i = (this.hub[event] || []).findIndex(h => h === handler);
    if (i > -1) this.hub[event].splice(i, 1);
    if (this.hub[event].length === 0) delete this.hub[event];
  }
});
```

<details>
<summary>Examples</summary>

```js
const handler = data => console.log(data);
const hub = createEventHub();
let increment = 0;

// Subscribe: listen for different types of events
hub.on('message', handler);
hub.on('message', () => console.log('Message event fired'));
hub.on('increment', () => increment++);

// Publish: emit events to invoke all handlers subscribed to them, passing the data to them as an argument
hub.emit('message', 'hello world'); // logs 'hello world' and 'Message event fired'
hub.emit('message', { hello: 'world' }); // logs the object and 'Message event fired'
hub.emit('increment'); // `increment` variable is now 1

// Unsubscribe: stop a specific handler from listening to the 'message' event
hub.off('message', handler);
```

</details>

<br>[⬆ Back to top](#contents)

### currentURL

Returns the current URL.

Use `window.location.href` to get current URL.

```js
const currentURL = () => window.location.href;
```

<details>
<summary>Examples</summary>

```js
currentURL(); // 'https://google.com'
```

</details>

<br>[⬆ Back to top](#contents)

### detectDeviceType

Detects whether the website is being opened in a mobile device or a desktop/laptop.

Use a regular expression to test the `navigator.userAgent` property to figure out if the device is a mobile device or a desktop/laptop.

```js
const detectDeviceType = () =>
  /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent)
    ? 'Mobile'
    : 'Desktop';
```

<details>
<summary>Examples</summary>

```js
detectDeviceType(); // "Mobile" or "Desktop"
```

</details>

<br>[⬆ Back to top](#contents)

### elementContains

Returns `true` if the `parent` element contains the `child` element, `false` otherwise.

Check that `parent` is not the same element as `child`, use `parent.contains(child)` to check if the `parent` element contains the `child` element.

```js
const elementContains = (parent, child) => parent !== child && parent.contains(child);
```

<details>
<summary>Examples</summary>

```js
elementContains(document.querySelector('head'), document.querySelector('title')); // true
elementContains(document.querySelector('body'), document.querySelector('body')); // false
```

</details>

<br>[⬆ Back to top](#contents)

### elementIsVisibleInViewport ![advanced](/advanced.svg)

Returns `true` if the element specified is visible in the viewport, `false` otherwise.

Use `Element.getBoundingClientRect()` and the `window.inner(Width|Height)` values
to determine if a given element is visible in the viewport.
Omit the second argument to determine if the element is entirely visible, or specify `true` to determine if
it is partially visible.

```js
const elementIsVisibleInViewport = (el, partiallyVisible = false) => {
  const { top, left, bottom, right } = el.getBoundingClientRect();
  const { innerHeight, innerWidth } = window;
  return partiallyVisible
    ? ((top > 0 && top < innerHeight) || (bottom > 0 && bottom < innerHeight)) &&
        ((left > 0 && left < innerWidth) || (right > 0 && right < innerWidth))
    : top >= 0 && left >= 0 && bottom <= innerHeight && right <= innerWidth;
};
```

<details>
<summary>Examples</summary>

```js
// e.g. 100x100 viewport and a 10x10px element at position {top: -1, left: 0, bottom: 9, right: 10}
elementIsVisibleInViewport(el); // false - (not fully visible)
elementIsVisibleInViewport(el, true); // true - (partially visible)
```

</details>

<br>[⬆ Back to top](#contents)

### formToObject

Encode a set of form elements as an `object`.

Use the `FormData` constructor to convert the HTML `form` to `FormData`, `Array.from()` to convert to an array.
Collect the object from the array, using `Array.prototype.reduce()`.

```js
const formToObject = form =>
  Array.from(new FormData(form)).reduce(
    (acc, [key, value]) => ({
      ...acc,
      [key]: value
    }),
    {}
  );
```

<details>
<summary>Examples</summary>

```js
formToObject(document.querySelector('#form')); // { email: 'test@email.com', name: 'Test Name' }
```

</details>

<br>[⬆ Back to top](#contents)

### getImages

Fetches all images from within an element and puts them into an array

Use `Element.prototype.getElementsByTagName()` to fetch all `<img>` elements inside the provided element, `Array.prototype.map()` to map every `src` attribute of their respective `<img>` element, then create a `Set` to eliminate duplicates and return the array.

```js
const getImages = (el, includeDuplicates = false) => {
  const images = [...el.getElementsByTagName('img')].map(img => img.getAttribute('src'));
  return includeDuplicates ? images : [...new Set(images)];
};
```

<details>
<summary>Examples</summary>

```js
getImages(document, true); // ['image1.jpg', 'image2.png', 'image1.png', '...']
getImages(document, false); // ['image1.jpg', 'image2.png', '...']
```

</details>

<br>[⬆ Back to top](#contents)

### getScrollPosition

Returns the scroll position of the current page.

Use `pageXOffset` and `pageYOffset` if they are defined, otherwise `scrollLeft` and `scrollTop`.
You can omit `el` to use a default value of `window`.

```js
const getScrollPosition = (el = window) => ({
  x: el.pageXOffset !== undefined ? el.pageXOffset : el.scrollLeft,
  y: el.pageYOffset !== undefined ? el.pageYOffset : el.scrollTop
});
```

<details>
<summary>Examples</summary>

```js
getScrollPosition(); // {x: 0, y: 200}
```

</details>

<br>[⬆ Back to top](#contents)

### getStyle

Returns the value of a CSS rule for the specified element.

Use `Window.getComputedStyle()` to get the value of the CSS rule for the specified element.

```js
const getStyle = (el, ruleName) => getComputedStyle(el)[ruleName];
```

<details>
<summary>Examples</summary>

```js
getStyle(document.querySelector('p'), 'font-size'); // '16px'
```

</details>

<br>[⬆ Back to top](#contents)

### hasClass

Returns `true` if the element has the specified class, `false` otherwise.

Use `element.classList.contains()` to check if the element has the specified class.

```js
const hasClass = (el, className) => el.classList.contains(className);
```

<details>
<summary>Examples</summary>

```js
hasClass(document.querySelector('p.special'), 'special'); // true
```

</details>

<br>[⬆ Back to top](#contents)

### hashBrowser ![advanced](/advanced.svg)

Creates a hash for a value using the [SHA-256](https://en.wikipedia.org/wiki/SHA-2) algorithm. Returns a promise.

Use the [SubtleCrypto](https://developer.mozilla.org/en-US/docs/Web/API/SubtleCrypto) API to create a hash for the given value.

```js
const hashBrowser = val =>
  crypto.subtle.digest('SHA-256', new TextEncoder('utf-8').encode(val)).then(h => {
    let hexes = [],
      view = new DataView(h);
    for (let i = 0; i < view.byteLength; i += 4)
      hexes.push(('00000000' + view.getUint32(i).toString(16)).slice(-8));
    return hexes.join('');
  });
```

<details>
<summary>Examples</summary>

```js
hashBrowser(JSON.stringify({ a: 'a', b: [1, 2, 3, 4], foo: { c: 'bar' } })).then(console.log); // '04aa106279f5977f59f9067fa9712afc4aedc6f5862a8defc34552d8c7206393'
```

</details>

<br>[⬆ Back to top](#contents)

### hide

Hides all the elements specified.

Use `NodeList.prototype.forEach()` to apply `display: none` to each element specified.

```js
const hide = (...el) => [...el].forEach(e => (e.style.display = 'none'));
```

<details>
<summary>Examples</summary>

```js
hide(document.querySelectorAll('img')); // Hides all <img> elements on the page
```

</details>

<br>[⬆ Back to top](#contents)

### httpsRedirect

Redirects the page to HTTPS if its currently in HTTP. Also, pressing the back button doesn't take it back to the HTTP page as its replaced in the history.

Use `location.protocol` to get the protocol currently being used. If it's not HTTPS, use `location.replace()` to replace the existing page with the HTTPS version of the page. Use `location.href` to get the full address, split it with `String.prototype.split()` and remove the protocol part of the URL.

```js
const httpsRedirect = () => {
  if (location.protocol !== 'https:') location.replace('https://' + location.href.split('//')[1]);
};
```

<details>
<summary>Examples</summary>

```js
httpsRedirect(); // If you are on http://mydomain.com, you are redirected to https://mydomain.com
```

</details>

<br>[⬆ Back to top](#contents)

### insertAfter

Inserts an HTML string after the end of the specified element.

Use `el.insertAdjacentHTML()` with a position of `'afterend'` to parse `htmlString` and insert it after the end of `el`.

```js
const insertAfter = (el, htmlString) => el.insertAdjacentHTML('afterend', htmlString);
```

<details>
<summary>Examples</summary>

```js
insertAfter(document.getElementById('myId'), '<p>after</p>'); // <div id="myId">...</div> <p>after</p>
```

</details>

<br>[⬆ Back to top](#contents)

### insertBefore

Inserts an HTML string before the start of the specified element.

Use `el.insertAdjacentHTML()` with a position of `'beforebegin'` to parse `htmlString` and insert it before the start of `el`.

```js
const insertBefore = (el, htmlString) => el.insertAdjacentHTML('beforebegin', htmlString);
```

<details>
<summary>Examples</summary>

```js
insertBefore(document.getElementById('myId'), '<p>before</p>'); // <p>before</p> <div id="myId">...</div>
```

</details>

<br>[⬆ Back to top](#contents)

### isBrowserTabFocused

Returns `true` if the browser tab of the page is focused, `false` otherwise.

Use the `Document.hidden` property, introduced by the Page Visibility API to check if the browser tab of the page is visible or hidden.

```js
const isBrowserTabFocused = () => !document.hidden;
```

<details>
<summary>Examples</summary>

```js
isBrowserTabFocused(); // true
```

</details>

<br>[⬆ Back to top](#contents)

### nodeListToArray

Converts a `NodeList` to an array.

Use spread operator inside new array to convert a `NodeList` to an array.

```js
const nodeListToArray = nodeList => [...nodeList];
```

<details>
<summary>Examples</summary>

```js
nodeListToArray(document.childNodes); // [ <!DOCTYPE html>, html ]
```

</details>

<br>[⬆ Back to top](#contents)

### observeMutations ![advanced](/advanced.svg)

Returns a new MutationObserver and runs the provided callback for each mutation on the specified element.

Use a [`MutationObserver`](https://developer.mozilla.org/en-US/docs/Web/API/MutationObserver) to observe mutations on the given element.
Use `Array.prototype.forEach()` to run the callback for each mutation that is observed.
Omit the third argument, `options`, to use the default [options](https://developer.mozilla.org/en-US/docs/Web/API/MutationObserver#MutationObserverInit) (all `true`).

```js
const observeMutations = (element, callback, options) => {
  const observer = new MutationObserver(mutations => mutations.forEach(m => callback(m)));
  observer.observe(
    element,
    Object.assign(
      {
        childList: true,
        attributes: true,
        attributeOldValue: true,
        characterData: true,
        characterDataOldValue: true,
        subtree: true
      },
      options
    )
  );
  return observer;
};
```

<details>
<summary>Examples</summary>

```js
const obs = observeMutations(document, console.log); // Logs all mutations that happen on the page
obs.disconnect(); // Disconnects the observer and stops logging mutations on the page
```

</details>

<br>[⬆ Back to top](#contents)

### off

Removes an event listener from an element.

Use `EventTarget.removeEventListener()` to remove an event listener from an element. 
Omit the fourth argument `opts` to use `false` or specify it based on the options used when the event listener was added.

```js
const off = (el, evt, fn, opts = false) => el.removeEventListener(evt, fn, opts);
```

<details>
<summary>Examples</summary>

```js
const fn = () => console.log('!');
document.body.addEventListener('click', fn);
off(document.body, 'click', fn); // no longer logs '!' upon clicking on the page
```

</details>

<br>[⬆ Back to top](#contents)

### on

Adds an event listener to an element with the ability to use event delegation.

Use `EventTarget.addEventListener()` to add an event listener to an element. If there is a `target` property supplied to the options object, ensure the event target matches the target specified and then invoke the callback by supplying the correct `this` context.
Returns a reference to the custom delegator function, in order to be possible to use with [`off`](#off).
Omit `opts` to default to non-delegation behavior and event bubbling.

```js
const on = (el, evt, fn, opts = {}) => {
  const delegatorFn = e => e.target.matches(opts.target) && fn.call(e.target, e);
  el.addEventListener(evt, opts.target ? delegatorFn : fn, opts.options || false);
  if (opts.target) return delegatorFn;
};
```

<details>
<summary>Examples</summary>

```js
const fn = () => console.log('!');
on(document.body, 'click', fn); // logs '!' upon clicking the body
on(document.body, 'click', fn, { target: 'p' }); // logs '!' upon clicking a `p` element child of the body
on(document.body, 'click', fn, { options: true }); // use capturing instead of bubbling
```

</details>

<br>[⬆ Back to top](#contents)

### onUserInputChange ![advanced](/advanced.svg)

Run the callback whenever the user input type changes (`mouse` or `touch`). Useful for enabling/disabling code depending on the input device. This process is dynamic and works with hybrid devices (e.g. touchscreen laptops).

Use two event listeners. Assume `mouse` input initially and bind a `touchstart` event listener to the document. 
On `touchstart`, add a `mousemove` event listener to listen for two consecutive `mousemove` events firing within 20ms, using `performance.now()`.
Run the callback with the input type as an argument in either of these situations.

```js
const onUserInputChange = callback => {
  let type = 'mouse',
    lastTime = 0;
  const mousemoveHandler = () => {
    const now = performance.now();
    if (now - lastTime < 20)
      (type = 'mouse'), callback(type), document.removeEventListener('mousemove', mousemoveHandler);
    lastTime = now;
  };
  document.addEventListener('touchstart', () => {
    if (type === 'touch') return;
    (type = 'touch'), callback(type), document.addEventListener('mousemove', mousemoveHandler);
  });
};
```

<details>
<summary>Examples</summary>

```js
onUserInputChange(type => {
  console.log('The user is now using', type, 'as an input method.');
});
```

</details>

<br>[⬆ Back to top](#contents)

### prefix

Returns the prefixed version (if necessary) of a CSS property that the browser supports.

Use `Array.prototype.findIndex()` on an array of vendor prefix strings to test if `document.body` has one of them defined in its `CSSStyleDeclaration` object, otherwise return `null`.
Use `String.prototype.charAt()` and `String.prototype.toUpperCase()` to capitalize the property, which will be appended to the vendor prefix string.

```js
const prefix = prop => {
  const capitalizedProp = prop.charAt(0).toUpperCase() + prop.slice(1);
  const prefixes = ['', 'webkit', 'moz', 'ms', 'o'];
  const i = prefixes.findIndex(
    prefix => typeof document.body.style[prefix ? prefix + capitalizedProp : prop] !== 'undefined'
  );
  return i !== -1 ? (i === 0 ? prop : prefixes[i] + capitalizedProp) : null;
};
```

<details>
<summary>Examples</summary>

```js
prefix('appearance'); // 'appearance' on a supported browser, otherwise 'webkitAppearance', 'mozAppearance', 'msAppearance' or 'oAppearance'
```

</details>

<br>[⬆ Back to top](#contents)

### recordAnimationFrames

Invokes the provided callback on each animation frame.

Use recursion. 
Provided that `running` is `true`, continue invoking `window.requestAnimationFrame()` which invokes the provided callback. 
Return an object with two methods `start` and `stop` to allow manual control of the recording. 
Omit the second argument, `autoStart`, to implicitly call `start` when the function is invoked.

```js
const recordAnimationFrames = (callback, autoStart = true) => {
  let running = true,
    raf;
  const stop = () => {
    running = false;
    cancelAnimationFrame(raf);
  };
  const start = () => {
    running = true;
    run();
  };
  const run = () => {
    raf = requestAnimationFrame(() => {
      callback();
      if (running) run();
    });
  };
  if (autoStart) start();
  return { start, stop };
};
```

<details>
<summary>Examples</summary>

```js
const cb = () => console.log('Animation frame fired');
const recorder = recordAnimationFrames(cb); // logs 'Animation frame fired' on each animation frame
recorder.stop(); // stops logging
recorder.start(); // starts again
const recorder2 = recordAnimationFrames(cb, false); // `start` needs to be explicitly called to begin recording frames
```

</details>

<br>[⬆ Back to top](#contents)

### redirect

Redirects to a specified URL.

Use `window.location.href` or `window.location.replace()` to redirect to `url`.
Pass a second argument to simulate a link click (`true` - default) or an HTTP redirect (`false`).

```js
const redirect = (url, asLink = true) =>
  asLink ? (window.location.href = url) : window.location.replace(url);
```

<details>
<summary>Examples</summary>

```js
redirect('https://google.com');
```

</details>

<br>[⬆ Back to top](#contents)

### runAsync ![advanced](/advanced.svg)

Runs a function in a separate thread by using a [Web Worker](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers), allowing long running functions to not block the UI.

Create a new `Worker` using a `Blob` object URL, the contents of which should be the stringified version of the supplied function.
Immediately post the return value of calling the function back.
Return a promise, listening for `onmessage` and `onerror` events and resolving the data posted back from the worker, or throwing an error.

```js
const runAsync = fn => {
  const worker = new Worker(
    URL.createObjectURL(new Blob([`postMessage((${fn})());`]), {
      type: 'application/javascript; charset=utf-8'
    })
  );
  return new Promise((res, rej) => {
    worker.onmessage = ({ data }) => {
      res(data), worker.terminate();
    };
    worker.onerror = err => {
      rej(err), worker.terminate();
    };
  });
};
```

<details>
<summary>Examples</summary>

```js
const longRunningFunction = () => {
  let result = 0;
  for (let i = 0; i < 1000; i++)
    for (let j = 0; j < 700; j++) for (let k = 0; k < 300; k++) result = result + i + j + k;

  return result;
};
/*
  NOTE: Since the function is running in a different context, closures are not supported.
  The function supplied to `runAsync` gets stringified, so everything becomes literal.
  All variables and functions must be defined inside.
*/
runAsync(longRunningFunction).then(console.log); // 209685000000
runAsync(() => 10 ** 3).then(console.log); // 1000
let outsideVariable = 50;
runAsync(() => typeof outsideVariable).then(console.log); // 'undefined'
```

</details>

<br>[⬆ Back to top](#contents)

### scrollToTop

Smooth-scrolls to the top of the page.

Get distance from top using `document.documentElement.scrollTop` or `document.body.scrollTop`.
Scroll by a fraction of the distance from the top. Use `window.requestAnimationFrame()` to animate the scrolling.

```js
const scrollToTop = () => {
  const c = document.documentElement.scrollTop || document.body.scrollTop;
  if (c > 0) {
    window.requestAnimationFrame(scrollToTop);
    window.scrollTo(0, c - c / 8);
  }
};
```

<details>
<summary>Examples</summary>

```js
scrollToTop();
```

</details>

<br>[⬆ Back to top](#contents)

### serializeForm

Encode a set of form elements as a query string.

Use the `FormData` constructor to convert the HTML `form` to `FormData`, `Array.from()` to convert to an array, passing a map function as the second argument.
Use `Array.prototype.map()` and `window.encodeURIComponent()` to encode each field's value.
Use `Array.prototype.join()` with appropriate argumens to produce an appropriate query string.

```js
const serializeForm = form =>
  Array.from(new FormData(form), field => field.map(encodeURIComponent).join('=')).join('&');
```

<details>
<summary>Examples</summary>

```js
serializeForm(document.querySelector('#form')); // email=test%40email.com&name=Test%20Name
```

</details>

<br>[⬆ Back to top](#contents)

### setStyle

Sets the value of a CSS rule for the specified element.

Use `element.style` to set the value of the CSS rule for the specified element to `val`.

```js
const setStyle = (el, ruleName, val) => (el.style[ruleName] = val);
```

<details>
<summary>Examples</summary>

```js
setStyle(document.querySelector('p'), 'font-size', '20px'); // The first <p> element on the page will have a font-size of 20px
```

</details>

<br>[⬆ Back to top](#contents)

### show

Shows all the elements specified.

Use the spread operator (`...`) and `Array.prototype.forEach()` to clear the `display` property for each element specified.

```js
const show = (...el) => [...el].forEach(e => (e.style.display = ''));
```

<details>
<summary>Examples</summary>

```js
show(...document.querySelectorAll('img')); // Shows all <img> elements on the page
```

</details>

<br>[⬆ Back to top](#contents)

### smoothScroll

Smoothly scrolls the element on which it's called into the visible area of the browser window.

Use `.scrollIntoView` method to scroll the element. 
Pass `{ behavior: 'smooth' }` to `.scrollIntoView` so it scrolls smoothly.

```js
const smoothScroll = element =>
  document.querySelector(element).scrollIntoView({
    behavior: 'smooth'
  });
```

<details>
<summary>Examples</summary>

```js
smoothScroll('#fooBar'); // scrolls smoothly to the element with the id fooBar
smoothScroll('.fooBar'); // scrolls smoothly to the first element with a class of fooBar
```

</details>

<br>[⬆ Back to top](#contents)

### toggleClass

Toggle a class for an element.

Use `element.classList.toggle()` to toggle the specified class for the element.

```js
const toggleClass = (el, className) => el.classList.toggle(className);
```

<details>
<summary>Examples</summary>

```js
toggleClass(document.querySelector('p.special'), 'special'); // The paragraph will not have the 'special' class anymore
```

</details>

<br>[⬆ Back to top](#contents)

### triggerEvent

Triggers a specific event on a given element, optionally passing custom data.

Use `new CustomEvent()` to create an event from the specified `eventType` and details.
Use `el.dispatchEvent()` to trigger the newly created event on the given element.
Omit the third argument, `detail`, if you do not want to pass custom data to the triggered event.

```js
const triggerEvent = (el, eventType, detail) =>
  el.dispatchEvent(new CustomEvent(eventType, { detail }));
```

<details>
<summary>Examples</summary>

```js
triggerEvent(document.getElementById('myId'), 'click');
triggerEvent(document.getElementById('myId'), 'click', { username: 'bob' });
```

</details>

<br>[⬆ Back to top](#contents)

### UUIDGeneratorBrowser

Generates a UUID in a browser.

Use `crypto` API to generate a UUID, compliant with [RFC4122](https://www.ietf.org/rfc/rfc4122.txt) version 4.

```js
const UUIDGeneratorBrowser = () =>
  ([1e7] + -1e3 + -4e3 + -8e3 + -1e11).replace(/[018]/g, c =>
    (c ^ (crypto.getRandomValues(new Uint8Array(1))[0] & (15 >> (c / 4)))).toString(16)
  );
```

<details>
<summary>Examples</summary>

```js
UUIDGeneratorBrowser(); // '7982fcfe-5721-4632-bede-6000885be57d'
```

</details>

<br>[⬆ Back to top](#contents)


---

## ⏱️ Date

### dayOfYear

Gets the day of the year from a `Date` object.

Use `new Date()` and `Date.prototype.getFullYear()` to get the first day of the year as a `Date` object, subtract it from the provided `date` and divide with the milliseconds in each day to get the result.
Use `Math.floor()` to appropriately round the resulting day count to an integer.

```js
const dayOfYear = date =>
  Math.floor((date - new Date(date.getFullYear(), 0, 0)) / 1000 / 60 / 60 / 24);
```

<details>
<summary>Examples</summary>

```js
dayOfYear(new Date()); // 272
```

</details>

<br>[⬆ Back to top](#contents)

### formatDuration

Returns the human readable format of the given number of milliseconds.

Divide `ms` with the appropriate values to obtain the appropriate values for `day`, `hour`, `minute`, `second` and `millisecond`.
Use `Object.entries()` with `Array.prototype.filter()` to keep only non-zero values.
Use `Array.prototype.map()` to create the string for each value, pluralizing appropriately.
Use `String.prototype.join(', ')` to combine the values into a string.

```js
const formatDuration = ms => {
  if (ms < 0) ms = -ms;
  const time = {
    day: Math.floor(ms / 86400000),
    hour: Math.floor(ms / 3600000) % 24,
    minute: Math.floor(ms / 60000) % 60,
    second: Math.floor(ms / 1000) % 60,
    millisecond: Math.floor(ms) % 1000
  };
  return Object.entries(time)
    .filter(val => val[1] !== 0)
    .map(([key, val]) => `${val} ${key}${val !== 1 ? 's' : ''}`)
    .join(', ');
};
```

<details>
<summary>Examples</summary>

```js
formatDuration(1001); // '1 second, 1 millisecond'
formatDuration(34325055574); // '397 days, 6 hours, 44 minutes, 15 seconds, 574 milliseconds'
```

</details>

<br>[⬆ Back to top](#contents)

### getColonTimeFromDate

Returns a string of the form `HH:MM:SS` from a `Date` object.

Use `Date.prototype.toTimeString()` and `String.prototype.slice()` to get the `HH:MM:SS` part of a given `Date` object.

```js
const getColonTimeFromDate = date => date.toTimeString().slice(0, 8);
```

<details>
<summary>Examples</summary>

```js
getColonTimeFromDate(new Date()); // "08:38:00"
```

</details>

<br>[⬆ Back to top](#contents)

### getDaysDiffBetweenDates

Returns the difference (in days) between two dates.

Calculate the difference (in days) between two `Date` objects.

```js
const getDaysDiffBetweenDates = (dateInitial, dateFinal) =>
  (dateFinal - dateInitial) / (1000 * 3600 * 24);
```

<details>
<summary>Examples</summary>

```js
getDaysDiffBetweenDates(new Date('2017-12-13'), new Date('2017-12-22')); // 9
```

</details>

<br>[⬆ Back to top](#contents)

### getMeridiemSuffixOfInteger

Converts an integer to a suffixed string, adding `am` or `pm` based on its value.

Use the modulo operator (`%`) and conditional checks to transform an integer to a stringified 12-hour format with meridiem suffix.

```js
const getMeridiemSuffixOfInteger = num =>
  num === 0 || num === 24
    ? 12 + 'am'
    : num === 12
      ? 12 + 'pm'
      : num < 12
        ? (num % 12) + 'am'
        : (num % 12) + 'pm';
```

<details>
<summary>Examples</summary>

```js
getMeridiemSuffixOfInteger(0); // "12am"
getMeridiemSuffixOfInteger(11); // "11am"
getMeridiemSuffixOfInteger(13); // "1pm"
getMeridiemSuffixOfInteger(25); // "1pm"
```

</details>

<br>[⬆ Back to top](#contents)

### isAfterDate

Check if a date is after another date.

Use the greater than operator (`>`) to check if the first date comes after the second one.

```js
const isAfterDate = (dateA, dateB) => dateA > dateB;
```

<details>
<summary>Examples</summary>

```js
isAfterDate(new Date(2010, 10, 21), new Date(2010, 10, 20)); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isBeforeDate

Check if a date is before another date.

Use the less than operator (`<`) to check if the first date comes before the second one.

```js
const isBeforeDate = (dateA, dateB) => dateA < dateB;
```

<details>
<summary>Examples</summary>

```js
isBeforeDate(new Date(2010, 10, 20), new Date(2010, 10, 21)); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isSameDate

Check if a date is the same as another date.

Use `Date.prototype.toISOString()` and strict equality checking (`===`) to check if the first date is the same as the second one.

```js
const isSameDate = (dateA, dateB) => dateA.toISOString() === dateB.toISOString();
```

<details>
<summary>Examples</summary>

```js
isSameDate(new Date(2010, 10, 20), new Date(2010, 10, 20)); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isWeekday

Results in a boolean representation of a specific date.

Pass the specific date object firstly.
Use `Date.getDay()` to check weekday by using a modulo operator and then returning a boolean.

```js
const isWeekday = (t = new Date()) => {
  return t.getDay() % 6 !== 0;
};
```

<details>
<summary>Examples</summary>

```js
isWeekday(); // true (if current date is 2019-07-19)
```

</details>

<br>[⬆ Back to top](#contents)

### isWeekend

Results in a boolean representation of a specific date.

Pass the specific date object firstly.
Use `Date.getDay()` to check weekend based on the day being returned as 0 - 6 using a modulo operation then return a boolean.

```js
const isWeekend = (t = new Date()) => {
  return t.getDay() % 6 === 0;
};
```

<details>
<summary>Examples</summary>

```js
isWeekend(); // 2018-10-19 (if current date is 2018-10-18)
```

</details>

<br>[⬆ Back to top](#contents)

### maxDate

Returns the maximum of the given dates.

Use the ES6 spread syntax with `Math.max` to find the maximum date value, `new Date()` to convert it to a `Date` object.

```js
const maxDate = dates => new Date(Math.max(...dates));
```

<details>
<summary>Examples</summary>

```js
const array = [
  new Date(2017, 4, 13),
  new Date(2018, 2, 12),
  new Date(2016, 0, 10),
  new Date(2016, 0, 9)
];
maxDate(array); // 2018-03-11T22:00:00.000Z
```

</details>

<br>[⬆ Back to top](#contents)

### minDate

Returns the minimum of the given dates.

Use the ES6 spread syntax to find the minimum date value, `new Date()` to convert it to a `Date` object.

```js
const minDate = dates => new Date(Math.min(...dates));
```

<details>
<summary>Examples</summary>

```js
const array = [
  new Date(2017, 4, 13),
  new Date(2018, 2, 12),
  new Date(2016, 0, 10),
  new Date(2016, 0, 9)
];
minDate(array); // 2016-01-08T22:00:00.000Z
```

</details>

<br>[⬆ Back to top](#contents)

### tomorrow

Results in a string representation of tomorrow's date.

Use `new Date()` to get the current date, increment by one using `Date.getDate()` and set the value to the result using `Date.setDate()`. 
Use `Date.prototype.toISOString()` to return a string in `yyyy-mm-dd` format.

```js
const tomorrow = () => {
  let t = new Date();
  t.setDate(t.getDate() + 1);
  return t.toISOString().split('T')[0];
};
```

<details>
<summary>Examples</summary>

```js
tomorrow(); // 2018-10-19 (if current date is 2018-10-18)
```

</details>

<br>[⬆ Back to top](#contents)

### yesterday

Results in a string representation of yesterday's date.

Use `new Date()` to get the current date, decrement by one using `Date.getDate()` and set the value to the result using `Date.setDate()`.
Use `Date.prototype.toISOString()` to return a string in `yyyy-mm-dd` format.

```js
const yesterday = () => {
  let t = new Date();
  t.setDate(t.getDate() - 1);
  return t.toISOString().split('T')[0];
};
```

<details>
<summary>Examples</summary>

```js
yesterday(); // 2018-10-17 (if current date is 2018-10-18)
```

</details>

<br>[⬆ Back to top](#contents)


---

## 🎛️ Function

### attempt



尝试调用作为参数的函数，返回结果或捕获到的错误对象。

使用 `try ... catch` 块返回函数的结果或适当的错误。


```js
const attempt = (fn, ...args) => {
  try {
    return fn(...args);
  } catch (e) {
    return e instanceof Error ? e : new Error(e);
  }
};
```

<details>
<summary>Examples</summary>

```js
var elements = attempt(function(selector) {
  return document.querySelectorAll(selector);
}, '>_>');
if (elements instanceof Error) elements = []; // elements = []
```

</details>

<br>[⬆ Back to top](#contents)

### bind



创建一个函数，该函数使用给定的上下文调用 `fn`，最初的参数列表中添加任何额外提供的可选参数。

返回一个 `function`，它使用 `Function.prototype.apply()` 将给定的 `context` 应用于 `fn`。
使用 spread 操作符(`...`) 将任何额外提供的可选参数添加到参数列表中，并传递给 `fn`。

```js
const bind = (fn, context, ...boundArgs) => (...args) => fn.apply(context, [...boundArgs, ...args]);
```

<details>
<summary>Examples</summary>

```js
function greet(greeting, punctuation) {
  return greeting + ' ' + this.user + punctuation;
}
const freddy = { user: 'fred' };
const freddyBound = bind(greet, freddy);
console.log(freddyBound('hi', '!')); // 'hi fred!'
```

</details>

<br>[⬆ Back to top](#contents)

### bindKey



创建一个函数，该函数以对象的给定键调用方法，并可选地在参数的开头添加任何额外提供的参数。

```js
const bindKey = (context, fn, ...boundArgs) => (...args) =>
  context[fn].apply(context, [...boundArgs, ...args]);
```

<details>
<summary>Examples</summary>

```js
const freddy = {
  user: 'fred',
  greet: function(greeting, punctuation) {
    return greeting + ' ' + this.user + punctuation;
  }
};
const freddyBound = bindKey(freddy, 'greet');
console.log(freddyBound('hi', '!')); // 'hi fred!'
```

</details>

<br>[⬆ Back to top](#contents)

### chainAsync



链式调用异步函数。

循环遍历包含异步事件的函数数组，每次异步事件完成后调用 `next`。

```js
const chainAsync = fns => {
  let curr = 0;
  const last = fns[fns.length - 1];
  const next = () => {
    const fn = fns[curr++];
    fn === last ? fn() : fn(next);
  };
  next();
};
```

<details>
<summary>Examples</summary>

```js
chainAsync([
  next => {
    console.log('0 seconds');
    setTimeout(next, 1000);
  },
  next => {
    console.log('1 second');
    setTimeout(next, 1000);
  },
  () => {
    console.log('2 second');
  }
]);
```

</details>

<br>[⬆ Back to top](#contents)

### checkProp



给定一个断言（predicate）函数和一个 `prop` 字符串，这个柯里化（curried）函数将接收一个 `object` 对象，把对象访问的属性值，传递给断言函数，

调用 `obj` 上的 `prop` ，将它传递给提供的 `predicate` 函数，并返回一个布尔值。

```js
const checkProp = (predicate, prop) => obj => !!predicate(obj[prop]);
```

<details>
<summary>Examples</summary>

```js


const lengthIs4 = checkProp(l => l === 4, 'length');
lengthIs4([]); // false
lengthIs4([1,2,3,4]); // true
lengthIs4(new Set([1,2,3,4])); // false (Set uses Size, not length)

const session = { user: {} };
const validUserSession = checkProps(u => u.active && !u.disabled, 'user');

validUserSession(session); // false

session.user.active = true;
validUserSession(session); // true

const noLength(l => l === undefined, 'length');
noLength([]); // false
noLength({}); // true
noLength(new Set()); // true
```

</details>

<br>[⬆ Back to top](#contents)

### compose - 函数式编程术语：函数组合



执行从右到左的函数组合。

使用 `Array.prototype.reduce()` 执行从右到左的函数组合。
最后一个(最右边的)函数可以接受一个或多个参数;其余的函数必须是接收一个参数的函数。

```js
const compose = (...fns) => fns.reduce((f, g) => (...args) => f(g(...args)));
```

<details>
<summary>Examples</summary>

```js
const add5 = x => x + 5;
const multiply = (x, y) => x * y;
const multiplyAndAdd5 = compose(
  add5,
  multiply
);
multiplyAndAdd5(5, 2); // 15
```

</details>

<br>[⬆ Back to top](#contents)

### composeRight



执行从左到右的函数组合。

使用 `Array.prototype.reduce()` 执行从左到右的函数组合。
第一个(最左边的)函数可以接受一个或多个参数;其余的函数必须是接收一个参数的函数。

```js
const composeRight = (...fns) => fns.reduce((f, g) => (...args) => g(f(...args)));
```

<details>
<summary>Examples</summary>

```js
const add = (x, y) => x + y;
const square = x => x * x;
const addAndSquare = composeRight(add, square);
addAndSquare(1, 2); // 9
```

</details>

<br>[⬆ Back to top](#contents)

### converge



接受聚合函数和分支函数列表，并返回一个函数，该函数将参数传递给每个分支函数，分支函数的结果作为参数传递给聚合函数。

使用 `Array.prototype.map()` 和 `function .prototype.apply()` 使每个函数处理给定的参数。
调用 `coverger` 使用 spread 操作符('...')得到所有其他函数的结果。

```js
const converge = (converger, fns) => (...args) => converger(...fns.map(fn => fn.apply(null, args)));
```

<details>
<summary>Examples</summary>

```js
const average = converge((a, b) => a / b, [
  arr => arr.reduce((a, v) => a + v, 0),
  arr => arr.length
]);
average([1, 2, 3, 4, 5, 6, 7]); // 4
```

</details>

<br>[⬆ Back to top](#contents)

### curry --- 函数式编程术语：柯里化



柯里化一个函数。

使用递归。 
如果提供的参数 (`args`) 是函数 `fn` 接受的参数数量，则调用传递的函数 `fn`， 否则返回一个可接收剩余参数被柯里化后的函数 `fn`。
如果你想柯里化一个接受可变参数数量的函数(可变参数的函数，例如 `Math.min()` )，你可以选择将参数个数传递给第二个参数 `arity`。

```js
const curry = (fn, arity = fn.length, ...args) =>
  arity <= args.length ? fn(...args) : curry.bind(null, fn, arity, ...args);
```

<details>
<summary>Examples</summary>

```js
curry(Math.pow)(2)(10); // 1024
curry(Math.min, 3)(10)(50)(2); // 2
```

</details>

<br>[⬆ Back to top](#contents)

### debounce

Creates a debounced function that delays invoking the provided function until at least `ms` milliseconds have elapsed since the last time it was invoked.

Each time the debounced function is invoked, clear the current pending timeout with `clearTimeout()` and use `setTimeout()` to create a new timeout that delays invoking the function until at least `ms` milliseconds has elapsed. Use `Function.prototype.apply()` to apply the `this` context to the function and provide the necessary arguments.
Omit the second argument, `ms`, to set the timeout at a default of 0 ms.

```js
const debounce = (fn, ms = 0) => {
  let timeoutId;
  return function(...args) {
    clearTimeout(timeoutId);
    timeoutId = setTimeout(() => fn.apply(this, args), ms);
  };
};
```

<details>
<summary>Examples</summary>

```js
window.addEventListener(
  'resize',
  debounce(() => {
    console.log(window.innerWidth);
    console.log(window.innerHeight);
  }, 250)
); // Will log the window dimensions at most every 250ms
```

</details>

<br>[⬆ Back to top](#contents)

### defer

Defers invoking a function until the current call stack has cleared.

Use `setTimeout()` with a timeout of 1ms to add a new event to the browser event queue and allow the rendering engine to complete its work. Use the spread (`...`) operator to supply the function with an arbitrary number of arguments.

```js
const defer = (fn, ...args) => setTimeout(fn, 1, ...args);
```

<details>
<summary>Examples</summary>

```js
// Example A:
defer(console.log, 'a'), console.log('b'); // logs 'b' then 'a'

// Example B:
document.querySelector('#someElement').innerHTML = 'Hello';
longRunningFunction(); // Browser will not update the HTML until this has finished
defer(longRunningFunction); // Browser will update the HTML then run the function
```

</details>

<br>[⬆ Back to top](#contents)

### delay

Invokes the provided function after `wait` milliseconds.

Use `setTimeout()` to delay execution of `fn`.
Use the spread (`...`) operator to supply the function with an arbitrary number of arguments.

```js
const delay = (fn, wait, ...args) => setTimeout(fn, wait, ...args);
```

<details>
<summary>Examples</summary>

```js
delay(
  function(text) {
    console.log(text);
  },
  1000,
  'later'
); // Logs 'later' after one second.
```

</details>

<br>[⬆ Back to top](#contents)

### functionName

Logs the name of a function.

Use `console.debug()` and the `name` property of the passed method to log the method's name to the `debug` channel of the console.

```js
const functionName = fn => (console.debug(fn.name), fn);
```

<details>
<summary>Examples</summary>

```js
functionName(Math.max); // max (logged in debug channel of console)
```

</details>

<br>[⬆ Back to top](#contents)

### hz

Returns the number of times a function executed per second. 
`hz` is the unit for `hertz`, the unit of frequency defined as one cycle per second.

Use `performance.now()` to get the difference in milliseconds before and after the iteration loop to calculate the time elapsed executing the function `iterations` times. 
Return the number of cycles per second by converting milliseconds to seconds and dividing it by the time elapsed. 
Omit the second argument, `iterations`, to use the default of 100 iterations.

```js
const hz = (fn, iterations = 100) => {
  const before = performance.now();
  for (let i = 0; i < iterations; i++) fn();
  return (1000 * iterations) / (performance.now() - before);
};
```

<details>
<summary>Examples</summary>

```js
// 10,000 element array
const numbers = Array(10000)
  .fill()
  .map((_, i) => i);

// Test functions with the same goal: sum up the elements in the array
const sumReduce = () => numbers.reduce((acc, n) => acc + n, 0);
const sumForLoop = () => {
  let sum = 0;
  for (let i = 0; i < numbers.length; i++) sum += numbers[i];
  return sum;
};

// `sumForLoop` is nearly 10 times faster
Math.round(hz(sumReduce)); // 572
Math.round(hz(sumForLoop)); // 4784
```

</details>

<br>[⬆ Back to top](#contents)

### memoize ![advanced](/advanced.svg)

Returns the memoized (cached) function.

Create an empty cache by instantiating a new `Map` object.
Return a function which takes a single argument to be supplied to the memoized function by first checking if the function's output for that specific input value is already cached, or store and return it if not. The `function` keyword must be used in order to allow the memoized function to have its `this` context changed if necessary.
Allow access to the `cache` by setting it as a property on the returned function.

```js
const memoize = fn => {
  const cache = new Map();
  const cached = function(val) {
    return cache.has(val) ? cache.get(val) : cache.set(val, fn.call(this, val)) && cache.get(val);
  };
  cached.cache = cache;
  return cached;
};
```

<details>
<summary>Examples</summary>

```js
// See the `anagrams` snippet.
const anagramsCached = memoize(anagrams);
anagramsCached('javascript'); // takes a long time
anagramsCached('javascript'); // returns virtually instantly since it's now cached
console.log(anagramsCached.cache); // The cached anagrams map
```

</details>

<br>[⬆ Back to top](#contents)

### negate

Negates a predicate function.

Take a predicate function and apply the not operator (`!`) to it with its arguments.

```js
const negate = func => (...args) => !func(...args);
```

<details>
<summary>Examples</summary>

```js
[1, 2, 3, 4, 5, 6].filter(negate(n => n % 2 === 0)); // [ 1, 3, 5 ]
```

</details>

<br>[⬆ Back to top](#contents)

### once

Ensures a function is called only once.

Utilizing a closure, use a flag, `called`, and set it to `true` once the function is called for the first time, preventing it from being called again. In order to allow the function to have its `this` context changed (such as in an event listener), the `function` keyword must be used, and the supplied function must have the context applied.
Allow the function to be supplied with an arbitrary number of arguments using the rest/spread (`...`) operator.

```js
const once = fn => {
  let called = false;
  return function(...args) {
    if (called) return;
    called = true;
    return fn.apply(this, args);
  };
};
```

<details>
<summary>Examples</summary>

```js
const startApp = function(event) {
  console.log(this, event); // document.body, MouseEvent
};
document.body.addEventListener('click', once(startApp)); // only runs `startApp` once upon click
```

</details>

<br>[⬆ Back to top](#contents)

### partial

Creates a function that invokes `fn` with `partials` prepended to the arguments it receives.

Use the spread operator (`...`) to prepend `partials` to the list of arguments of `fn`.

```js
const partial = (fn, ...partials) => (...args) => fn(...partials, ...args);
```

<details>
<summary>Examples</summary>

```js
const greet = (greeting, name) => greeting + ' ' + name + '!';
const greetHello = partial(greet, 'Hello');
greetHello('John'); // 'Hello John!'
```

</details>

<br>[⬆ Back to top](#contents)

### partialRight

Creates a function that invokes `fn` with `partials` appended to the arguments it receives.

Use the spread operator (`...`) to append `partials` to the list of arguments of `fn`.

```js
const partialRight = (fn, ...partials) => (...args) => fn(...args, ...partials);
```

<details>
<summary>Examples</summary>

```js
const greet = (greeting, name) => greeting + ' ' + name + '!';
const greetJohn = partialRight(greet, 'John');
greetJohn('Hello'); // 'Hello John!'
```

</details>

<br>[⬆ Back to top](#contents)

### runPromisesInSeries

Runs an array of promises in series.

Use `Array.prototype.reduce()` to create a promise chain, where each promise returns the next promise when resolved.

```js
const runPromisesInSeries = ps => ps.reduce((p, next) => p.then(next), Promise.resolve());
```

<details>
<summary>Examples</summary>

```js
const delay = d => new Promise(r => setTimeout(r, d));
runPromisesInSeries([() => delay(1000), () => delay(2000)]); // Executes each promise sequentially, taking a total of 3 seconds to complete
```

</details>

<br>[⬆ Back to top](#contents)

### sleep

Delays the execution of an asynchronous function.

Delay executing part of an `async` function, by putting it to sleep, returning a `Promise`.

```js
const sleep = ms => new Promise(resolve => setTimeout(resolve, ms));
```

<details>
<summary>Examples</summary>

```js
async function sleepyWork() {
  console.log("I'm going to sleep for 1 second.");
  await sleep(1000);
  console.log('I woke up after 1 second.');
}
```

</details>

<br>[⬆ Back to top](#contents)

### throttle ![advanced](/advanced.svg)

Creates a throttled function that only invokes the provided function at most once per every `wait` milliseconds

Use `setTimeout()` and `clearTimeout()` to throttle the given method, `fn`.
Use `Function.prototype.apply()` to apply the `this` context to the function and provide the necessary `arguments`.
Use `Date.now()` to keep track of the last time the throttled function was invoked.
Omit the second argument, `wait`, to set the timeout at a default of 0 ms.

```js
const throttle = (fn, wait) => {
  let inThrottle, lastFn, lastTime;
  return function() {
    const context = this,
      args = arguments;
    if (!inThrottle) {
      fn.apply(context, args);
      lastTime = Date.now();
      inThrottle = true;
    } else {
      clearTimeout(lastFn);
      lastFn = setTimeout(function() {
        if (Date.now() - lastTime >= wait) {
          fn.apply(context, args);
          lastTime = Date.now();
        }
      }, Math.max(wait - (Date.now() - lastTime), 0));
    }
  };
};
```

<details>
<summary>Examples</summary>

```js
window.addEventListener(
  'resize',
  throttle(function(evt) {
    console.log(window.innerWidth);
    console.log(window.innerHeight);
  }, 250)
); // Will log the window dimensions at most every 250ms
```

</details>

<br>[⬆ Back to top](#contents)

### times

Iterates over a callback `n` times

Use `Function.call()` to call `fn` `n` times or until it returns `false`.
Omit the last argument, `context`, to use an `undefined` object (or the global object in non-strict mode).

```js
const times = (n, fn, context = undefined) => {
  let i = 0;
  while (fn.call(context, i) !== false && ++i < n) {}
};
```

<details>
<summary>Examples</summary>

```js
var output = '';
times(5, i => (output += i));
console.log(output); // 01234
```

</details>

<br>[⬆ Back to top](#contents)

### uncurry

Uncurries a function up to depth `n`.

Return a variadic function.
Use `Array.prototype.reduce()` on the provided arguments to call each subsequent curry level of the function.
If the `length` of the provided arguments is less than `n` throw an error.
Otherwise, call `fn` with the proper amount of arguments, using `Array.prototype.slice(0, n)`.
Omit the second argument, `n`, to uncurry up to depth `1`.

```js
const uncurry = (fn, n = 1) => (...args) => {
  const next = acc => args => args.reduce((x, y) => x(y), acc);
  if (n > args.length) throw new RangeError('Arguments too few!');
  return next(fn)(args.slice(0, n));
};
```

<details>
<summary>Examples</summary>

```js
const add = x => y => z => x + y + z;
const uncurriedAdd = uncurry(add, 3);
uncurriedAdd(1, 2, 3); // 6
```

</details>

<br>[⬆ Back to top](#contents)

### unfold

Builds an array, using an iterator function and an initial seed value.

Use a `while` loop and `Array.prototype.push()` to call the function repeatedly until it returns `false`.
The iterator function accepts one argument (`seed`) and must always return an array with two elements ([`value`, `nextSeed`]) or `false` to terminate.

```js
const unfold = (fn, seed) => {
  let result = [],
    val = [null, seed];
  while ((val = fn(val[1]))) result.push(val[0]);
  return result;
};
```

<details>
<summary>Examples</summary>

```js
var f = n => (n > 50 ? false : [-n, n + 10]);
unfold(f, 10); // [-10, -20, -30, -40, -50]
```

</details>

<br>[⬆ Back to top](#contents)

### when

Tests a value, `x`, against a predicate function. If `true`, return `fn(x)`. Else, return `x`. 

Return a function expecting a single value, `x`, that returns the appropriate value based on `pred`.

```js
const when = (pred, whenTrue) => x => (pred(x) ? whenTrue(x) : x);
```

<details>
<summary>Examples</summary>

```js
const doubleEvenNumbers = when(x => x % 2 === 0, x => x * 2);
doubleEvenNumbers(2); // 4
doubleEvenNumbers(1); // 1
```

</details>

<br>[⬆ Back to top](#contents)


---

## ➗ Math

### approximatelyEqual

Checks if two numbers are approximately equal to each other.

Use `Math.abs()` to compare the absolute difference of the two values to `epsilon`.
Omit the third parameter, `epsilon`, to use a default value of `0.001`.

检查两个数是否近似相等。

使用 `Math.abs()` 将两个值的绝对差值与 `epsilon` 进行比较。
省略第三个参数 `epsilon`，使用默认值`0.001`。


```js
const approximatelyEqual = (v1, v2, epsilon = 0.001) => Math.abs(v1 - v2) < epsilon;
```

<details>
<summary>Examples</summary>

```js
approximatelyEqual(Math.PI / 2.0, 1.5708); // true
```

</details>

<br>[⬆ Back to top](#contents)

### average



返回两个或更多数字的平均值。

使用 `array. prototype.reduce()` 将每个值累加，初始值为 `0`，然后除以数组的 `length`。


```js
const average = (...nums) => nums.reduce((acc, val) => acc + val, 0) / nums.length;
```

<details>
<summary>Examples</summary>

```js
average(...[1, 2, 3]); // 2
average(1, 2, 3); // 2
```

</details>

<br>[⬆ Back to top](#contents)

### averageBy



使用提供的函数将每个元素映射到一个值后，返回数组的平均值。

使用 `Array.prototype.map()` 将每个元素映射到 `fn` 函数的返回值，使用 `array. prototype.reduce()` 将每个值累加，初始值为 `0`，然后除以数组的 `length`。

```js
const averageBy = (arr, fn) =>
  arr.map(typeof fn === 'function' ? fn : val => val[fn]).reduce((acc, val) => acc + val, 0) /
  arr.length;
```

<details>
<summary>Examples</summary>

```js
averageBy([{ n: 4 }, { n: 2 }, { n: 8 }, { n: 6 }], o => o.n); // 5
averageBy([{ n: 4 }, { n: 2 }, { n: 8 }, { n: 6 }], 'n'); // 5
```

</details>

<br>[⬆ Back to top](#contents)

### binomialCoefficient

Evaluates the binomial coefficient of two integers `n` and `k`.

Use `Number.isNaN()` to check if any of the two values is `NaN`.
Check if `k` is less than `0`, greater than or equal to `n`, equal to `1` or `n - 1` and return the appropriate result.
Check if `n - k` is less than `k` and switch their values accordingly.
Loop from `2` through `k` and calculate the binomial coefficient.
Use `Math.round()` to account for rounding errors in the calculation.

```js
const binomialCoefficient = (n, k) => {
  if (Number.isNaN(n) || Number.isNaN(k)) return NaN;
  if (k < 0 || k > n) return 0;
  if (k === 0 || k === n) return 1;
  if (k === 1 || k === n - 1) return n;
  if (n - k < k) k = n - k;
  let res = n;
  for (let j = 2; j <= k; j++) res *= (n - j + 1) / j;
  return Math.round(res);
};
```

<details>
<summary>Examples</summary>

```js
binomialCoefficient(8, 2); // 28
```

</details>

<br>[⬆ Back to top](#contents)

### clampNumber

Clamps `num` within the inclusive range specified by the boundary values `a` and `b`.

If `num` falls within the range, return `num`.
Otherwise, return the nearest number in the range.

将num夹在由边值a和b指定的包含范围内。

在边界值“a”和“b”指定的包含范围内钳位`num`。

返回由边界值 `a` 和 `b` 限定范围内的 `num` 。

如果 `num` 在限定范围内，则返回 `num`。 否则，返回范围内最接近 `num` 的数字。

```js
const clampNumber = (num, a, b) => Math.max(Math.min(num, Math.max(a, b)), Math.min(a, b));
```

<details>
<summary>Examples</summary>

```js
clampNumber(2, 3, 5); // 3
clampNumber(1, -1, -5); // -1
```

</details>

<br>[⬆ Back to top](#contents)

### degreesToRads

Converts an angle from degrees to radians.

Use `Math.PI` and the degree to radian formula to convert the angle from degrees to radians.

```js
const degreesToRads = deg => (deg * Math.PI) / 180.0;
```

<details>
<summary>Examples</summary>

```js
degreesToRads(90.0); // ~1.5708
```

</details>

<br>[⬆ Back to top](#contents)

### digitize

Converts a number to an array of digits.

Convert the number to a string, using the spread operator (`...`) to build an array.
Use `Array.prototype.map()` and `parseInt()` to transform each value to an integer.

```js
const digitize = n => [...`${n}`].map(i => parseInt(i));
```

<details>
<summary>Examples</summary>

```js
digitize(123); // [1, 2, 3]
```

</details>

<br>[⬆ Back to top](#contents)

### distance

Returns the distance between two points.

Use `Math.hypot()` to calculate the Euclidean distance between two points.

```js
const distance = (x0, y0, x1, y1) => Math.hypot(x1 - x0, y1 - y0);
```

<details>
<summary>Examples</summary>

```js
distance(1, 1, 2, 3); // 2.23606797749979
```

</details>

<br>[⬆ Back to top](#contents)

### elo ![advanced](/advanced.svg)

Computes the new ratings between two or more opponents using the [Elo rating system](https://en.wikipedia.org/wiki/Elo_rating_system). It takes an array
of pre-ratings and returns an array containing post-ratings.
The array should be ordered from best performer to worst performer (winner -> loser).

Use the exponent `**` operator and math operators to compute the expected score (chance of winning).
of each opponent and compute the new rating for each.
Loop through the ratings, using each permutation to compute the post-Elo rating for each player in a pairwise fashion. 
Omit the second argument to use the default `kFactor` of 32.

```js
const elo = ([...ratings], kFactor = 32, selfRating) => {
  const [a, b] = ratings;
  const expectedScore = (self, opponent) => 1 / (1 + 10 ** ((opponent - self) / 400));
  const newRating = (rating, i) =>
    (selfRating || rating) + kFactor * (i - expectedScore(i ? a : b, i ? b : a));
  if (ratings.length === 2) return [newRating(a, 1), newRating(b, 0)];

  for (let i = 0, len = ratings.length; i < len; i++) {
    let j = i;
    while (j < len - 1) {
      j++;
      [ratings[i], ratings[j]] = elo([ratings[i], ratings[j]], kFactor);
    }
  }
  return ratings;
};
```

<details>
<summary>Examples</summary>

```js
// Standard 1v1s
elo([1200, 1200]); // [1216, 1184]
elo([1200, 1200], 64); // [1232, 1168]
// 4 player FFA, all same rank
elo([1200, 1200, 1200, 1200]).map(Math.round); // [1246, 1215, 1185, 1154]
/*
For teams, each rating can adjusted based on own team's average rating vs.
average rating of opposing team, with the score being added to their
own individual rating by supplying it as the third argument.
*/
```

</details>

<br>[⬆ Back to top](#contents)

### factorial

Calculates the factorial of a number.

Use recursion.
If `n` is less than or equal to `1`, return `1`.
Otherwise, return the product of `n` and the factorial of `n - 1`.
Throws an exception if `n` is a negative number.

```js
const factorial = n =>
  n < 0
    ? (() => {
      throw new TypeError('Negative numbers are not allowed!');
    })()
    : n <= 1
      ? 1
      : n * factorial(n - 1);
```

<details>
<summary>Examples</summary>

```js
factorial(6); // 720
```

</details>

<br>[⬆ Back to top](#contents)

### fibonacci

Generates an array, containing the Fibonacci sequence, up until the nth term.

Create an empty array of the specific length, initializing the first two values (`0` and `1`).
Use `Array.prototype.reduce()` to add values into the array, using the sum of the last two values, except for the first two.

```js
const fibonacci = n =>
  Array.from({ length: n }).reduce(
    (acc, val, i) => acc.concat(i > 1 ? acc[i - 1] + acc[i - 2] : i),
    []
  );
```

<details>
<summary>Examples</summary>

```js
fibonacci(6); // [0, 1, 1, 2, 3, 5]
```

</details>

<br>[⬆ Back to top](#contents)

### gcd

Calculates the greatest common divisor between two or more numbers/arrays.

The inner `_gcd` function uses recursion.
Base case is when `y` equals `0`. In this case, return `x`.
Otherwise, return the GCD of `y` and the remainder of the division `x/y`.

```js
const gcd = (...arr) => {
  const _gcd = (x, y) => (!y ? x : gcd(y, x % y));
  return [...arr].reduce((a, b) => _gcd(a, b));
};
```

<details>
<summary>Examples</summary>

```js
gcd(8, 36); // 4
gcd(...[12, 8, 32]); // 4
```

</details>

<br>[⬆ Back to top](#contents)

### geometricProgression

Initializes an array containing the numbers in the specified range where `start` and `end` are inclusive and the ratio between two terms is `step`.
Returns an error if `step` equals `1`.

Use `Array.from()`, `Math.log()` and `Math.floor()` to create an array of the desired length, `Array.prototype.map()` to fill with the desired values in a range.
Omit the second argument, `start`, to use a default value of `1`.
Omit the third argument, `step`, to use a default value of `2`.

```js
const geometricProgression = (end, start = 1, step = 2) =>
  Array.from({ length: Math.floor(Math.log(end / start) / Math.log(step)) + 1 }).map(
    (v, i) => start * step ** i
  );
```

<details>
<summary>Examples</summary>

```js
geometricProgression(256); // [1, 2, 4, 8, 16, 32, 64, 128, 256]
geometricProgression(256, 3); // [3, 6, 12, 24, 48, 96, 192]
geometricProgression(256, 1, 4); // [1, 4, 16, 64, 256]
```

</details>

<br>[⬆ Back to top](#contents)

### hammingDistance

Calculates the Hamming distance between two values.

Use XOR operator (`^`) to find the bit difference between the two numbers, convert to a binary string using `toString(2)`.
Count and return the number of `1`s in the string, using `match(/1/g)`.

```js
const hammingDistance = (num1, num2) => ((num1 ^ num2).toString(2).match(/1/g) || '').length;
```

<details>
<summary>Examples</summary>

```js
hammingDistance(2, 3); // 1
```

</details>

<br>[⬆ Back to top](#contents)

### inRange

Checks if the given number falls within the given range.

Use arithmetic comparison to check if the given number is in the specified range.
If the second parameter, `end`, is not specified, the range is considered to be from `0` to `start`.

```js
const inRange = (n, start, end = null) => {
  if (end && start > end) [end, start] = [start, end];
  return end == null ? n >= 0 && n < start : n >= start && n < end;
};
```

<details>
<summary>Examples</summary>

```js
inRange(3, 2, 5); // true
inRange(3, 4); // true
inRange(2, 3, 5); // false
inRange(3, 2); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isDivisible

Checks if the first numeric argument is divisible by the second one.

Use the modulo operator (`%`) to check if the remainder is equal to `0`.

```js
const isDivisible = (dividend, divisor) => dividend % divisor === 0;
```

<details>
<summary>Examples</summary>

```js
isDivisible(6, 3); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isEven

Returns `true` if the given number is even, `false` otherwise.

Checks whether a number is odd or even using the modulo (`%`) operator.
Returns `true` if the number is even, `false` if the number is odd.

```js
const isEven = num => num % 2 === 0;
```

<details>
<summary>Examples</summary>

```js
isEven(3); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isNegativeZero

Checks if the given value is equal to negative zero (`-0`).

Checks whether a passed value is equal to `0` and if `1` divided by the value equals `-Infinity`.

```js
const isNegativeZero = val => val === 0 && 1 / val === -Infinity;
```

<details>
<summary>Examples</summary>

```js
isNegativeZero(-0); // true
isNegativeZero(0); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isPrime

Checks if the provided integer is a prime number.

Check numbers from `2` to the square root of the given number.
Return `false` if any of them divides the given number, else return `true`, unless the number is less than `2`.

```js
const isPrime = num => {
  const boundary = Math.floor(Math.sqrt(num));
  for (var i = 2; i <= boundary; i++) if (num % i === 0) return false;
  return num >= 2;
};
```

<details>
<summary>Examples</summary>

```js
isPrime(11); // true
```

</details>

<br>[⬆ Back to top](#contents)

### lcm

Returns the least common multiple of two or more numbers.

Use the greatest common divisor (GCD) formula and the fact that `lcm(x,y) = x * y / gcd(x,y)` to determine the least common multiple.
The GCD formula uses recursion.

```js
const lcm = (...arr) => {
  const gcd = (x, y) => (!y ? x : gcd(y, x % y));
  const _lcm = (x, y) => (x * y) / gcd(x, y);
  return [...arr].reduce((a, b) => _lcm(a, b));
};
```

<details>
<summary>Examples</summary>

```js
lcm(12, 7); // 84
lcm(...[1, 3, 4, 5]); // 60
```

</details>

<br>[⬆ Back to top](#contents)

### luhnCheck ![advanced](/advanced.svg)

Implementation of the [Luhn Algorithm](https://en.wikipedia.org/wiki/Luhn_algorithm) used to validate a variety of identification numbers, such as credit card numbers, IMEI numbers, National Provider Identifier numbers etc.

Use `String.prototype.split('')`, `Array.prototype.reverse()` and `Array.prototype.map()` in combination with `parseInt()` to obtain an array of digits.
Use `Array.prototype.splice(0,1)` to obtain the last digit.
Use `Array.prototype.reduce()` to implement the Luhn Algorithm.
Return `true` if `sum` is divisible by `10`, `false` otherwise.


```js
const luhnCheck = num => {
  let arr = (num + '')
    .split('')
    .reverse()
    .map(x => parseInt(x));
  let lastDigit = arr.splice(0, 1)[0];
  let sum = arr.reduce((acc, val, i) => (i % 2 !== 0 ? acc + val : acc + ((val * 2) % 9) || 9), 0);
  sum += lastDigit;
  return sum % 10 === 0;
};
```

<details>
<summary>Examples</summary>

```js
luhnCheck('4485275742308327'); // true
luhnCheck(6011329933655299); //  false
luhnCheck(123456789); // false
```

</details>

<br>[⬆ Back to top](#contents)

### mapNumRange

Maps a number from one range to another range.

Returns `num` mapped between `outMin`-`outMax` from `inMin`-`inMax`.

```js
const mapNumRange = (num, inMin, inMax, outMin, outMax) =>
  ((num - inMin) * (outMax - outMin)) / (inMax - inMin) + outMin;
```

<details>
<summary>Examples</summary>

```js
mapNumRange(5, 0, 10, 0, 100); // 50
```

</details>

<br>[⬆ Back to top](#contents)

### maxBy

Returns the maximum value of an array, after mapping each element to a value using the provided function.

Use `Array.prototype.map()` to map each element to the value returned by `fn`, `Math.max()` to get the maximum value.

```js
const maxBy = (arr, fn) => Math.max(...arr.map(typeof fn === 'function' ? fn : val => val[fn]));
```

<details>
<summary>Examples</summary>

```js
maxBy([{ n: 4 }, { n: 2 }, { n: 8 }, { n: 6 }], o => o.n); // 8
maxBy([{ n: 4 }, { n: 2 }, { n: 8 }, { n: 6 }], 'n'); // 8
```

</details>

<br>[⬆ Back to top](#contents)

### median

Returns the median of an array of numbers.

Find the middle of the array, use `Array.prototype.sort()` to sort the values.
Return the number at the midpoint if `length` is odd, otherwise the average of the two middle numbers.

```js
const median = arr => {
  const mid = Math.floor(arr.length / 2),
    nums = [...arr].sort((a, b) => a - b);
  return arr.length % 2 !== 0 ? nums[mid] : (nums[mid - 1] + nums[mid]) / 2;
};
```

<details>
<summary>Examples</summary>

```js
median([5, 6, 50, 1, -5]); // 5
```

</details>

<br>[⬆ Back to top](#contents)

### midpoint

Calculates the midpoint between two pairs of (x,y) points.

Destructure the array to get `x1`, `y1`, `x2` and `y2`, calculate the midpoint for each dimension by dividing the sum of the two endpoints by `2`.

```js
const midpoint = ([x1, y1], [x2, y2]) => [(x1 + x2) / 2, (y1 + y2) / 2];
```

<details>
<summary>Examples</summary>

```js
midpoint([2, 2], [4, 4]); // [3, 3]
midpoint([4, 4], [6, 6]); // [5, 5]
midpoint([1, 3], [2, 4]); // [1.5, 3.5]
```


</details>

<br>[⬆ Back to top](#contents)

### minBy

Returns the minimum value of an array, after mapping each element to a value using the provided function.

Use `Array.prototype.map()` to map each element to the value returned by `fn`, `Math.min()` to get the minimum value.

```js
const minBy = (arr, fn) => Math.min(...arr.map(typeof fn === 'function' ? fn : val => val[fn]));
```

<details>
<summary>Examples</summary>

```js
minBy([{ n: 4 }, { n: 2 }, { n: 8 }, { n: 6 }], o => o.n); // 2
minBy([{ n: 4 }, { n: 2 }, { n: 8 }, { n: 6 }], 'n'); // 2
```

</details>

<br>[⬆ Back to top](#contents)

### percentile

Uses the percentile formula to calculate how many numbers in the given array are less or equal to the given value.

Use `Array.prototype.reduce()` to calculate how many numbers are below the value and how many are the same value and apply the percentile formula.

```js
const percentile = (arr, val) =>
  (100 * arr.reduce((acc, v) => acc + (v < val ? 1 : 0) + (v === val ? 0.5 : 0), 0)) / arr.length;
```

<details>
<summary>Examples</summary>

```js
percentile([1, 2, 3, 4, 5, 6, 7, 8, 9, 10], 6); // 55
```

</details>

<br>[⬆ Back to top](#contents)

### powerset

Returns the powerset of a given array of numbers.

Use `Array.prototype.reduce()` combined with `Array.prototype.map()` to iterate over elements and combine into an array containing all combinations.

```js
const powerset = arr => arr.reduce((a, v) => a.concat(a.map(r => [v].concat(r))), [[]]);
```

<details>
<summary>Examples</summary>

```js
powerset([1, 2]); // [[], [1], [2], [2, 1]]
```

</details>

<br>[⬆ Back to top](#contents)

### primes

Generates primes up to a given number, using the Sieve of Eratosthenes.

Generate an array from `2` to the given number. Use `Array.prototype.filter()` to filter out the values divisible by any number from `2` to the square root of the provided number.

```js
const primes = num => {
  let arr = Array.from({ length: num - 1 }).map((x, i) => i + 2),
    sqroot = Math.floor(Math.sqrt(num)),
    numsTillSqroot = Array.from({ length: sqroot - 1 }).map((x, i) => i + 2);
  numsTillSqroot.forEach(x => (arr = arr.filter(y => y % x !== 0 || y === x)));
  return arr;
};
```

<details>
<summary>Examples</summary>

```js
primes(10); // [2,3,5,7]
```

</details>

<br>[⬆ Back to top](#contents)

### radsToDegrees

Converts an angle from radians to degrees.

Use `Math.PI` and the radian to degree formula to convert the angle from radians to degrees.

```js
const radsToDegrees = rad => (rad * 180.0) / Math.PI;
```

<details>
<summary>Examples</summary>

```js
radsToDegrees(Math.PI / 2); // 90
```

</details>

<br>[⬆ Back to top](#contents)

### randomIntArrayInRange

Returns an array of n random integers in the specified range.

Use `Array.from()` to create an empty array of the specific length, `Math.random()` to generate a random number and map it to the desired range, using `Math.floor()` to make it an integer.

```js
const randomIntArrayInRange = (min, max, n = 1) =>
  Array.from({ length: n }, () => Math.floor(Math.random() * (max - min + 1)) + min);
```

<details>
<summary>Examples</summary>

```js
randomIntArrayInRange(12, 35, 10); // [ 34, 14, 27, 17, 30, 27, 20, 26, 21, 14 ]
```

</details>

<br>[⬆ Back to top](#contents)

### randomIntegerInRange

Returns a random integer in the specified range.

Use `Math.random()` to generate a random number and map it to the desired range, using `Math.floor()` to make it an integer.

```js
const randomIntegerInRange = (min, max) => Math.floor(Math.random() * (max - min + 1)) + min;
```

<details>
<summary>Examples</summary>

```js
randomIntegerInRange(0, 5); // 2
```

</details>

<br>[⬆ Back to top](#contents)

### randomNumberInRange

Returns a random number in the specified range.

Use `Math.random()` to generate a random value, map it to the desired range using multiplication.

```js
const randomNumberInRange = (min, max) => Math.random() * (max - min) + min;
```

<details>
<summary>Examples</summary>

```js
randomNumberInRange(2, 10); // 6.0211363285087005
```

</details>

<br>[⬆ Back to top](#contents)

### round

Rounds a number to a specified amount of digits.

Use `Math.round()` and template literals to round the number to the specified number of digits.
Omit the second argument, `decimals` to round to an integer.

```js
const round = (n, decimals = 0) => Number(`${Math.round(`${n}e${decimals}`)}e-${decimals}`);
```

<details>
<summary>Examples</summary>

```js
round(1.005, 2); // 1.01
```

</details>

<br>[⬆ Back to top](#contents)

### sdbm

Hashes the input string into a whole number.

Use `String.prototype.split('')` and `Array.prototype.reduce()` to create a hash of the input string, utilizing bit shifting.

```js
const sdbm = str => {
  let arr = str.split('');
  return arr.reduce(
    (hashCode, currentVal) =>
      (hashCode = currentVal.charCodeAt(0) + (hashCode << 6) + (hashCode << 16) - hashCode),
    0
  );
};
```

<details>
<summary>Examples</summary>

```js
sdbm('name'); // -3521204949
```

</details>

<br>[⬆ Back to top](#contents)

### standardDeviation

Returns the standard deviation of an array of numbers.

Use `Array.prototype.reduce()` to calculate the mean, variance and the sum of the variance of the values, the variance of the values, then
determine the standard deviation.
You can omit the second argument to get the sample standard deviation or set it to `true` to get the population standard deviation.

```js
const standardDeviation = (arr, usePopulation = false) => {
  const mean = arr.reduce((acc, val) => acc + val, 0) / arr.length;
  return Math.sqrt(
    arr.reduce((acc, val) => acc.concat((val - mean) ** 2), []).reduce((acc, val) => acc + val, 0) /
      (arr.length - (usePopulation ? 0 : 1))
  );
};
```

<details>
<summary>Examples</summary>

```js
standardDeviation([10, 2, 38, 23, 38, 23, 21]); // 13.284434142114991 (sample)
standardDeviation([10, 2, 38, 23, 38, 23, 21], true); // 12.29899614287479 (population)
```

</details>

<br>[⬆ Back to top](#contents)

### sum

Returns the sum of two or more numbers/arrays.

Use `Array.prototype.reduce()` to add each value to an accumulator, initialized with a value of `0`.

```js
const sum = (...arr) => [...arr].reduce((acc, val) => acc + val, 0);
```

<details>
<summary>Examples</summary>

```js
sum(1, 2, 3, 4); // 10
sum(...[1, 2, 3, 4]); // 10
```

</details>

<br>[⬆ Back to top](#contents)

### sumBy

Returns the sum of an array, after mapping each element to a value using the provided function.

Use `Array.prototype.map()` to map each element to the value returned by `fn`, `Array.prototype.reduce()` to add each value to an accumulator, initialized with a value of `0`.

```js
const sumBy = (arr, fn) =>
  arr.map(typeof fn === 'function' ? fn : val => val[fn]).reduce((acc, val) => acc + val, 0);
```

<details>
<summary>Examples</summary>

```js
sumBy([{ n: 4 }, { n: 2 }, { n: 8 }, { n: 6 }], o => o.n); // 20
sumBy([{ n: 4 }, { n: 2 }, { n: 8 }, { n: 6 }], 'n'); // 20
```

</details>

<br>[⬆ Back to top](#contents)

### sumPower

Returns the sum of the powers of all the numbers from `start` to `end` (both inclusive).

Use `Array.prototype.fill()` to create an array of all the numbers in the target range, `Array.prototype.map()` and the exponent operator (`**`) to raise them to `power` and `Array.prototype.reduce()` to add them together.
Omit the second argument, `power`, to use a default power of `2`.
Omit the third argument, `start`, to use a default starting value of `1`.

```js
const sumPower = (end, power = 2, start = 1) =>
  Array(end + 1 - start)
    .fill(0)
    .map((x, i) => (i + start) ** power)
    .reduce((a, b) => a + b, 0);
```

<details>
<summary>Examples</summary>

```js
sumPower(10); // 385
sumPower(10, 3); // 3025
sumPower(10, 3, 5); // 2925
```

</details>

<br>[⬆ Back to top](#contents)

### toSafeInteger

Converts a value to a safe integer.

Use `Math.max()` and `Math.min()` to find the closest safe value.
Use `Math.round()` to convert to an integer.

```js
const toSafeInteger = num =>
  Math.round(Math.max(Math.min(num, Number.MAX_SAFE_INTEGER), Number.MIN_SAFE_INTEGER));
```

<details>
<summary>Examples</summary>

```js
toSafeInteger('3.2'); // 3
toSafeInteger(Infinity); // 9007199254740991
```

</details>

<br>[⬆ Back to top](#contents)

### vectorDistance

Returns the distance between two vectors.

Use `Array.prototype.reduce()`, `Math.pow()` and `Math.sqrt()` to calculate the Euclidean distance between two vectors.

```js
const vectorDistance = (...coords) => {
  let pointLength = Math.trunc(coords.length / 2);
  let sum = coords
    .slice(0, pointLength)
    .reduce((acc, val, i) => acc + Math.pow(val - coords[pointLength + i], 2), 0);
  return Math.sqrt(sum);
};
```

<details>
<summary>Examples</summary>

```js
vectorDistance(10, 0, 5, 20, 0, 10); // 11.180339887498949
```

</details>

<br>[⬆ Back to top](#contents)


---

## 📦 Node

### atob



解码使用 `base-64` 编码的数据字符串。

使用 `base-64` 编码为给定字符串创建 `Buffer`，并使用 `Buffer.toString（'binary'）` 返回已解码的字符串。

```js
const atob = str => Buffer.from(str, 'base64').toString('binary');
```

<details>
<summary>Examples</summary>

```js
atob('Zm9vYmFy'); // 'foobar'
```

</details>

<br>[⬆ Back to top](#contents)

### btoa

Creates a base-64 encoded ASCII string from a String object in which each character in the string is treated as a byte of binary data.

Create a `Buffer` for the given string with binary encoding and use `Buffer.toString('base64')` to return the encoded string.


创建 `base-64` 编码的 `ASCII` 字符串，其中字符串中的每个字符都被视为二进制数据的字节。

使用二进制编码为给定字符串创建 `Buffer`，并使用 `Buffer.toString（'base64'）` 返回编码字符串。

```js
const btoa = str => Buffer.from(str, 'binary').toString('base64');
```

<details>
<summary>Examples</summary>

```js
btoa('foobar'); // 'Zm9vYmFy'
```

</details>

<br>[⬆ Back to top](#contents)

### colorize

Add special characters to text to print in color in the console (combined with `console.log()`).

Use template literals and special characters to add the appropriate color code to the string output.
For background colors, add a special character that resets the background color at the end of the string.

```js
const colorize = (...args) => ({
  black: `\x1b[30m${args.join(' ')}`,
  red: `\x1b[31m${args.join(' ')}`,
  green: `\x1b[32m${args.join(' ')}`,
  yellow: `\x1b[33m${args.join(' ')}`,
  blue: `\x1b[34m${args.join(' ')}`,
  magenta: `\x1b[35m${args.join(' ')}`,
  cyan: `\x1b[36m${args.join(' ')}`,
  white: `\x1b[37m${args.join(' ')}`,
  bgBlack: `\x1b[40m${args.join(' ')}\x1b[0m`,
  bgRed: `\x1b[41m${args.join(' ')}\x1b[0m`,
  bgGreen: `\x1b[42m${args.join(' ')}\x1b[0m`,
  bgYellow: `\x1b[43m${args.join(' ')}\x1b[0m`,
  bgBlue: `\x1b[44m${args.join(' ')}\x1b[0m`,
  bgMagenta: `\x1b[45m${args.join(' ')}\x1b[0m`,
  bgCyan: `\x1b[46m${args.join(' ')}\x1b[0m`,
  bgWhite: `\x1b[47m${args.join(' ')}\x1b[0m`
});
```

向文本中添加特殊字符，以便在控制台中以彩色方式打印(与 `console.log()` 结合)。

使用模板字面量和特殊字符将相应的颜色代码添加到字符串输出中。 对于有背景颜色的，添加一个特殊字符，在字符串的末尾重置背景颜色。

<details>
<summary>Examples</summary>

```js
console.log(colorize('foo').red); // 'foo' (red letters)
console.log(colorize('foo', 'bar').bgBlue); // 'foo bar' (blue background)
console.log(colorize(colorize('foo').yellow, colorize('foo').green).bgWhite); // 'foo bar' (first word in yellow letters, second word in green letters, white background for both)
```

</details>

<br>[⬆ Back to top](#contents)

### createDirIfNotExists

Creates a directory, if it does not exist.

Use `fs.existsSync()` to check if the directory exists, `fs.mkdirSync()` to create it.

```js
const fs = require('fs');
const createDirIfNotExists = dir => (!fs.existsSync(dir) ? fs.mkdirSync(dir) : undefined);
```

<details>
<summary>Examples</summary>

```js
createDirIfNotExists('test'); // creates the directory 'test', if it doesn't exist
```

</details>

<br>[⬆ Back to top](#contents)

### hasFlags

Check if the current process's arguments contain the specified flags.

Use `Array.prototype.every()` and `Array.prototype.includes()` to check if `process.argv` contains all the specified flags.
Use a regular expression to test if the specified flags are prefixed with `-` or `--` and prefix them accordingly.

```js
const hasFlags = (...flags) =>
  flags.every(flag => process.argv.includes(/^-{1,2}/.test(flag) ? flag : '--' + flag));
```

<details>
<summary>Examples</summary>

```js
// node myScript.js -s --test --cool=true
hasFlags('-s'); // true
hasFlags('--test', 'cool=true', '-s'); // true
hasFlags('special'); // false
```

</details>

<br>[⬆ Back to top](#contents)

### hashNode

Creates a hash for a value using the [SHA-256](https://en.wikipedia.org/wiki/SHA-2) algorithm. Returns a promise.

Use `crypto` API to create a hash for the given value, `setTimeout` to prevent blocking on a long operation, and a `Promise` to give it a familiar interface.

```js
const crypto = require('crypto');
const hashNode = val =>
  new Promise(resolve =>
    setTimeout(
      () =>
        resolve(
          crypto
            .createHash('sha256')
            .update(val)
            .digest('hex')
        ),
      0
    )
  );
```

<details>
<summary>Examples</summary>

```js
hashNode(JSON.stringify({ a: 'a', b: [1, 2, 3, 4], foo: { c: 'bar' } })).then(console.log); // '04aa106279f5977f59f9067fa9712afc4aedc6f5862a8defc34552d8c7206393'
```

</details>

<br>[⬆ Back to top](#contents)

### isDuplexStream

Checks if the given argument is a duplex (readable and writable) stream.

Check if the value is different from `null`, use `typeof` to check if a value is of type `object` and the `pipe` property is of type `function`.
Additionally check if the `typeof` the `_read`, `_write` and `_readableState`, `_writableState` properties are `function` and `object` respectively.

```js
const isDuplexStream = val =>
  val !== null &&
  typeof val === 'object' &&
  typeof val.pipe === 'function' &&
  typeof val._read === 'function' &&
  typeof val._readableState === 'object' &&
  typeof val._write === 'function' &&
  typeof val._writableState === 'object';
```

<details>
<summary>Examples</summary>

```js
const Stream = require('stream');
isDuplexStream(new Stream.Duplex()); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isReadableStream

Checks if the given argument is a readable stream.

Check if the value is different from `null`, use `typeof` to check if the value is of type `object` and the `pipe` property is of type `function`.
Additionally check if the `typeof` the `_read` and `_readableState` properties are `function` and `object` respectively.

```js
const isReadableStream = val =>
  val !== null &&
  typeof val === 'object' &&
  typeof val.pipe === 'function' &&
  typeof val._read === 'function' &&
  typeof val._readableState === 'object';
```

<details>
<summary>Examples</summary>

```js
const fs = require('fs');
isReadableStream(fs.createReadStream('test.txt')); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isStream

Checks if the given argument is a stream.

Check if the value is different from `null`, use `typeof` to check if the value is of type `object` and the `pipe` property is of type `function`.

```js
const isStream = val => val !== null && typeof val === 'object' && typeof val.pipe === 'function';
```

<details>
<summary>Examples</summary>

```js
const fs = require('fs');
isStream(fs.createReadStream('test.txt')); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isTravisCI

Checks if the current environment is [Travis CI](https://travis-ci.org/).

Checks if the current environment has the `TRAVIS` and `CI` environment variables ([reference](https://docs.travis-ci.com/user/environment-variables/#Default-Environment-Variables)).

```js
const isTravisCI = () => 'TRAVIS' in process.env && 'CI' in process.env;
```

<details>
<summary>Examples</summary>

```js
isTravisCI(); // true (if code is running on Travis CI)
```

</details>

<br>[⬆ Back to top](#contents)

### isWritableStream

Checks if the given argument is a writable stream.

Check if the value is different from `null`, use `typeof` to check if the value is of type `object` and the `pipe` property is of type `function`.
Additionally check if the `typeof` the `_write` and `_writableState` properties are `function` and `object` respectively.

```js
const isWritableStream = val =>
  val !== null &&
  typeof val === 'object' &&
  typeof val.pipe === 'function' &&
  typeof val._write === 'function' &&
  typeof val._writableState === 'object';
```

<details>
<summary>Examples</summary>

```js
const fs = require('fs');
isWritableStream(fs.createWriteStream('test.txt')); // true
```

</details>

<br>[⬆ Back to top](#contents)

### JSONToFile

Writes a JSON object to a file.

Use `fs.writeFile()`, template literals and `JSON.stringify()` to write a `json` object to a `.json` file.

```js
const fs = require('fs');
const JSONToFile = (obj, filename) =>
  fs.writeFile(`${filename}.json`, JSON.stringify(obj, null, 2));
```

<details>
<summary>Examples</summary>

```js
JSONToFile({ test: 'is passed' }, 'testJsonFile'); // writes the object to 'testJsonFile.json'
```

</details>

<br>[⬆ Back to top](#contents)

### readFileLines

Returns an array of lines from the specified file.

Use `readFileSync` function in `fs` node package to create a `Buffer` from a file.
convert buffer to string using `toString(encoding)` function.
creating an array from contents of file by `split`ing file content line by line (each `\n`).

```js
const fs = require('fs');
const readFileLines = filename =>
  fs
    .readFileSync(filename)
    .toString('UTF8')
    .split('\n');
```

<details>
<summary>Examples</summary>

```js
/*
contents of test.txt :
  line1
  line2
  line3
  ___________________________
*/
let arr = readFileLines('test.txt');
console.log(arr); // ['line1', 'line2', 'line3']
```


</details>

<br>[⬆ Back to top](#contents)

### untildify

Converts a tilde path to an absolute path.

Use `String.prototype.replace()` with a regular expression and `OS.homedir()` to replace the `~` in the start of the path with the home directory.

```js
const untildify = str => str.replace(/^~($|\/|\\)/, `${require('os').homedir()}$1`);
```

<details>
<summary>Examples</summary>

```js
untildify('~/node'); // '/Users/aUser/node'
```

</details>

<br>[⬆ Back to top](#contents)

### UUIDGeneratorNode

Generates a UUID in Node.JS.

Use `crypto` API to generate a UUID, compliant with [RFC4122](https://www.ietf.org/rfc/rfc4122.txt) version 4.

```js
const crypto = require('crypto');
const UUIDGeneratorNode = () =>
  ([1e7] + -1e3 + -4e3 + -8e3 + -1e11).replace(/[018]/g, c =>
    (c ^ (crypto.randomBytes(1)[0] & (15 >> (c / 4)))).toString(16)
  );
```

<details>
<summary>Examples</summary>

```js
UUIDGeneratorNode(); // '79c7c136-60ee-40a2-beb2-856f1feabefc'
```

</details>

<br>[⬆ Back to top](#contents)


---

## 🗃️ Object

### bindAll



将对象的方法绑定到对象本身，覆盖现有方法。

使用 `Array.prototype.forEach()` 返回一个 `function` ，该函数使用 `function.prototype.apply()` 为每个指定的函数将给定的上下文(`obj`) 应用于 `fn`。

```js
const bindAll = (obj, ...fns) =>
  fns.forEach(
    fn => (
      (f = obj[fn]),
      (obj[fn] = function() {
        return f.apply(obj);
      })
    )
  );
```

<details>
<summary>Examples</summary>

```js
var view = {
  label: 'docs',
  click: function() {
    console.log('clicked ' + this.label);
  }
};
bindAll(view, 'click');
jQuery(element).on('click', view.click); // Logs 'clicked docs' when clicked.
```

</details>

<br>[⬆ Back to top](#contents)

### deepClone

Creates a deep clone of an object.

Use recursion.
Use `Object.assign()` and an empty object (`{}`) to create a shallow clone of the original.
Use `Object.keys()` and `Array.prototype.forEach()` to determine which key-value pairs need to be deep cloned.

```js
const deepClone = obj => {
  let clone = Object.assign({}, obj);
  Object.keys(clone).forEach(
    key => (clone[key] = typeof obj[key] === 'object' ? deepClone(obj[key]) : obj[key])
  );
  return Array.isArray(obj) && obj.length
    ? (clone.length = obj.length) && Array.from(clone)
    : Array.isArray(obj)
      ? Array.from(obj)
      : clone;
};
```

<details>
<summary>Examples</summary>

```js
const a = { foo: 'bar', obj: { a: 1, b: 2 } };
const b = deepClone(a); // a !== b, a.obj !== b.obj
```

</details>

<br>[⬆ Back to top](#contents)

### deepFreeze

Deep freezes an object.

Calls `Object.freeze(obj)` recursively on all unfrozen properties of passed object that are `instanceof` object.

```js
const deepFreeze = obj =>
  Object.keys(obj).forEach(
    prop =>
      !(obj[prop] instanceof Object) || Object.isFrozen(obj[prop]) ? null : deepFreeze(obj[prop])
  ) || Object.freeze(obj);
```

<details>
<summary>Examples</summary>

```js
'use strict';

const o = deepFreeze([1, [2, 3]]);

o[0] = 3; // not allowed
o[1][0] = 4; // not allowed as well
```

</details>

<br>[⬆ Back to top](#contents)

### deepGet

Returns the target value in a nested JSON object, based on the `keys` array.

Compare the keys you want in the nested JSON object as an `Array`.
Use `Array.prototype.reduce()` to get value from nested JSON object one by one. 
If the key exists in object, return target value, otherwise, return `null`.

```js
const deepGet = (obj, keys) => keys.reduce((xs, x) => (xs && xs[x] ? xs[x] : null), obj);
```

<details>
<summary>Examples</summary>

```js
let index = 2;
const data = {
  foo: {
    foz: [1, 2, 3],
    bar: {
      baz: ['a', 'b', 'c']
    }
  }
};
deepGet(data, ['foo', 'foz', index]); // get 3
deepGet(data, ['foo', 'bar', 'baz', 8, 'foz']); // null
```

</details>

<br>[⬆ Back to top](#contents)

### deepMapKeys ![advanced](/advanced.svg)

Deep maps an object keys.

Creates an object with the same values as the provided object and keys generated by running the provided function for each key.

Use `Object.keys(obj)` to iterate over the object's keys. 
Use `Array.prototype.reduce()` to create a new object with the same values and mapped keys using `fn`.

```js
const deepMapKeys = (obj, f) =>
  Array.isArray(obj)
    ? obj.map(val => deepMapKeys(val, f))
    : typeof obj === 'object'
      ? Object.keys(obj).reduce((acc, current) => {
        const val = obj[current];
        acc[f(current)] =
            val !== null && typeof val === 'object' ? deepMapKeys(val, f) : (acc[f(current)] = val);
        return acc;
      }, {})
      : obj;
```

<details>
<summary>Examples</summary>

```js
const obj = {
  foo: '1',
  nested: {
    child: {
      withArray: [
        {
          grandChild: ['hello']
        }
      ]
    }
  }
};
const upperKeysObj = deepMapKeys(obj, key => key.toUpperCase());
/*
{
  "FOO":"1",
  "NESTED":{
    "CHILD":{
      "WITHARRAY":[
        {
          "GRANDCHILD":[ 'hello' ]
        }
      ]
    }
  }
}
*/
```

</details>

<br>[⬆ Back to top](#contents)

### defaults

Assigns default values for all properties in an object that are `undefined`.

Use `Object.assign()` to create a new empty object and copy the original one to maintain key order, use `Array.prototype.reverse()` and the spread operator `...` to combine the default values from left to right, finally use `obj` again to overwrite properties that originally had a value.

```js
const defaults = (obj, ...defs) => Object.assign({}, obj, ...defs.reverse(), obj);
```

<details>
<summary>Examples</summary>

```js
defaults({ a: 1 }, { b: 2 }, { b: 6 }, { a: 3 }); // { a: 1, b: 2 }
```

</details>

<br>[⬆ Back to top](#contents)

### dig

Returns the target value in a nested JSON object, based on the given key.

Use the `in` operator to check if `target` exists in `obj`.
If found, return the value of `obj[target]`, otherwise use `Object.values(obj)` and `Array.prototype.reduce()` to recursively call `dig` on each nested object until the first matching key/value pair is found.

```js
const dig = (obj, target) =>
  target in obj
    ? obj[target]
    : Object.values(obj).reduce((acc, val) => {
      if (acc !== undefined) return acc;
      if (typeof val === 'object') return dig(val, target);
    }, undefined);
```

<details>
<summary>Examples</summary>

```js
const data = {
  level1: {
    level2: {
      level3: 'some data'
    }
  }
};
dig(data, 'level3'); // 'some data'
dig(data, 'level4'); // undefined
```

</details>

<br>[⬆ Back to top](#contents)

### equals ![advanced](/advanced.svg)

Performs a deep comparison between two values to determine if they are equivalent.

Check if the two values are identical, if they are both `Date` objects with the same time, using `Date.getTime()` or if they are both non-object values with an equivalent value (strict comparison).
Check if only one value is `null` or `undefined` or if their prototypes differ.
If none of the above conditions are met, use `Object.keys()` to check if both values have the same number of keys, then use `Array.prototype.every()` to check if every key in the first value exists in the second one and if they are equivalent by calling this method recursively.

```js
const equals = (a, b) => {
  if (a === b) return true;
  if (a instanceof Date && b instanceof Date) return a.getTime() === b.getTime();
  if (!a || !b || (typeof a !== 'object' && typeof b !== 'object')) return a === b;
  if (a === null || a === undefined || b === null || b === undefined) return false;
  if (a.prototype !== b.prototype) return false;
  let keys = Object.keys(a);
  if (keys.length !== Object.keys(b).length) return false;
  return keys.every(k => equals(a[k], b[k]));
};
```

<details>
<summary>Examples</summary>

```js
equals({ a: [2, { e: 3 }], b: [4], c: 'foo' }, { a: [2, { e: 3 }], b: [4], c: 'foo' }); // true
```

</details>

<br>[⬆ Back to top](#contents)

### findKey

Returns the first key that satisfies the provided testing function. Otherwise `undefined` is returned.

Use `Object.keys(obj)` to get all the properties of the object, `Array.prototype.find()` to test the provided function for each key-value pair. The callback receives three arguments - the value, the key and the object.

```js
const findKey = (obj, fn) => Object.keys(obj).find(key => fn(obj[key], key, obj));
```

<details>
<summary>Examples</summary>

```js
findKey(
  {
    barney: { age: 36, active: true },
    fred: { age: 40, active: false },
    pebbles: { age: 1, active: true }
  },
  o => o['active']
); // 'barney'
```

</details>

<br>[⬆ Back to top](#contents)

### findLastKey

Returns the last key that satisfies the provided testing function.
Otherwise `undefined` is returned.

Use `Object.keys(obj)` to get all the properties of the object, `Array.prototype.reverse()` to reverse their order and `Array.prototype.find()` to test the provided function for each key-value pair.
The callback receives three arguments - the value, the key and the object.

```js
const findLastKey = (obj, fn) =>
  Object.keys(obj)
    .reverse()
    .find(key => fn(obj[key], key, obj));
```

<details>
<summary>Examples</summary>

```js
findLastKey(
  {
    barney: { age: 36, active: true },
    fred: { age: 40, active: false },
    pebbles: { age: 1, active: true }
  },
  o => o['active']
); // 'pebbles'
```

</details>

<br>[⬆ Back to top](#contents)

### flattenObject

Flatten an object with the paths for keys.

Use recursion.
Use `Object.keys(obj)` combined with `Array.prototype.reduce()` to convert every leaf node to a flattened path node.
If the value of a key is an object, the function calls itself with the appropriate `prefix` to create the path using `Object.assign()`.
Otherwise, it adds the appropriate prefixed key-value pair to the accumulator object.
You should always omit the second argument, `prefix`, unless you want every key to have a prefix.

```js
const flattenObject = (obj, prefix = '') =>
  Object.keys(obj).reduce((acc, k) => {
    const pre = prefix.length ? prefix + '.' : '';
    if (typeof obj[k] === 'object') Object.assign(acc, flattenObject(obj[k], pre + k));
    else acc[pre + k] = obj[k];
    return acc;
  }, {});
```

<details>
<summary>Examples</summary>

```js
flattenObject({ a: { b: { c: 1 } }, d: 1 }); // { 'a.b.c': 1, d: 1 }
```

</details>

<br>[⬆ Back to top](#contents)

### forOwn

Iterates over all own properties of an object, running a callback for each one.

Use `Object.keys(obj)` to get all the properties of the object, `Array.prototype.forEach()` to run the provided function for each key-value pair. The callback receives three arguments - the value, the key and the object.

```js
const forOwn = (obj, fn) => Object.keys(obj).forEach(key => fn(obj[key], key, obj));
```

<details>
<summary>Examples</summary>

```js
forOwn({ foo: 'bar', a: 1 }, v => console.log(v)); // 'bar', 1
```

</details>

<br>[⬆ Back to top](#contents)

### forOwnRight

Iterates over all own properties of an object in reverse, running a callback for each one.

Use `Object.keys(obj)` to get all the properties of the object, `Array.prototype.reverse()` to reverse their order and `Array.prototype.forEach()` to run the provided function for each key-value pair. The callback receives three arguments - the value, the key and the object.

```js
const forOwnRight = (obj, fn) =>
  Object.keys(obj)
    .reverse()
    .forEach(key => fn(obj[key], key, obj));
```

<details>
<summary>Examples</summary>

```js
forOwnRight({ foo: 'bar', a: 1 }, v => console.log(v)); // 1, 'bar'
```

</details>

<br>[⬆ Back to top](#contents)

### functions

Returns an array of function property names from own (and optionally inherited) enumerable properties of an object.

Use `Object.keys(obj)` to iterate over the object's own properties.
If `inherited` is `true`, use `Object.get.PrototypeOf(obj)` to also get the object's inherited properties.
Use `Array.prototype.filter()` to keep only those properties that are functions.
Omit the second argument, `inherited`, to not include inherited properties by default.

```js
const functions = (obj, inherited = false) =>
  (inherited
    ? [...Object.keys(obj), ...Object.keys(Object.getPrototypeOf(obj))]
    : Object.keys(obj)
  ).filter(key => typeof obj[key] === 'function');
```

<details>
<summary>Examples</summary>

```js
function Foo() {
  this.a = () => 1;
  this.b = () => 2;
}
Foo.prototype.c = () => 3;
functions(new Foo()); // ['a', 'b']
functions(new Foo(), true); // ['a', 'b', 'c']
```

</details>

<br>[⬆ Back to top](#contents)

### get

Retrieve a set of properties indicated by the given selectors from an object.

Use `Array.prototype.map()` for each selector, `String.prototype.replace()` to replace square brackets with dots, `String.prototype.split('.')` to split each selector, `Array.prototype.filter()` to remove empty values and `Array.prototype.reduce()` to get the value indicated by it.

```js
const get = (from, ...selectors) =>
  [...selectors].map(s =>
    s
      .replace(/\[([^\[\]]*)\]/g, '.$1.')
      .split('.')
      .filter(t => t !== '')
      .reduce((prev, cur) => prev && prev[cur], from)
  );
```

<details>
<summary>Examples</summary>

```js
const obj = { selector: { to: { val: 'val to select' } }, target: [1, 2, { a: 'test' }] };
get(obj, 'selector.to.val', 'target[0]', 'target[2].a'); // ['val to select', 1, 'test']
```

</details>

<br>[⬆ Back to top](#contents)

### invertKeyValues

Inverts the key-value pairs of an object, without mutating it. The corresponding inverted value of each inverted key is an array of keys responsible for generating the inverted value. If a function is supplied, it is applied to each inverted key.

Use `Object.keys()` and `Array.prototype.reduce()` to invert the key-value pairs of an object and apply the function provided (if any).
Omit the second argument, `fn`, to get the inverted keys without applying a function to them.

```js
const invertKeyValues = (obj, fn) =>
  Object.keys(obj).reduce((acc, key) => {
    const val = fn ? fn(obj[key]) : obj[key];
    acc[val] = acc[val] || [];
    acc[val].push(key);
    return acc;
  }, {});
```

<details>
<summary>Examples</summary>

```js
invertKeyValues({ a: 1, b: 2, c: 1 }); // { 1: [ 'a', 'c' ], 2: [ 'b' ] }
invertKeyValues({ a: 1, b: 2, c: 1 }, value => 'group' + value); // { group1: [ 'a', 'c' ], group2: [ 'b' ] }
```

</details>

<br>[⬆ Back to top](#contents)

### lowercaseKeys

Creates a new object from the specified object, where all the keys are in lowercase.

Use `Object.keys()` and `Array.prototype.reduce()` to create a new object from the specified object.
Convert each key in the original object to lowercase, using `String.toLowerCase()`.

```js
const lowercaseKeys = obj =>
  Object.keys(obj).reduce((acc, key) => {
    acc[key.toLowerCase()] = obj[key];
    return acc;
  }, {});
```

<details>
<summary>Examples</summary>

```js
const myObj = { Name: 'Adam', sUrnAME: 'Smith' };
const myObjLower = lowercaseKeys(myObj); // {name: 'Adam', surname: 'Smith'};
```

</details>

<br>[⬆ Back to top](#contents)

### mapKeys

Creates an object with keys generated by running the provided function for each key and the same values as the provided object.

Use `Object.keys(obj)` to iterate over the object's keys.
Use `Array.prototype.reduce()` to create a new object with the same values and mapped keys using `fn`.

```js
const mapKeys = (obj, fn) =>
  Object.keys(obj).reduce((acc, k) => {
    acc[fn(obj[k], k, obj)] = obj[k];
    return acc;
  }, {});
```

<details>
<summary>Examples</summary>

```js
mapKeys({ a: 1, b: 2 }, (val, key) => key + val); // { a1: 1, b2: 2 }
```

</details>

<br>[⬆ Back to top](#contents)

### mapValues

Creates an object with the same keys as the provided object and values generated by running the provided function for each value.

Use `Object.keys(obj)` to iterate over the object's keys.
Use `Array.prototype.reduce()` to create a new object with the same keys and mapped values using `fn`.

```js
const mapValues = (obj, fn) =>
  Object.keys(obj).reduce((acc, k) => {
    acc[k] = fn(obj[k], k, obj);
    return acc;
  }, {});
```

<details>
<summary>Examples</summary>

```js
const users = {
  fred: { user: 'fred', age: 40 },
  pebbles: { user: 'pebbles', age: 1 }
};
mapValues(users, u => u.age); // { fred: 40, pebbles: 1 }
```

</details>

<br>[⬆ Back to top](#contents)

### matches

Compares two objects to determine if the first one contains equivalent property values to the second one.

Use `Object.keys(source)` to get all the keys of the second object, then `Array.prototype.every()`, `Object.hasOwnProperty()` and strict comparison to determine if all keys exist in the first object and have the same values.

```js
const matches = (obj, source) =>
  Object.keys(source).every(key => obj.hasOwnProperty(key) && obj[key] === source[key]);
```

<details>
<summary>Examples</summary>

```js
matches({ age: 25, hair: 'long', beard: true }, { hair: 'long', beard: true }); // true
matches({ hair: 'long', beard: true }, { age: 25, hair: 'long', beard: true }); // false
```

</details>

<br>[⬆ Back to top](#contents)

### matchesWith

Compares two objects to determine if the first one contains equivalent property values to the second one, based on a provided function.

Use `Object.keys(source)` to get all the keys of the second object, then `Array.prototype.every()`, `Object.hasOwnProperty()` and the provided function to determine if all keys exist in the first object and have equivalent values.
If no function is provided, the values will be compared using the equality operator.

```js
const matchesWith = (obj, source, fn) =>
  Object.keys(source).every(
    key =>
      obj.hasOwnProperty(key) && fn
        ? fn(obj[key], source[key], key, obj, source)
        : obj[key] == source[key]
  );
```

<details>
<summary>Examples</summary>

```js
const isGreeting = val => /^h(?:i|ello)$/.test(val);
matchesWith(
  { greeting: 'hello' },
  { greeting: 'hi' },
  (oV, sV) => isGreeting(oV) && isGreeting(sV)
); // true
```

</details>

<br>[⬆ Back to top](#contents)

### merge

Creates a new object from the combination of two or more objects.

Use `Array.prototype.reduce()` combined with `Object.keys(obj)` to iterate over all objects and keys.
Use `hasOwnProperty()` and `Array.prototype.concat()` to append values for keys existing in multiple objects.

```js
const merge = (...objs) =>
  [...objs].reduce(
    (acc, obj) =>
      Object.keys(obj).reduce((a, k) => {
        acc[k] = acc.hasOwnProperty(k) ? [].concat(acc[k]).concat(obj[k]) : obj[k];
        return acc;
      }, {}),
    {}
  );
```

<details>
<summary>Examples</summary>

```js
const object = {
  a: [{ x: 2 }, { y: 4 }],
  b: 1
};
const other = {
  a: { z: 3 },
  b: [2, 3],
  c: 'foo'
};
merge(object, other); // { a: [ { x: 2 }, { y: 4 }, { z: 3 } ], b: [ 1, 2, 3 ], c: 'foo' }
```

</details>

<br>[⬆ Back to top](#contents)

### nest

Given a flat array of objects linked to one another, it will nest them recursively.
Useful for nesting comments, such as the ones on reddit.com.

Use recursion.
Use `Array.prototype.filter()` to filter the items where the `id` matches the `link`, then `Array.prototype.map()` to map each one to a new object that has a `children` property which recursively nests the items based on which ones are children of the current item.
Omit the second argument, `id`, to default to `null` which indicates the object is not linked to another one (i.e. it is a top level object).
Omit the third argument, `link`, to use `'parent_id'` as the default property which links the object to another one by its `id`.

```js
const nest = (items, id = null, link = 'parent_id') =>
  items
    .filter(item => item[link] === id)
    .map(item => ({ ...item, children: nest(items, item.id) }));
```

<details>
<summary>Examples</summary>

```js
// One top level comment
const comments = [
  { id: 1, parent_id: null },
  { id: 2, parent_id: 1 },
  { id: 3, parent_id: 1 },
  { id: 4, parent_id: 2 },
  { id: 5, parent_id: 4 }
];
const nestedComments = nest(comments); // [{ id: 1, parent_id: null, children: [...] }]
```


</details>

<br>[⬆ Back to top](#contents)

### objectFromPairs

Creates an object from the given key-value pairs.

Use `Array.prototype.reduce()` to create and combine key-value pairs.

```js
const objectFromPairs = arr => arr.reduce((a, [key, val]) => ((a[key] = val), a), {});
```

<details>
<summary>Examples</summary>

```js
objectFromPairs([['a', 1], ['b', 2]]); // {a: 1, b: 2}
```

</details>

<br>[⬆ Back to top](#contents)

### objectToPairs

Creates an array of key-value pair arrays from an object.

Use `Object.keys()` and `Array.prototype.map()` to iterate over the object's keys and produce an array with key-value pairs.

```js
const objectToPairs = obj => Object.keys(obj).map(k => [k, obj[k]]);
```

<details>
<summary>Examples</summary>

```js
objectToPairs({ a: 1, b: 2 }); // [ ['a', 1], ['b', 2] ]
```

</details>

<br>[⬆ Back to top](#contents)

### omit

Omits the key-value pairs corresponding to the given keys from an object.

Use `Object.keys(obj)`, `Array.prototype.filter()` and `Array.prototype.includes()` to remove the provided keys.
Use `Array.prototype.reduce()` to convert the filtered keys back to an object with the corresponding key-value pairs.

```js
const omit = (obj, arr) =>
  Object.keys(obj)
    .filter(k => !arr.includes(k))
    .reduce((acc, key) => ((acc[key] = obj[key]), acc), {});
```

<details>
<summary>Examples</summary>

```js
omit({ a: 1, b: '2', c: 3 }, ['b']); // { 'a': 1, 'c': 3 }
```

</details>

<br>[⬆ Back to top](#contents)

### omitBy

Creates an object composed of the properties the given function returns falsy for. The function is invoked with two arguments: (value, key).

Use `Object.keys(obj)` and `Array.prototype.filter()`to remove the keys for which `fn` returns a truthy value.
Use `Array.prototype.reduce()` to convert the filtered keys back to an object with the corresponding key-value pairs.

```js
const omitBy = (obj, fn) =>
  Object.keys(obj)
    .filter(k => !fn(obj[k], k))
    .reduce((acc, key) => ((acc[key] = obj[key]), acc), {});
```

<details>
<summary>Examples</summary>

```js
omitBy({ a: 1, b: '2', c: 3 }, x => typeof x === 'number'); // { b: '2' }
```

</details>

<br>[⬆ Back to top](#contents)

### orderBy

Returns a sorted array of objects ordered by properties and orders.

Uses `Array.prototype.sort()`, `Array.prototype.reduce()` on the `props` array with a default value of `0`, use array destructuring to swap the properties position depending on the order passed.
If no `orders` array is passed it sort by `'asc'` by default.

```js
const orderBy = (arr, props, orders) =>
  [...arr].sort((a, b) =>
    props.reduce((acc, prop, i) => {
      if (acc === 0) {
        const [p1, p2] = orders && orders[i] === 'desc' ? [b[prop], a[prop]] : [a[prop], b[prop]];
        acc = p1 > p2 ? 1 : p1 < p2 ? -1 : 0;
      }
      return acc;
    }, 0)
  );
```

<details>
<summary>Examples</summary>

```js
const users = [{ name: 'fred', age: 48 }, { name: 'barney', age: 36 }, { name: 'fred', age: 40 }];
orderBy(users, ['name', 'age'], ['asc', 'desc']); // [{name: 'barney', age: 36}, {name: 'fred', age: 48}, {name: 'fred', age: 40}]
orderBy(users, ['name', 'age']); // [{name: 'barney', age: 36}, {name: 'fred', age: 40}, {name: 'fred', age: 48}]
```

</details>

<br>[⬆ Back to top](#contents)

### pick

Picks the key-value pairs corresponding to the given keys from an object.

Use `Array.prototype.reduce()` to convert the filtered/picked keys back to an object with the corresponding key-value pairs if the key exists in the object.

```js
const pick = (obj, arr) =>
  arr.reduce((acc, curr) => (curr in obj && (acc[curr] = obj[curr]), acc), {});
```

<details>
<summary>Examples</summary>

```js
pick({ a: 1, b: '2', c: 3 }, ['a', 'c']); // { 'a': 1, 'c': 3 }
```

</details>

<br>[⬆ Back to top](#contents)

### pickBy

Creates an object composed of the properties the given function returns truthy for. The function is invoked with two arguments: (value, key).

Use `Object.keys(obj)` and `Array.prototype.filter()`to remove the keys for which `fn` returns a falsy value.
Use `Array.prototype.reduce()` to convert the filtered keys back to an object with the corresponding key-value pairs.

```js
const pickBy = (obj, fn) =>
  Object.keys(obj)
    .filter(k => fn(obj[k], k))
    .reduce((acc, key) => ((acc[key] = obj[key]), acc), {});
```

<details>
<summary>Examples</summary>

```js
pickBy({ a: 1, b: '2', c: 3 }, x => typeof x === 'number'); // { 'a': 1, 'c': 3 }
```

</details>

<br>[⬆ Back to top](#contents)

### renameKeys

Replaces the names of multiple object keys with the values provided.

Use `Object.keys()` in combination with `Array.prototype.reduce()` and the spread operator (`...`) to get the object's keys and rename them according to `keysMap`.

```js
const renameKeys = (keysMap, obj) =>
  Object.keys(obj).reduce(
    (acc, key) => ({
      ...acc,
      ...{ [keysMap[key] || key]: obj[key] }
    }),
    {}
  );
```

<details>
<summary>Examples</summary>

```js
const obj = { name: 'Bobo', job: 'Front-End Master', shoeSize: 100 };
renameKeys({ name: 'firstName', job: 'passion' }, obj); // { firstName: 'Bobo', passion: 'Front-End Master', shoeSize: 100 }
```

</details>

<br>[⬆ Back to top](#contents)

### shallowClone

Creates a shallow clone of an object.

Use `Object.assign()` and an empty object (`{}`) to create a shallow clone of the original.

```js
const shallowClone = obj => Object.assign({}, obj);
```

<details>
<summary>Examples</summary>

```js
const a = { x: true, y: 1 };
const b = shallowClone(a); // a !== b
```

</details>

<br>[⬆ Back to top](#contents)

### size

Get size of arrays, objects or strings.

Get type of `val` (`array`, `object` or `string`). 
Use `length` property for arrays.
Use `length` or `size` value if available or number of keys for objects.
Use `size` of a [`Blob` object](https://developer.mozilla.org/en-US/docs/Web/API/Blob) created from `val` for strings.

Split strings into array of characters with `split('')` and return its length.

```js
const size = val =>
  Array.isArray(val)
    ? val.length
    : val && typeof val === 'object'
      ? val.size || val.length || Object.keys(val).length
      : typeof val === 'string'
        ? new Blob([val]).size
        : 0;
```

<details>
<summary>Examples</summary>

```js
size([1, 2, 3, 4, 5]); // 5
size('size'); // 4
size({ one: 1, two: 2, three: 3 }); // 3
```

</details>

<br>[⬆ Back to top](#contents)

### transform

Applies a function against an accumulator and each key in the object (from left to right).

Use `Object.keys(obj)` to iterate over each key in the object, `Array.prototype.reduce()` to call the apply the specified function against the given accumulator.

```js
const transform = (obj, fn, acc) => Object.keys(obj).reduce((a, k) => fn(a, obj[k], k, obj), acc);
```

<details>
<summary>Examples</summary>

```js
transform(
  { a: 1, b: 2, c: 1 },
  (r, v, k) => {
    (r[v] || (r[v] = [])).push(k);
    return r;
  },
  {}
); // { '1': ['a', 'c'], '2': ['b'] }
```

</details>

<br>[⬆ Back to top](#contents)

### truthCheckCollection

Checks if the predicate (second argument) is truthy on all elements of a collection (first argument).

Use `Array.prototype.every()` to check if each passed object has the specified property and if it returns a truthy value.

```js
const truthCheckCollection = (collection, pre) => collection.every(obj => obj[pre]);
```

<details>
<summary>Examples</summary>

```js
truthCheckCollection([{ user: 'Tinky-Winky', sex: 'male' }, { user: 'Dipsy', sex: 'male' }], 'sex'); // true
```

</details>

<br>[⬆ Back to top](#contents)

### unflattenObject ![advanced](/advanced.svg)

Unflatten an object with the paths for keys.

Use `Object.keys(obj)` combined with `Array.prototype.reduce()` to convert flattened path node to a leaf node.
If the value of a key contains a dot delimiter (`.`), use `Array.prototype.split('.')`, string transformations and `JSON.parse()` to create an object, then `Object.assign()` to create the leaf node.
Otherwise, add the appropriate key-value pair to the accumulator object.

```js
const unflattenObject = obj =>
  Object.keys(obj).reduce((acc, k) => {
    if (k.indexOf('.') !== -1) {
      const keys = k.split('.');
      Object.assign(
        acc,
        JSON.parse(
          '{' +
            keys.map((v, i) => (i !== keys.length - 1 ? `"${v}":{` : `"${v}":`)).join('') +
            obj[k] +
            '}'.repeat(keys.length)
        )
      );
    } else acc[k] = obj[k];
    return acc;
  }, {});
```

<details>
<summary>Examples</summary>

```js
unflattenObject({ 'a.b.c': 1, d: 1 }); // { a: { b: { c: 1 } }, d: 1 }
```

</details>

<br>[⬆ Back to top](#contents)


---

## 📜 String

### byteSize

Returns the length of a string in bytes.

Convert a given string to a [`Blob` Object](https://developer.mozilla.org/en-US/docs/Web/API/Blob) and find its `size`.

以字节为单位返回字符串的长度。

将给定的字符串转换为[`Blob Object`]（https://developer.mozilla.org/en-US/docs/Web/API/Blob）并找到它的`size`。

```js
const byteSize = str => new Blob([str]).size;
```

<details>
<summary>Examples</summary>

```js
byteSize('😀'); // 4
byteSize('Hello World'); // 11
```

</details>

<br>[⬆ Back to top](#contents)

### capitalize

Capitalizes the first letter of a string.

Use array destructuring and `String.prototype.toUpperCase()` to capitalize first letter, `...rest` to get array of characters after first letter and then `Array.prototype.join('')` to make it a string again.
Omit the `lowerRest` parameter to keep the rest of the string intact, or set it to `true` to convert to lowercase.


将字符串的第一个字母大写。

使用数组解构和 `String.prototype.toUpperCase()` 把第一个字母大写，`...rest ` 获取第一个字母后的字符组成的数组，然后 `array .prototype.join(")` 将其再次变为字符串。
省略 `lowerRest` 参数保持字符串的其余部分不变，或将其设置为 `true` 将字符串的剩余部分都转换为小写。

```js
const capitalize = ([first, ...rest], lowerRest = false) =>
  first.toUpperCase() + (lowerRest ? rest.join('').toLowerCase() : rest.join(''));
```

<details>
<summary>Examples</summary>

```js
capitalize('fooBar'); // 'FooBar'
capitalize('fooBar', true); // 'Foobar'
```

</details>

<br>[⬆ Back to top](#contents)

### capitalizeEveryWord

Capitalizes the first letter of every word in a string.

Use `String.prototype.replace()` to match the first character of each word and `String.prototype.toUpperCase()` to capitalize it.

将字符串中每个单词的第一个字母大写。

使用 `String.prototype.replace()` 匹配每个单词的第一个字符，并使用 `String.prototype.toUpperCase()` 将其大写。


```js
const capitalizeEveryWord = str => str.replace(/\b[a-z]/g, char => char.toUpperCase());
```

<details>
<summary>Examples</summary>

```js
capitalizeEveryWord('hello world!'); // 'Hello World!'
```

</details>

<br>[⬆ Back to top](#contents)

### compactWhitespace

Returns a string with whitespaces compacted.

Use `String.prototype.replace()` with a regular expression to replace all occurrences of 2 or more whitespace characters with a single space.

返回替换空白字符后的字符串。

使用 `String.prototype.replace()` 将正则表达式匹配到的2个或更多空白字符替换为1个空白字符。

```js
const compactWhitespace = str => str.replace(/\s{2,}/g, ' ');
```

<details>
<summary>Examples</summary>

```js
compactWhitespace('Lorem    Ipsum'); // 'Lorem Ipsum'
compactWhitespace('Lorem \n Ipsum'); // 'Lorem Ipsum'
```

</details>

<br>[⬆ Back to top](#contents)

### CSVToArray

Converts a comma-separated values (CSV) string to a 2D array.

Use `Array.prototype.slice()` and `Array.prototype.indexOf('\n')` to remove the first row (title row) if `omitFirstRow` is `true`.
Use `String.prototype.split('\n')` to create a string for each row, then `String.prototype.split(delimiter)` to separate the values in each row.
Omit the second argument, `delimiter`, to use a default delimiter of `,`.
Omit the third argument, `omitFirstRow`, to include the first row (title row) of the CSV string.

```js
const CSVToArray = (data, delimiter = ',', omitFirstRow = false) =>
  data
    .slice(omitFirstRow ? data.indexOf('\n') + 1 : 0)
    .split('\n')
    .map(v => v.split(delimiter));
```

<details>
<summary>Examples</summary>

```js
CSVToArray('a,b\nc,d'); // [['a','b'],['c','d']];
CSVToArray('a;b\nc;d', ';'); // [['a','b'],['c','d']];
CSVToArray('col1,col2\na,b\nc,d', ',', true); // [['a','b'],['c','d']];
```

</details>

<br>[⬆ Back to top](#contents)

### CSVToJSON ![advanced](/advanced.svg)

Converts a comma-separated values (CSV) string to a 2D array of objects.
The first row of the string is used as the title row.

Use `Array.prototype.slice()` and `Array.prototype.indexOf('\n')` and `String.prototype.split(delimiter)` to separate the first row (title row) into values.
Use `String.prototype.split('\n')` to create a string for each row, then `Array.prototype.map()` and `String.prototype.split(delimiter)` to separate the values in each row.
Use `Array.prototype.reduce()` to create an object for each row's values, with the keys parsed from the title row.
Omit the second argument, `delimiter`, to use a default delimiter of `,`.

```js
const CSVToJSON = (data, delimiter = ',') => {
  const titles = data.slice(0, data.indexOf('\n')).split(delimiter);
  return data
    .slice(data.indexOf('\n') + 1)
    .split('\n')
    .map(v => {
      const values = v.split(delimiter);
      return titles.reduce((obj, title, index) => ((obj[title] = values[index]), obj), {});
    });
};
```

<details>
<summary>Examples</summary>

```js
CSVToJSON('col1,col2\na,b\nc,d'); // [{'col1': 'a', 'col2': 'b'}, {'col1': 'c', 'col2': 'd'}];
CSVToJSON('col1;col2\na;b\nc;d', ';'); // [{'col1': 'a', 'col2': 'b'}, {'col1': 'c', 'col2': 'd'}];
```

</details>

<br>[⬆ Back to top](#contents)

### decapitalize

Decapitalizes the first letter of a string.

Use array destructuring and `String.toLowerCase()` to decapitalize first letter, `...rest` to get array of characters after first letter and then `Array.prototype.join('')` to make it a string again.
Omit the `upperRest` parameter to keep the rest of the string intact, or set it to `true` to convert to uppercase.

```js
const decapitalize = ([first, ...rest], upperRest = false) =>
  first.toLowerCase() + (upperRest ? rest.join('').toUpperCase() : rest.join(''));
```

<details>
<summary>Examples</summary>

```js
decapitalize('FooBar'); // 'fooBar'
decapitalize('FooBar', true); // 'fOOBAR'
```

</details>

<br>[⬆ Back to top](#contents)

### escapeHTML

Escapes a string for use in HTML.

Use `String.prototype.replace()` with a regexp that matches the characters that need to be escaped, using a callback function to replace each character instance with its associated escaped character using a dictionary (object).

```js
const escapeHTML = str =>
  str.replace(
    /[&<>'"]/g,
    tag =>
      ({
        '&': '&amp;',
        '<': '&lt;',
        '>': '&gt;',
        "'": '&#39;',
        '"': '&quot;'
      }[tag] || tag)
  );
```

<details>
<summary>Examples</summary>

```js
escapeHTML('<a href="#">Me & you</a>'); // '&lt;a href=&quot;#&quot;&gt;Me &amp; you&lt;/a&gt;'
```

</details>

<br>[⬆ Back to top](#contents)

### escapeRegExp

Escapes a string to use in a regular expression.

Use `String.prototype.replace()` to escape special characters.

```js
const escapeRegExp = str => str.replace(/[.*+?^${}()|[\]\\]/g, '\\$&');
```

<details>
<summary>Examples</summary>

```js
escapeRegExp('(test)'); // \\(test\\)
```

</details>

<br>[⬆ Back to top](#contents)

### fromCamelCase

Converts a string from camelcase.

Use `String.prototype.replace()` to remove underscores, hyphens, and spaces and convert words to camelcase.
Omit the second argument to use a default `separator` of `_`.

```js
const fromCamelCase = (str, separator = '_') =>
  str
    .replace(/([a-z\d])([A-Z])/g, '$1' + separator + '$2')
    .replace(/([A-Z]+)([A-Z][a-z\d]+)/g, '$1' + separator + '$2')
    .toLowerCase();
```

<details>
<summary>Examples</summary>

```js
fromCamelCase('someDatabaseFieldName', ' '); // 'some database field name'
fromCamelCase('someLabelThatNeedsToBeCamelized', '-'); // 'some-label-that-needs-to-be-camelized'
fromCamelCase('someJavascriptProperty', '_'); // 'some_javascript_property'
```

</details>

<br>[⬆ Back to top](#contents)

### indentString

Indents each line in the provided string.

Use `String.replace` and a regular expression to add the character specified by `indent` `count` times at the start of each line.
Omit the third parameter, `indent`, to use a default indentation character of `' '`.

```js
const indentString = (str, count, indent = ' ') => str.replace(/^/gm, indent.repeat(count));
```

<details>
<summary>Examples</summary>

```js
indentString('Lorem\nIpsum', 2); // '  Lorem\n  Ipsum'
indentString('Lorem\nIpsum', 2, '_'); // '__Lorem\n__Ipsum'
```

</details>

<br>[⬆ Back to top](#contents)

### isAbsoluteURL

Returns `true` if the given string is an absolute URL, `false` otherwise.

Use a regular expression to test if the string is an absolute URL.

```js
const isAbsoluteURL = str => /^[a-z][a-z0-9+.-]*:/.test(str);
```

<details>
<summary>Examples</summary>

```js
isAbsoluteURL('https://google.com'); // true
isAbsoluteURL('ftp://www.myserver.net'); // true
isAbsoluteURL('/foo/bar'); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isAnagram

Checks if a string is an anagram of another string (case-insensitive, ignores spaces, punctuation and special characters).

Use `String.toLowerCase()`, `String.prototype.replace()` with an appropriate regular expression to remove unnecessary characters, `String.prototype.split('')`, `Array.prototype.sort()` and `Array.prototype.join('')` on both strings to normalize them, then check if their normalized forms are equal.

```js
const isAnagram = (str1, str2) => {
  const normalize = str =>
    str
      .toLowerCase()
      .replace(/[^a-z0-9]/gi, '')
      .split('')
      .sort()
      .join('');
  return normalize(str1) === normalize(str2);
};
```

<details>
<summary>Examples</summary>

```js
isAnagram('iceman', 'cinema'); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isLowerCase

Checks if a string is lower case.

Convert the given string to lower case, using `String.toLowerCase()` and compare it to the original.

```js
const isLowerCase = str => str === str.toLowerCase();
```

<details>
<summary>Examples</summary>

```js
isLowerCase('abc'); // true
isLowerCase('a3@$'); // true
isLowerCase('Ab4'); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isUpperCase

Checks if a string is upper case.

Convert the given string to upper case, using `String.prototype.toUpperCase()` and compare it to the original.


```js
const isUpperCase = str => str === str.toUpperCase();
```

<details>
<summary>Examples</summary>

```js
isUpperCase('ABC'); // true
isLowerCase('A3@$'); // true
isLowerCase('aB4'); // false
```

</details>

<br>[⬆ Back to top](#contents)

### mapString

Creates a new string with the results of calling a provided function on every character in the calling string.

Use `String.prototype.split('')` and `Array.prototype.map()` to call the provided function, `fn`, for each character in `str`.
Use `Array.prototype.join('')` to recombine the array of characters into a string.
The callback function, `fn`, takes three arguments (the current character, the index of the current character and the string `mapString` was called upon).

```js
const mapString = (str, fn) =>
  str
    .split('')
    .map((c, i) => fn(c, i, str))
    .join('');
```

<details>
<summary>Examples</summary>

```js
mapString('lorem ipsum', c => c.toUpperCase()); // 'LOREM IPSUM'
```

</details>

<br>[⬆ Back to top](#contents)

### mask

Replaces all but the last `num` of characters with the specified mask character.

Use `String.prototype.slice()` to grab the portion of the characters that will remain unmasked and use `String.padStart()` to fill the beginning of the string with the mask character up to the original length.
Omit the second argument, `num`, to keep a default of `4` characters unmasked. If `num` is negative, the unmasked characters will be at the start of the string.
Omit the third argument, `mask`, to use a default character of `'*'` for the mask.

```js
const mask = (cc, num = 4, mask = '*') => `${cc}`.slice(-num).padStart(`${cc}`.length, mask);
```

<details>
<summary>Examples</summary>

```js
mask(1234567890); // '******7890'
mask(1234567890, 3); // '*******890'
mask(1234567890, -4, '$'); // '$$$$567890'
```

</details>

<br>[⬆ Back to top](#contents)

### pad

Pads a string on both sides with the specified character, if it's shorter than the specified length.

Use `String.padStart()` and `String.padEnd()` to pad both sides of the given string.
Omit the third argument, `char`, to use the whitespace character as the default padding character.

```js
const pad = (str, length, char = ' ') =>
  str.padStart((str.length + length) / 2, char).padEnd(length, char);
```

<details>
<summary>Examples</summary>

```js
pad('cat', 8); // '  cat   '
pad(String(42), 6, '0'); // '004200'
pad('foobar', 3); // 'foobar'
```

</details>

<br>[⬆ Back to top](#contents)

### palindrome

Returns `true` if the given string is a palindrome, `false` otherwise.

Convert the string to `String.prototype.toLowerCase()` and use `String.prototype.replace()` to remove non-alphanumeric characters from it.
Then, use the spread operator (`...`) to split the string into individual characters, `Array.prototype.reverse()`, `String.prototype.join('')` and compare it to the original, unreversed string, after converting it to `String.prototype.toLowerCase()`.

```js
const palindrome = str => {
  const s = str.toLowerCase().replace(/[\W_]/g, '');
  return s === [...s].reverse().join('');
};
```

<details>
<summary>Examples</summary>

```js
palindrome('taco cat'); // true
```

</details>

<br>[⬆ Back to top](#contents)

### pluralize

Returns the singular or plural form of the word based on the input number. If the first argument is an `object`, it will use a closure by returning a function that can auto-pluralize words that don't simply end in `s` if the supplied dictionary contains the word.

If `num` is either `-1` or `1`, return the singular form of the word. If `num` is any other number, return the plural form. Omit the third argument to use the default of the singular word + `s`, or supply a custom pluralized word when necessary. If the first argument is an `object`, utilize a closure by returning a function which can use the supplied dictionary to resolve the correct plural form of the word.

```js
const pluralize = (val, word, plural = word + 's') => {
  const _pluralize = (num, word, plural = word + 's') =>
    [1, -1].includes(Number(num)) ? word : plural;
  if (typeof val === 'object') return (num, word) => _pluralize(num, word, val[word]);
  return _pluralize(val, word, plural);
};
```

<details>
<summary>Examples</summary>

```js
pluralize(0, 'apple'); // 'apples'
pluralize(1, 'apple'); // 'apple'
pluralize(2, 'apple'); // 'apples'
pluralize(2, 'person', 'people'); // 'people'

const PLURALS = {
  person: 'people',
  radius: 'radii'
};
const autoPluralize = pluralize(PLURALS);
autoPluralize(2, 'person'); // 'people'
```

</details>

<br>[⬆ Back to top](#contents)

### removeNonASCII

Removes non-printable ASCII characters.

Use a regular expression to remove non-printable ASCII characters.

```js
const removeNonASCII = str => str.replace(/[^\x20-\x7E]/g, '');
```

<details>
<summary>Examples</summary>

```js
removeNonASCII('äÄçÇéÉêlorem-ipsumöÖÐþúÚ'); // 'lorem-ipsum'
```

</details>

<br>[⬆ Back to top](#contents)

### reverseString

Reverses a string.

Use the spread operator (`...`) and `Array.prototype.reverse()` to reverse the order of the characters in the string.
Combine characters to get a string using `String.prototype.join('')`.

```js
const reverseString = str => [...str].reverse().join('');
```

<details>
<summary>Examples</summary>

```js
reverseString('foobar'); // 'raboof'
```

</details>

<br>[⬆ Back to top](#contents)

### sortCharactersInString

Alphabetically sorts the characters in a string.

Use the spread operator (`...`), `Array.prototype.sort()` and  `String.localeCompare()` to sort the characters in `str`, recombine using `String.prototype.join('')`.

```js
const sortCharactersInString = str => [...str].sort((a, b) => a.localeCompare(b)).join('');
```

<details>
<summary>Examples</summary>

```js
sortCharactersInString('cabbage'); // 'aabbceg'
```

</details>

<br>[⬆ Back to top](#contents)

### splitLines

Splits a multiline string into an array of lines.

Use `String.prototype.split()` and a regular expression to match line breaks and create an array.

```js
const splitLines = str => str.split(/\r?\n/);
```

<details>
<summary>Examples</summary>

```js
splitLines('This\nis a\nmultiline\nstring.\n'); // ['This', 'is a', 'multiline', 'string.' , '']
```

</details>

<br>[⬆ Back to top](#contents)

### stringPermutations ![advanced](/advanced.svg)

⚠️ **WARNING**: This function's execution time increases exponentially with each character. Anything more than 8 to 10 characters will cause your browser to hang as it tries to solve all the different combinations.

Generates all permutations of a string (contains duplicates).

Use recursion.
For each letter in the given string, create all the partial permutations for the rest of its letters.
Use `Array.prototype.map()` to combine the letter with each partial permutation, then `Array.prototype.reduce()` to combine all permutations in one array.
Base cases are for string `length` equal to `2` or `1`.

```js
const stringPermutations = str => {
  if (str.length <= 2) return str.length === 2 ? [str, str[1] + str[0]] : [str];
  return str
    .split('')
    .reduce(
      (acc, letter, i) =>
        acc.concat(stringPermutations(str.slice(0, i) + str.slice(i + 1)).map(val => letter + val)),
      []
    );
};
```

<details>
<summary>Examples</summary>

```js
stringPermutations('abc'); // ['abc','acb','bac','bca','cab','cba']
```

</details>

<br>[⬆ Back to top](#contents)

### stripHTMLTags

Removes HTML/XML tags from string.

Use a regular expression to remove HTML/XML tags from a string.

```js
const stripHTMLTags = str => str.replace(/<[^>]*>/g, '');
```

<details>
<summary>Examples</summary>

```js
stripHTMLTags('<p><em>lorem</em> <strong>ipsum</strong></p>'); // 'lorem ipsum'
```

</details>

<br>[⬆ Back to top](#contents)

### toCamelCase

Converts a string to camelcase.

Break the string into words and combine them capitalizing the first letter of each word, using a regexp.

```js
const toCamelCase = str => {
  let s =
    str &&
    str
      .match(/[A-Z]{2,}(?=[A-Z][a-z]+[0-9]*|\b)|[A-Z]?[a-z]+[0-9]*|[A-Z]|[0-9]+/g)
      .map(x => x.slice(0, 1).toUpperCase() + x.slice(1).toLowerCase())
      .join('');
  return s.slice(0, 1).toLowerCase() + s.slice(1);
};
```

<details>
<summary>Examples</summary>

```js
toCamelCase('some_database_field_name'); // 'someDatabaseFieldName'
toCamelCase('Some label that needs to be camelized'); // 'someLabelThatNeedsToBeCamelized'
toCamelCase('some-javascript-property'); // 'someJavascriptProperty'
toCamelCase('some-mixed_string with spaces_underscores-and-hyphens'); // 'someMixedStringWithSpacesUnderscoresAndHyphens'
```

</details>

<br>[⬆ Back to top](#contents)

### toKebabCase

Converts a string to kebab case.

Break the string into words and combine them adding `-` as a separator, using a regexp.

```js
const toKebabCase = str =>
  str &&
  str
    .match(/[A-Z]{2,}(?=[A-Z][a-z]+[0-9]*|\b)|[A-Z]?[a-z]+[0-9]*|[A-Z]|[0-9]+/g)
    .map(x => x.toLowerCase())
    .join('-');
```

<details>
<summary>Examples</summary>

```js
toKebabCase('camelCase'); // 'camel-case'
toKebabCase('some text'); // 'some-text'
toKebabCase('some-mixed_string With spaces_underscores-and-hyphens'); // 'some-mixed-string-with-spaces-underscores-and-hyphens'
toKebabCase('AllThe-small Things'); // "all-the-small-things"
toKebabCase('IAmListeningToFMWhileLoadingDifferentURLOnMyBrowserAndAlsoEditingSomeXMLAndHTML'); // "i-am-listening-to-fm-while-loading-different-url-on-my-browser-and-also-editing-xml-and-html"
```

</details>

<br>[⬆ Back to top](#contents)

### toSnakeCase

Converts a string to snake case.

Break the string into words and combine them adding `_` as a separator, using a regexp.

```js
const toSnakeCase = str =>
  str &&
  str
    .match(/[A-Z]{2,}(?=[A-Z][a-z]+[0-9]*|\b)|[A-Z]?[a-z]+[0-9]*|[A-Z]|[0-9]+/g)
    .map(x => x.toLowerCase())
    .join('_');
```

<details>
<summary>Examples</summary>

```js
toSnakeCase('camelCase'); // 'camel_case'
toSnakeCase('some text'); // 'some_text'
toSnakeCase('some-mixed_string With spaces_underscores-and-hyphens'); // 'some_mixed_string_with_spaces_underscores_and_hyphens'
toSnakeCase('AllThe-small Things'); // "all_the_smal_things"
toSnakeCase('IAmListeningToFMWhileLoadingDifferentURLOnMyBrowserAndAlsoEditingSomeXMLAndHTML'); // "i_am_listening_to_fm_while_loading_different_url_on_my_browser_and_also_editing_some_xml_and_html"
```

</details>

<br>[⬆ Back to top](#contents)

### toTitleCase

Converts a string to title case.

Break the string into words, using a regexp, and combine them capitalizing the first letter of each word and adding a whitespace between them.

```js
const toTitleCase = str =>
  str
    .match(/[A-Z]{2,}(?=[A-Z][a-z]+[0-9]*|\b)|[A-Z]?[a-z]+[0-9]*|[A-Z]|[0-9]+/g)
    .map(x => x.charAt(0).toUpperCase() + x.slice(1))
    .join(' ');
```

<details>
<summary>Examples</summary>

```js
toTitleCase('some_database_field_name'); // 'Some Database Field Name'
toTitleCase('Some label that needs to be title-cased'); // 'Some Label That Needs To Be Title Cased'
toTitleCase('some-package-name'); // 'Some Package Name'
toTitleCase('some-mixed_string with spaces_underscores-and-hyphens'); // 'Some Mixed String With Spaces Underscores And Hyphens'
```

</details>

<br>[⬆ Back to top](#contents)

### truncateString

Truncates a string up to a specified length.

Determine if the string's `length` is greater than `num`.
Return the string truncated to the desired length, with `'...'` appended to the end or the original string.

```js
const truncateString = (str, num) =>
  str.length > num ? str.slice(0, num > 3 ? num - 3 : num) + '...' : str;
```

<details>
<summary>Examples</summary>

```js
truncateString('boomerang', 7); // 'boom...'
```

</details>

<br>[⬆ Back to top](#contents)

### unescapeHTML

Unescapes escaped HTML characters.

Use `String.prototype.replace()` with a regex that matches the characters that need to be unescaped, using a callback function to replace each escaped character instance with its associated unescaped character using a dictionary (object).

```js
const unescapeHTML = str =>
  str.replace(
    /&amp;|&lt;|&gt;|&#39;|&quot;/g,
    tag =>
      ({
        '&amp;': '&',
        '&lt;': '<',
        '&gt;': '>',
        '&#39;': "'",
        '&quot;': '"'
      }[tag] || tag)
  );
```

<details>
<summary>Examples</summary>

```js
unescapeHTML('&lt;a href=&quot;#&quot;&gt;Me &amp; you&lt;/a&gt;'); // '<a href="#">Me & you</a>'
```

</details>

<br>[⬆ Back to top](#contents)

### URLJoin ![advanced](/advanced.svg)

Joins all given URL segments together, then normalizes the resulting URL.

Use `String.prototype.join('/')` to combine URL segments, then a series of `String.prototype.replace()` calls with various regexps to normalize the resulting URL (remove double slashes, add proper slashes for protocol, remove slashes before parameters, combine parameters with `'&'` and normalize first parameter delimiter).

```js
const URLJoin = (...args) =>
  args
    .join('/')
    .replace(/[\/]+/g, '/')
    .replace(/^(.+):\//, '$1://')
    .replace(/^file:/, 'file:/')
    .replace(/\/(\?|&|#[^!])/g, '$1')
    .replace(/\?/g, '&')
    .replace('&', '?');
```

<details>
<summary>Examples</summary>

```js
URLJoin('http://www.google.com', 'a', '/b/cd', '?foo=123', '?bar=foo'); // 'http://www.google.com/a/b/cd?foo=123&bar=foo'
```

</details>

<br>[⬆ Back to top](#contents)

### words

Converts a given string into an array of words.

Use `String.prototype.split()` with a supplied pattern (defaults to non-alpha as a regexp) to convert to an array of strings. Use `Array.prototype.filter()` to remove any empty strings.
Omit the second argument to use the default regexp.

```js
const words = (str, pattern = /[^a-zA-Z-]+/) => str.split(pattern).filter(Boolean);
```

<details>
<summary>Examples</summary>

```js
words('I love javaScript!!'); // ["I", "love", "javaScript"]
words('python, javaScript & coffee'); // ["python", "javaScript", "coffee"]
```

</details>

<br>[⬆ Back to top](#contents)


---

## 📃 Type

### getType

Returns the native type of a value.

Returns lowercased constructor name of value, `"undefined"` or `"null"` if value is `undefined` or `null`.

```js
const getType = v =>
  v === undefined ? 'undefined' : v === null ? 'null' : v.constructor.name.toLowerCase();
```

<details>
<summary>Examples</summary>

```js
getType(new Set([1, 2, 3])); // 'set'
```

</details>

<br>[⬆ Back to top](#contents)

### is

Checks if the provided value is of the specified type.

Ensure the value is not `undefined` or `null` using `Array.prototype.includes()`, and compare the `constructor` property on the value with `type` to check if the provided value is of the specified `type`.

```js
const is = (type, val) => ![, null].includes(val) && val.constructor === type;
```

<details>
<summary>Examples</summary>

```js
is(Array, [1]); // true
is(ArrayBuffer, new ArrayBuffer()); // true
is(Map, new Map()); // true
is(RegExp, /./g); // true
is(Set, new Set()); // true
is(WeakMap, new WeakMap()); // true
is(WeakSet, new WeakSet()); // true
is(String, ''); // true
is(String, new String('')); // true
is(Number, 1); // true
is(Number, new Number(1)); // true
is(Boolean, true); // true
is(Boolean, new Boolean(true)); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isArrayLike

Checks if the provided argument is array-like (i.e. is iterable).

Check if the provided argument is not `null` and that its `Symbol.iterator` property is a function.

```js
const isArrayLike = obj => obj != null && typeof obj[Symbol.iterator] === 'function';
```

<details>
<summary>Examples</summary>

```js
isArrayLike(document.querySelectorAll('.className')); // true
isArrayLike('abc'); // true
isArrayLike(null); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isBoolean

Checks if the given argument is a native boolean element.

Use `typeof` to check if a value is classified as a boolean primitive.

```js
const isBoolean = val => typeof val === 'boolean';
```

<details>
<summary>Examples</summary>

```js
isBoolean(null); // false
isBoolean(false); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isEmpty

Returns true if the a value is an empty object, collection, has no enumerable properties or is any type that is not considered a collection.

Check if the provided value is `null` or if its `length` is equal to `0`.

```js
const isEmpty = val => val == null || !(Object.keys(val) || val).length;
```

<details>
<summary>Examples</summary>

```js
isEmpty([]); // true
isEmpty({}); // true
isEmpty(''); // true
isEmpty([1, 2]); // false
isEmpty({ a: 1, b: 2 }); // false
isEmpty('text'); // false
isEmpty(123); // true - type is not considered a collection
isEmpty(true); // true - type is not considered a collection
```

</details>

<br>[⬆ Back to top](#contents)

### isFunction

Checks if the given argument is a function.

Use `typeof` to check if a value is classified as a function primitive.

```js
const isFunction = val => typeof val === 'function';
```

<details>
<summary>Examples</summary>

```js
isFunction('x'); // false
isFunction(x => x); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isNil

Returns `true` if the specified value is `null` or `undefined`, `false` otherwise.

Use the strict equality operator to check if the value and of `val` are equal to `null` or `undefined`.

```js
const isNil = val => val === undefined || val === null;
```

<details>
<summary>Examples</summary>

```js
isNil(null); // true
isNil(undefined); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isNull

Returns `true` if the specified value is `null`, `false` otherwise.

Use the strict equality operator to check if the value and of `val` are equal to `null`.

```js
const isNull = val => val === null;
```

<details>
<summary>Examples</summary>

```js
isNull(null); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isNumber

Checks if the given argument is a number.

Use `typeof` to check if a value is classified as a number primitive. 
To safeguard against `NaN`, check if `val === val` (as `NaN` has a `typeof` equal to `number` and is the only value not equal to itself).

```js
const isNumber = val => typeof val === 'number' && val === val;
```

<details>
<summary>Examples</summary>

```js
isNumber(1); // true
isNumber('1'); // false
isNumber(NaN); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isObject

Returns a boolean determining if the passed value is an object or not.

Uses the  `Object` constructor to create an object wrapper for the given value. 
If the value is `null` or `undefined`, create and return an empty object. Οtherwise, return an object of a type that corresponds to the given value.

```js
const isObject = obj => obj === Object(obj);
```

<details>
<summary>Examples</summary>

```js
isObject([1, 2, 3, 4]); // true
isObject([]); // true
isObject(['Hello!']); // true
isObject({ a: 1 }); // true
isObject({}); // true
isObject(true); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isObjectLike

Checks if a value is object-like.

Check if the provided value is not `null` and its `typeof` is equal to `'object'`.

```js
const isObjectLike = val => val !== null && typeof val === 'object';
```

<details>
<summary>Examples</summary>

```js
isObjectLike({}); // true
isObjectLike([1, 2, 3]); // true
isObjectLike(x => x); // false
isObjectLike(null); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isPlainObject

Checks if the provided value is an object created by the Object constructor.

Check if the provided value is truthy, use `typeof` to check if it is an object and `Object.constructor` to make sure the constructor is equal to `Object`.

```js
const isPlainObject = val => !!val && typeof val === 'object' && val.constructor === Object;
```

<details>
<summary>Examples</summary>

```js
isPlainObject({ a: 1 }); // true
isPlainObject(new Map()); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isPrimitive

Returns a boolean determining if the passed value is primitive or not.

Create an object from `val` and compare it with `val` to determine if the passed value is primitive (i.e. not equal to the created object).

```js
const isPrimitive = val => Object(val) !== val;
```

<details>
<summary>Examples</summary>

```js
isPrimitive(null); // true
isPrimitive(50); // true
isPrimitive('Hello!'); // true
isPrimitive(false); // true
isPrimitive(Symbol()); // true
isPrimitive([]); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isPromiseLike

Returns `true` if an object looks like a [`Promise`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise), `false` otherwise.

Check if the object is not `null`, its `typeof` matches either `object` or `function` and if it has a `.then` property, which is also a `function`.

```js
const isPromiseLike = obj =>
  obj !== null &&
  (typeof obj === 'object' || typeof obj === 'function') &&
  typeof obj.then === 'function';
```

<details>
<summary>Examples</summary>

```js
isPromiseLike({
  then: function() {
    return '';
  }
}); // true
isPromiseLike(null); // false
isPromiseLike({}); // false
```

</details>

<br>[⬆ Back to top](#contents)

### isString

Checks if the given argument is a string. Only works for string primitives.

Use `typeof` to check if a value is classified as a string primitive.

```js
const isString = val => typeof val === 'string';
```

<details>
<summary>Examples</summary>

```js
isString('10'); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isSymbol

Checks if the given argument is a symbol.

Use `typeof` to check if a value is classified as a symbol primitive.

```js
const isSymbol = val => typeof val === 'symbol';
```

<details>
<summary>Examples</summary>

```js
isSymbol(Symbol('x')); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isUndefined

Returns `true` if the specified value is `undefined`, `false` otherwise.

Use the strict equality operator to check if the value and of `val` are equal to `undefined`.

```js
const isUndefined = val => val === undefined;
```

<details>
<summary>Examples</summary>

```js
isUndefined(undefined); // true
```

</details>

<br>[⬆ Back to top](#contents)

### isValidJSON

Checks if the provided string is a valid JSON.

Use `JSON.parse()` and a `try... catch` block to check if the provided string is a valid JSON.

```js
const isValidJSON = str => {
  try {
    JSON.parse(str);
    return true;
  } catch (e) {
    return false;
  }
};
```

<details>
<summary>Examples</summary>

```js
isValidJSON('{"name":"Adam","age":20}'); // true
isValidJSON('{"name":"Adam",age:"20"}'); // false
isValidJSON(null); // true
```

</details>

<br>[⬆ Back to top](#contents)


---

## 🔧 Utility

### castArray

Casts the provided value as an array if it's not one.

Use `Array.prototype.isArray()` to determine if `val` is an array and return it as-is or encapsulated in an array accordingly.

如果提供的值不是数组，则将其转换为数组。

使用 `array.prototype.isarray()` 来确定 `val` 是否是一个数组，如果是数组，按原样返回；如果不是数组，将值封装在数组中返回。

```js
const castArray = val => (Array.isArray(val) ? val : [val]);
```

<details>
<summary>Examples</summary>

```js
castArray('foo'); // ['foo']
castArray([1]); // [1]
```

</details>

<br>[⬆ Back to top](#contents)

### cloneRegExp

Clones a regular expression.

Use `new RegExp()`, `RegExp.source` and `RegExp.flags` to clone the given regular expression.

克隆一个正则表达式。

使用 `new RegExp()` ， `RegExp.source` 和 `RegExp.flags` 来克隆给定的正则表达式。

```js
const cloneRegExp = regExp => new RegExp(regExp.source, regExp.flags);
```

<details>
<summary>Examples</summary>

```js
const regExp = /lorem ipsum/gi;
const regExp2 = cloneRegExp(regExp); // /lorem ipsum/gi
```

</details>

<br>[⬆ Back to top](#contents)

### coalesce

Returns the first non-null/undefined argument.

Use `Array.prototype.find()` to return the first non `null`/`undefined` argument.

返回第一个不是 `null` 或 `undefined` 的参数。

使用 `Array.prototype.find()` 返回第一个不是 `null` 或 `undefined` 的参数。

```js
const coalesce = (...args) => args.find(_ => ![undefined, null].includes(_));
```

<details>
<summary>Examples</summary>

```js
coalesce(null, undefined, '', NaN, 'Waldo'); // ""
```

</details>

<br>[⬆ Back to top](#contents)

### coalesceFactory

Returns a customized coalesce function that returns the first argument that returns `true` from the provided argument validation function.

Use `Array.prototype.find()` to return the first argument that returns `true` from the provided argument validation function.

返回一个自定义的 `coalesce` 函数，该函数返回从提供的参数验证函数返回为 `true` 的第一个参数。

使用 `Array.prototype.find()` 返回从提供的参数验证函数返回 `true` 的第一个参数。
```js
const coalesceFactory = valid => (...args) => args.find(valid);
```

<details>
<summary>Examples</summary>

```js
const customCoalesce = coalesceFactory(_ => ![null, undefined, '', NaN].includes(_));
customCoalesce(undefined, null, NaN, '', 'Waldo'); // "Waldo"
```

</details>

<br>[⬆ Back to top](#contents)

### extendHex

Extends a 3-digit color code to a 6-digit color code.

Use `Array.prototype.map()`, `String.prototype.split()` and `Array.prototype.join()` to join the mapped array for converting a 3-digit RGB notated hexadecimal color-code to the 6-digit form.
`Array.prototype.slice()` is used to remove `#` from string start since it's added once.

```js
const extendHex = shortHex =>
  '#' +
  shortHex
    .slice(shortHex.startsWith('#') ? 1 : 0)
    .split('')
    .map(x => x + x)
    .join('');
```

<details>
<summary>Examples</summary>

```js
extendHex('#03f'); // '#0033ff'
extendHex('05a'); // '#0055aa'
```

</details>

<br>[⬆ Back to top](#contents)

### getURLParameters

Returns an object containing the parameters of the current URL.

Use `String.match()` with an appropriate regular expression to get all key-value pairs, `Array.prototype.reduce()` to map and combine them into a single object.
Pass `location.search` as the argument to apply to the current `url`.

```js
const getURLParameters = url =>
  (url.match(/([^?=&]+)(=([^&]*))/g) || []).reduce(
    (a, v) => ((a[v.slice(0, v.indexOf('='))] = v.slice(v.indexOf('=') + 1)), a),
    {}
  );
```

<details>
<summary>Examples</summary>

```js
getURLParameters('http://url.com/page?name=Adam&surname=Smith'); // {name: 'Adam', surname: 'Smith'}
getURLParameters('google.com'); // {}
```

</details>

<br>[⬆ Back to top](#contents)

### hexToRGB ![advanced](/advanced.svg)

Converts a color code to a `rgb()` or `rgba()` string if alpha value is provided.

Use bitwise right-shift operator and mask bits with `&` (and) operator to convert a hexadecimal color code (with or without prefixed with `#`) to a string with the RGB values. If it's 3-digit color code, first convert to 6-digit version. If an alpha value is provided alongside 6-digit hex, give `rgba()` string in return.

```js
const hexToRGB = hex => {
  let alpha = false,
    h = hex.slice(hex.startsWith('#') ? 1 : 0);
  if (h.length === 3) h = [...h].map(x => x + x).join('');
  else if (h.length === 8) alpha = true;
  h = parseInt(h, 16);
  return (
    'rgb' +
    (alpha ? 'a' : '') +
    '(' +
    (h >>> (alpha ? 24 : 16)) +
    ', ' +
    ((h & (alpha ? 0x00ff0000 : 0x00ff00)) >>> (alpha ? 16 : 8)) +
    ', ' +
    ((h & (alpha ? 0x0000ff00 : 0x0000ff)) >>> (alpha ? 8 : 0)) +
    (alpha ? `, ${h & 0x000000ff}` : '') +
    ')'
  );
};
```

<details>
<summary>Examples</summary>

```js
hexToRGB('#27ae60ff'); // 'rgba(39, 174, 96, 255)'
hexToRGB('27ae60'); // 'rgb(39, 174, 96)'
hexToRGB('#fff'); // 'rgb(255, 255, 255)'
```

</details>

<br>[⬆ Back to top](#contents)

### httpGet

Makes a `GET` request to the passed URL.

Use [`XMLHttpRequest`](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest/Using_XMLHttpRequest) web api to make a `get` request to the given `url`.
Handle the `onload` event, by calling the given `callback` the `responseText`.
Handle the `onerror` event, by running the provided `err` function.
Omit the third argument, `err`, to log errors to the console's `error` stream by default.

```js
const httpGet = (url, callback, err = console.error) => {
  const request = new XMLHttpRequest();
  request.open('GET', url, true);
  request.onload = () => callback(request.responseText);
  request.onerror = () => err(request);
  request.send();
};
```

<details>
<summary>Examples</summary>

```js
httpGet(
  'https://jsonplaceholder.typicode.com/posts/1',
  console.log
); /*
Logs: {
  "userId": 1,
  "id": 1,
  "title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
  "body": "quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto"
}
*/
```

</details>

<br>[⬆ Back to top](#contents)

### httpPost

Makes a `POST` request to the passed URL.

Use [`XMLHttpRequest`](https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest/Using_XMLHttpRequest) web api to make a `post` request to the given `url`.
Set the value of an `HTTP` request header with `setRequestHeader` method.
Handle the `onload` event, by calling the given `callback` the `responseText`.
Handle the `onerror` event, by running the provided `err` function.
Omit the third argument, `data`, to send no data to the provided `url`.
Omit the fourth argument, `err`, to log errors to the console's `error` stream by default.

```js
const httpPost = (url, data, callback, err = console.error) => {
  const request = new XMLHttpRequest();
  request.open('POST', url, true);
  request.setRequestHeader('Content-type', 'application/json; charset=utf-8');
  request.onload = () => callback(request.responseText);
  request.onerror = () => err(request);
  request.send(data);
};
```

<details>
<summary>Examples</summary>

```js
const newPost = {
  userId: 1,
  id: 1337,
  title: 'Foo',
  body: 'bar bar bar'
};
const data = JSON.stringify(newPost);
httpPost(
  'https://jsonplaceholder.typicode.com/posts',
  data,
  console.log
); /*
Logs: {
  "userId": 1,
  "id": 1337,
  "title": "Foo",
  "body": "bar bar bar"
}
*/
httpPost(
  'https://jsonplaceholder.typicode.com/posts',
  null, // does not send a body
  console.log
); /*
Logs: {
  "id": 101
}
*/
```

</details>

<br>[⬆ Back to top](#contents)

### isBrowser

Determines if the current runtime environment is a browser so that front-end modules can run on the server (Node) without throwing errors.

Use `Array.prototype.includes()` on the `typeof` values of both `window` and `document` (globals usually only available in a browser environment unless they were explicitly defined), which will return `true` if one of them is `undefined`.
`typeof` allows globals to be checked for existence without throwing a `ReferenceError`.
If both of them are not `undefined`, then the current environment is assumed to be a browser.

```js
const isBrowser = () => ![typeof window, typeof document].includes('undefined');
```

<details>
<summary>Examples</summary>

```js
isBrowser(); // true (browser)
isBrowser(); // false (Node)
```

</details>

<br>[⬆ Back to top](#contents)

### mostPerformant

Returns the index of the function in an array of functions which executed the fastest.

Use `Array.prototype.map()` to generate an array where each value is the total time taken to execute the function after `iterations` times. Use the difference in `performance.now()` values before and after to get the total time in milliseconds to a high degree of accuracy.
Use `Math.min()` to find the minimum execution time, and return the index of that shortest time which corresponds to the index of the most performant function.
Omit the second argument, `iterations`, to use a default of 10,000 iterations. The more iterations, the more reliable the result but the longer it will take.

```js
const mostPerformant = (fns, iterations = 10000) => {
  const times = fns.map(fn => {
    const before = performance.now();
    for (let i = 0; i < iterations; i++) fn();
    return performance.now() - before;
  });
  return times.indexOf(Math.min(...times));
};
```

<details>
<summary>Examples</summary>

```js
mostPerformant([
  () => {
    // Loops through the entire array before returning `false`
    [1, 2, 3, 4, 5, 6, 7, 8, 9, '10'].every(el => typeof el === 'number');
  },
  () => {
    // Only needs to reach index `1` before returning false
    [1, '2', 3, 4, 5, 6, 7, 8, 9, 10].every(el => typeof el === 'number');
  }
]); // 1
```

</details>

<br>[⬆ Back to top](#contents)

### nthArg

Creates a function that gets the argument at index `n`. If `n` is negative, the nth argument from the end is returned.

Use `Array.prototype.slice()` to get the desired argument at index `n`.

```js
const nthArg = n => (...args) => args.slice(n)[0];
```

<details>
<summary>Examples</summary>

```js
const third = nthArg(2);
third(1, 2, 3); // 3
third(1, 2); // undefined
const last = nthArg(-1);
last(1, 2, 3, 4, 5); // 5
```

</details>

<br>[⬆ Back to top](#contents)

### parseCookie

Parse an HTTP Cookie header string and return an object of all cookie name-value pairs.

Use `String.prototype.split(';')` to separate key-value pairs from each other.
Use `Array.prototype.map()` and `String.prototype.split('=')` to separate keys from values in each pair.
Use `Array.prototype.reduce()` and `decodeURIComponent()` to create an object with all key-value pairs.

```js
const parseCookie = str =>
  str
    .split(';')
    .map(v => v.split('='))
    .reduce((acc, v) => {
      acc[decodeURIComponent(v[0].trim())] = decodeURIComponent(v[1].trim());
      return acc;
    }, {});
```

<details>
<summary>Examples</summary>

```js
parseCookie('foo=bar; equation=E%3Dmc%5E2'); // { foo: 'bar', equation: 'E=mc^2' }
```

</details>

<br>[⬆ Back to top](#contents)

### prettyBytes ![advanced](/advanced.svg)

Converts a number in bytes to a human-readable string.

Use an array dictionary of units to be accessed based on the exponent.
Use `Number.toPrecision()` to truncate the number to a certain number of digits.
Return the prettified string by building it up, taking into account the supplied options and whether it is negative or not.
Omit the second argument, `precision`, to use a default precision of `3` digits.
Omit the third argument, `addSpace`, to add space between the number and unit by default.

```js
const prettyBytes = (num, precision = 3, addSpace = true) => {
  const UNITS = ['B', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB'];
  if (Math.abs(num) < 1) return num + (addSpace ? ' ' : '') + UNITS[0];
  const exponent = Math.min(Math.floor(Math.log10(num < 0 ? -num : num) / 3), UNITS.length - 1);
  const n = Number(((num < 0 ? -num : num) / 1000 ** exponent).toPrecision(precision));
  return (num < 0 ? '-' : '') + n + (addSpace ? ' ' : '') + UNITS[exponent];
};
```

<details>
<summary>Examples</summary>

```js
prettyBytes(1000); // "1 KB"
prettyBytes(-27145424323.5821, 5); // "-27.145 GB"
prettyBytes(123456789, 3, false); // "123MB"
```

</details>

<br>[⬆ Back to top](#contents)

### randomHexColorCode

Generates a random hexadecimal color code.

Use `Math.random` to generate a random 24-bit(6x4bits) hexadecimal number. Use bit shifting and then convert it to an hexadecimal String using `toString(16)`.

```js
const randomHexColorCode = () => {
  let n = (Math.random() * 0xfffff * 1000000).toString(16);
  return '#' + n.slice(0, 6);
};
```

<details>
<summary>Examples</summary>

```js
randomHexColorCode(); // "#e34155"
```

</details>

<br>[⬆ Back to top](#contents)

### RGBToHex

Converts the values of RGB components to a color code.

Convert given RGB parameters to hexadecimal string using bitwise left-shift operator (`<<`) and `toString(16)`, then `String.padStart(6,'0')` to get a 6-digit hexadecimal value.

```js
const RGBToHex = (r, g, b) => ((r << 16) + (g << 8) + b).toString(16).padStart(6, '0');
```

<details>
<summary>Examples</summary>

```js
RGBToHex(255, 165, 1); // 'ffa501'
```

</details>

<br>[⬆ Back to top](#contents)

### serializeCookie

Serialize a cookie name-value pair into a Set-Cookie header string.

Use template literals and `encodeURIComponent()` to create the appropriate string.

```js
const serializeCookie = (name, val) => `${encodeURIComponent(name)}=${encodeURIComponent(val)}`;
```

<details>
<summary>Examples</summary>

```js
serializeCookie('foo', 'bar'); // 'foo=bar'
```

</details>

<br>[⬆ Back to top](#contents)

### timeTaken

Measures the time taken by a function to execute.

Use `console.time()` and `console.timeEnd()` to measure the difference between the start and end times to determine how long the callback took to execute.

```js
const timeTaken = callback => {
  console.time('timeTaken');
  const r = callback();
  console.timeEnd('timeTaken');
  return r;
};
```

<details>
<summary>Examples</summary>

```js
timeTaken(() => Math.pow(2, 10)); // 1024, (logged): timeTaken: 0.02099609375ms
```

</details>

<br>[⬆ Back to top](#contents)

### toCurrency

Take a number and return specified currency formatting.

Use `Intl.NumberFormat` to enable country / currency sensitive formatting.

```js
const toCurrency = (n, curr, LanguageFormat = undefined) =>
  Intl.NumberFormat(LanguageFormat, { style: 'currency', currency: curr }).format(n);
```

<details>
<summary>Examples</summary>

```js
toCurrency(123456.789, 'EUR'); // €123,456.79  | currency: Euro | currencyLangFormat: Local
toCurrency(123456.789, 'USD', 'en-us'); // $123,456.79  | currency: US Dollar | currencyLangFormat: English (United States)
toCurrency(123456.789, 'USD', 'fa'); // ۱۲۳٬۴۵۶٫۷۹ ؜$ | currency: US Dollar | currencyLangFormat: Farsi
toCurrency(322342436423.2435, 'JPY'); // ¥322,342,436,423 | currency: Japanese Yen | currencyLangFormat: Local
toCurrency(322342436423.2435, 'JPY', 'fi'); // 322 342 436 423 ¥ | currency: Japanese Yen | currencyLangFormat: Finnish
```

</details>

<br>[⬆ Back to top](#contents)

### toDecimalMark

Use `toLocaleString()` to convert a float-point arithmetic to the [Decimal mark](https://en.wikipedia.org/wiki/Decimal_mark) form. It makes a comma separated string from a number.

 ```js
const toDecimalMark = num => num.toLocaleString('en-US');
```

<details>
<summary>Examples</summary>

```js
toDecimalMark(12305030388.9087); // "12,305,030,388.909"
```

</details>

<br>[⬆ Back to top](#contents)

### toOrdinalSuffix

Adds an ordinal suffix to a number.

Use the modulo operator (`%`) to find values of single and tens digits.
Find which ordinal pattern digits match.
If digit is found in teens pattern, use teens ordinal.

```js
const toOrdinalSuffix = num => {
  const int = parseInt(num),
    digits = [int % 10, int % 100],
    ordinals = ['st', 'nd', 'rd', 'th'],
    oPattern = [1, 2, 3, 4],
    tPattern = [11, 12, 13, 14, 15, 16, 17, 18, 19];
  return oPattern.includes(digits[0]) && !tPattern.includes(digits[1])
    ? int + ordinals[digits[0] - 1]
    : int + ordinals[3];
};
```

<details>
<summary>Examples</summary>

```js
toOrdinalSuffix('123'); // "123rd"
```

</details>

<br>[⬆ Back to top](#contents)

### validateNumber

Returns `true` if the given value is a number, `false` otherwise.

Use `!isNaN()` in combination with `parseFloat()` to check if the argument is a number.
Use `isFinite()` to check if the number is finite.
Use `Number()` to check if the coercion holds.

```js
const validateNumber = n => !isNaN(parseFloat(n)) && isFinite(n) && Number(n) == n;
```

<details>
<summary>Examples</summary>

```js
validateNumber('10'); // true
```

</details>

<br>[⬆ Back to top](#contents)

### yesNo

Returns `true` if the string is `y`/`yes` or `false` if the string is `n`/`no`.

Use `RegExp.test()` to check if the string evaluates to `y/yes` or `n/no`.
Omit the second argument, `def` to set the default answer as `no`.

```js
const yesNo = (val, def = false) =>
  /^(y|yes)$/i.test(val) ? true : /^(n|no)$/i.test(val) ? false : def;
```

<details>
<summary>Examples</summary>

```js
yesNo('Y'); // true
yesNo('yes'); // true
yesNo('No'); // false
yesNo('Foo', true); // true
```

</details>

<br>[⬆ Back to top](#contents)


## Collaborators

| [<img src="https://github.com/Chalarangelo.png" width="100px;"/>](https://github.com/Chalarangelo)<br/> [<sub>Angelos Chalaris</sub>](https://github.com/Chalarangelo) | [<img src="https://github.com/flxwu.png" width="100px;"/>](https://github.com/flxwu)<br/> [<sub>Felix Wu</sub>](https://github.com/Pl4gue) | [<img src="https://github.com/fejes713.png" width="100px;"/>](https://github.com/fejes713)<br/> [<sub>Stefan Feješ</sub>](https://github.com/fejes713)  | [<img src="https://github.com/kingdavidmartins.png" width="100px;"/>](https://github.com/kingdavidmartins)<br/> [<sub>King David Martins</sub>](https://github.com/iamsoorena) | [<img src="https://github.com/iamsoorena.png" width="100px;"/>](https://github.com/iamsoorena)<br/> [<sub>Soorena Soleimani</sub>](https://github.com/iamsoorena) |
| --- | --- | --- | --- | --- |
| [<img src="https://github.com/elderhsouza.png" width="100px;"/>](https://github.com/elderhsouza)<br/> [<sub>Elder Henrique Souza</sub>](https://github.com/elderhsouza) | [<img src="https://github.com/skatcat31.png" width="100px;"/>](https://github.com/skatcat31)<br/> [<sub>Robert Mennell</sub>](https://github.com/skatcat31) | [<img src="https://github.com/atomiks.png" width="100px;"/>](https://github.com/atomiks)<br/> [<sub>atomiks</sub>](https://github.com/atomiks)  |


## Credits

*Logos made by [Angelos Chalaris](https://github.com/Chalarangelo) are licensed under the [MIT](https://opensource.org/licenses/MIT) license.*
*This README is built using [markdown-builder](https://github.com/30-seconds/markdown-builder).*

