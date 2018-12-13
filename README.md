node-crc-itu [![npm version](https://badge.fury.io/js/node-crc-itu.svg)](https://badge.fury.io/js/node-crc-itu) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://reactnavigation.org/docs/contributing.html)
=======

Install:

Using yarn
```
yarn add node-crc-itu 
```

Or

Using npm
```
npm install --save node-crc-itu 
```

Usage:

```
var crc16 = require('node-crc-itu');

// with string
var ret = crc16('0d0103588990501766460026');
console.log(ret); // 7bf9

// with buffer
var buff = Buffer.from('0d0103588990501766460026', 'hex');
var ret = crc16(buff);
console.log(ret); // 7bf9

// with string without encoding output
var ret = crc16('0d0103588990501766460026', { toString: false });
console.log(ret.toString(16)); // 7bf9
```
