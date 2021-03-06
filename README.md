# solidity-to-abi

<div>
  <!-- Dependency Status -->
  <a href="https://david-dm.org/SilentCicero/solidity-to-abi">
    <img src="https://david-dm.org/SilentCicero/solidity-to-abi.svg" alt="Dependency Status" />
  </a>

  <!-- devDependency Status -->
  <a href="https://david-dm.org/SilentCicero/solidity-to-abi#info=devDependencies">
    <img src="https://david-dm.org/SilentCicero/solidity-to-abi/status.svg" alt="devDependency Status" />
  </a>

  <!-- Build Status -->
  <a href="https://travis-ci.org/SilentCicero/solidity-to-abi">
    <img src="https://travis-ci.org/SilentCicero/solidity-to-abi.svg" alt="Build Status" />
  </a>

  <!-- Test Coverage
  <a href="https://coveralls.io/r/SilentCicero/solidity-to-abi">
    <img src="https://coveralls.io/repos/github/SilentCicero/solidity-to-abi/badge.svg" alt="Test Coverage" />
  </a>
   -->

  <!-- NPM Version -->
  <a href="https://www.npmjs.org/package/solidity-to-abi">
    <img src="http://img.shields.io/npm/v/solidity-to-abi.svg" alt="NPM version" />
  </a>

  <!-- Javascript Style -->
  <a href="http://airbnb.io/javascript/">
    <img src="https://img.shields.io/badge/code%20style-airbnb-brightgreen.svg" alt="js-airbnb-style" />
  </a>
</div>

<br />

A simple module that converts an Ethereum Solidity smart-contract method interface string into a web3 standard ABI object.

## Install

```
npm install --save-dev solidity-to-abi
```

## Usage

```js
import solidityToABI from `solidity-to-abi`;

// parse solidity method string
const abi = solidityToABI('balanceOf(address _addr):(uint256 balance)');

console.log(abi);
/*
Object result:
{
  "name": "balanceOf",
  "type": "function",
  "constant": false,
  "inputs": [
    {
      "type": "address",
      "name": "_addr"
    }
  ],
  "outputs": [
    {
      "type": "uint256",
      "name": "balance"
    }
  ]
}
*/
```

## Contributing

Please help better the ecosystem by submitting issues and pull requests to default. We need all the help we can get to build the absolute best linting standards and utilities. We follow the AirBNB linting standard. Please read more about contributing to `solidity-to-abi` in the `CONTRIBUTING.md`.

## Guides

You'll find more detailed information on using default and tailoring it to your needs in our guides:

- [User guide](docs/user-guide.md) - Usage, configuration, FAQ and complementary tools.
- [Developer guide](docs/developer-guide.md) - Contributing to solidity-to-abi and writing your own plugins & formatters.

## Help out

There is always a lot of work to do, and will have many rules to maintain. So please help out in any way that you can:

- Create, enhance, and debug rules (see our guide to ["Working on rules"](CONTRIBUTING.md)).
- Improve documentation.
- Chime in on any open issue or pull request.
- Open new issues about your ideas for making stylelint better, and pull requests to show us how your idea works.
- Add new tests to *absolutely anything*.

Please consult our [Code of Conduct](CODE_OF_CONDUCT.md) and [Contributing](.github/CONTRIBUTING.md) docs before helping out.

We communicate via [issues](https://github.com/SilentCicero/solidity-to-abi/issues) and [pull requests](https://github.com/SilentCicero/solidity-to-abi/pulls).

## Important documents

- [Changelog](CHANGELOG.md)
- [Contributing Guidelines](.github/CONTRIBUTING.md)
- [Code of Conduct](CODE_OF_CONDUCT.md)
- [License](https://raw.githubusercontent.com/SilentCicero/solidity-to-abi/master/LICENSE)

## Licence

This project is licensed under the MIT license, Copyright (c) 2016 Nick Dodson. For more information see LICENSE.md.

```
The MIT License

Copyright (c) 2016 Nick Dodson. nickdodson.com

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
