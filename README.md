node-crc-itu [![Build Status](https://travis-ci.org/KarlosQ/node-crc-itu.png?branch=master)](https://travis-ci.org/KarlosQ/node-crc-itu)
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

// with string without encoding
var ret = crc16('0d0103588990501766460026', { toString: false });
console.log(ret.toString(16)); // 7bf9
```
