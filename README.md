[![Build Status](https://secure.travis-ci.org/huangxiangsai/bespoke-tf.png?branch=master)](https://travis-ci.org/huangxiangsai/bespoke-tf) [![Coverage Status](https://coveralls.io/repos/huangxiangsai/bespoke-tf/badge.png)](https://coveralls.io/r/huangxiangsai/bespoke-tf)

# bespoke-tf

CSS slide transitions for [Bespoke.js](http://markdalgleish.com/projects/bespoke.js)

## 说明

原bespoke-fx.js插件的改版，bespoke-fx插件基于比较老的bespoke版本开发，由于最新的bespoke上接口的调整导致在无法与新版bespoke适配。

顾重新使用官方提供的插件生成器，生成基于bespoke-fx的插件

并修改bespoke-fx已知的BUG。

*PS*: 插件依赖于`modernizr.custom.js`，使用时需引入，并且需要引入`/lib/*.css`

后期将合并打包modernizr.custom.js,使用时只需引入`/dist/bespoke-tf.min.js`。

---------

*tf*指的是transform,应为改插件主要是通过改变css样式实现幻灯片的效果。

## Download

Download the [production version][min] or the [development version][max], or use a [package manager](#package-managers).

[min]: https://raw.github.com/huangxiangsai/bespoke-tf/master/dist/bespoke-tf.min.js
[max]: https://raw.github.com/huangxiangsai/bespoke-tf/master/dist/bespoke-tf.js

## Usage

This plugin is shipped in a [UMD format](https://github.com/umdjs/umd), meaning that it is available as a CommonJS/AMD module or browser global.

For example, when using CommonJS modules:

```js
var bespoke = require('bespoke'),
  tf = require('bespoke-tf');

bespoke.from('#presentation', [
  tf()
]);
```

When using browser globals:

```js
bespoke.from('#presentation', [
  bespoke.plugins.tf()
]);
```

## Package managers

### npm

```bash
$ npm install bespoke-tf
```

### Bower

```bash
$ bower install bespoke-tf
```

## Credits

This plugin was built with [generator-bespokeplugin](https://github.com/markdalgleish/generator-bespokeplugin).

## License

[MIT License](http://en.wikipedia.org/wiki/MIT_License)
