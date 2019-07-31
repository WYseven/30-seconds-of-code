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
