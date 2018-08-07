BIP39 Mnemonics for Bitcore-Saga
============================

[![NPM Package](https://img.shields.io/npm/v/@sagacrypto/bitcore-mnemonic-saga.svg?style=flat-square)](https://www.npmjs.org/package/@sagacrypto/bitcore-mnemonic-saga)
[![Build Status](https://img.shields.io/travis/sagacrypto/bitcore-mnemonic-saga.svg?branch=master&style=flat-square)](https://travis-ci.org/sagacrypto/bitcore-mnemonic-saga)
[![Coverage Status](https://img.shields.io/coveralls/sagacrypto/bitcore-mnemonic-saga.svg?style=flat-square)](https://coveralls.io/r/sagacrypto/bitcore-mnemonic-saga)

A module for [bitcore-saga](https://github.com/sagacrypto/bitcore-saga) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install bitcore-mnemonic-saga
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://bitcore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('bitcore-mnemonic-saga');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/sagacrypto/bitcore-saga/blob/master/CONTRIBUTING.md) on the main dashcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/sagacrypto/bitcore-saga/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2015-2018 Dash Developers.
Copyright 2018 Saga Development Team.
