# maths-vector

[![Build Status](https://travis-ci.org/boycgit/maths-vector.svg?branch=master)](https://travis-ci.org/boycgit/maths-vector) [![Coverage Status](https://coveralls.io/repos/github/boycgit/maths-vector/badge.svg?branch=master)](https://coveralls.io/github/boycgit/maths-vector?branch=master) [![MIT Licence](https://badges.frapsoft.com/os/mit/mit.svg?v=103)](https://opensource.org/licenses/mit-license.php) [![npm version](https://badge.fury.io/js/maths-vector.svg)](https://badge.fury.io/js/maths-vector)

该仓库是因 [victor](https://github.com/maxkueng/victor/) 激发而编写的，主要是为了提供数学中的 **向量操作** 的能力。

之所以 ”重复造轮子“ 是因为 [](https://github.com/maxkueng/victor/) 实例是可变（mutable）,使用起来非常的掣肘

## features

- immutable, a Vector is not changed by its methods.([victor](https://github.com/maxkueng/victor/) is mutable，you should always call it's clone() function, so I had to create this new repo)
- include [big.js](http://mikemcl.github.io/big.js/), support for arbitrary-precision decimal arithmetic; you can always using other lib (like [bignumber.js](https://github.com/MikeMcl/bignumber.js/) and [decimal.js](https://github.com/MikeMcl/decimal.js/)) with ease by config。
- functions are chainable, you can do `new Vector(1,2).add(2).multiply(3).dot(new Vector(4, 5))` and so on;
- 

## 安装

### Node.js / Browserify

```bash
npm install vector --save
```

```javascript
var Vector = require('vector');
var vec = new Vector(42, 1337);
```

### 全局对象

Include the pre-built script.

```html
<script src="./dist/vector.umd.js"></script>
<script>
var vec = new Vector(42, 1337);
</script>
```

## Build & test

```bash
npm run build
```

```bash
npm test
```

## Document

```bash
npm run doc
```

在浏览器中打开所生成的 `out/index.html` 文件

## License

[MIT](LICENSE).