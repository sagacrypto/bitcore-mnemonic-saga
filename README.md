BIP39 Mnemonics for Dashcore
============================

[![NPM Package](https://img.shields.io/npm/v/@dashcore/dashcore-mnemonic.svg?style=flat-square)](https://www.npmjs.org/package/@dashevo/dashcore-mnemonic)
[![Build Status](https://img.shields.io/travis/dashevo/dashcore-mnemonic.svg?branch=master&style=flat-square)](https://travis-ci.org/dashevo/dashcore-mnemonic)
[![Coverage Status](https://img.shields.io/coveralls/dashevo/dashcore-mnemonic.svg?style=flat-square)](https://coveralls.io/r/dashevo/dashcore-mnemonic)

A module for [dashcore](https://github.com/dashevo/dashcore) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install dashcore-mnemonic
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://bitcore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('dashcore-mnemonic');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/dashevo/dashcore/blob/master/CONTRIBUTING.md) on the main dashcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/dashevo/dashcore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2015-2018 Dash Developers.
