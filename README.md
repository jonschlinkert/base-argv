# base-argv [![NPM version](https://img.shields.io/npm/v/base-argv.svg?style=flat)](https://www.npmjs.com/package/base-argv) [![NPM downloads](https://img.shields.io/npm/dm/base-argv.svg?style=flat)](https://npmjs.org/package/base-argv) [![Build Status](https://img.shields.io/travis/node-base/base-argv.svg?style=flat)](https://travis-ci.org/node-base/base-argv)

> Plugin that post-processes the argv object from simplify how args are mapped to options, tasks and generators.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install base-argv --save
```

## Usage

```js
var Base = require('base-methods');
var argv = require('base-argv');

var app = new Base();
app.use(argv());

// parse argv
var args = app.argv(['foo', 'bar', '--set=a:b']);
console.log(args);
```

Results in:

```js
{ set: { a: 'b' }, tasks: [ 'foo', 'bar' ] }
```

This object can then be passed to something else for further processing.

## Related projects

You might also be interested in these projects:

* [base-cli](https://www.npmjs.com/package/base-cli): Plugin for base-methods that maps built-in methods to CLI args (also supports methods from a… [more](https://www.npmjs.com/package/base-cli) | [homepage](https://github.com/node-base/base-cli)
* [base-config](https://www.npmjs.com/package/base-config): base-methods plugin that adds a `config` method for mapping declarative configuration values to other 'base'… [more](https://www.npmjs.com/package/base-config) | [homepage](https://github.com/node-base/base-config)
* [base-methods](https://www.npmjs.com/package/base-methods): base-methods is the foundation for creating modular, unit testable and highly pluggable node.js applications, starting… [more](https://www.npmjs.com/package/base-methods) | [homepage](https://github.com/jonschlinkert/base-methods)
* [base-options](https://www.npmjs.com/package/base-options): Adds a few options methods to base-methods, like `option`, `enable` and `disable`. See the readme… [more](https://www.npmjs.com/package/base-options) | [homepage](https://github.com/jonschlinkert/base-options)
* [base-plugins](https://www.npmjs.com/package/base-plugins): Upgrade's plugin support in base applications to allow plugins to be called any time after… [more](https://www.npmjs.com/package/base-plugins) | [homepage](https://github.com/node-base/base-plugins)

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/jonschlinkert/base-argv/issues/new).

## Building docs

Generate readme and API documentation with [verb](https://github.com/verbose/verb):

```sh
$ npm install verb && npm run docs
```

Or, if [verb](https://github.com/verbose/verb) is installed globally:

```sh
$ verb
```

## Running tests

Install dev dependencies:

```sh
$ npm install -d && npm test
```

## Author

**Jon Schlinkert**

* [github/jonschlinkert](https://github.com/jonschlinkert)
* [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright © 2016, [Jon Schlinkert](https://github.com/jonschlinkert).
Released under the [MIT license](https://github.com/node-base/base-argv/blob/master/LICENSE).

***

_This file was generated by [verb](https://github.com/verbose/verb), v0.9.0, on April 14, 2016._