# pys

> **pys** is a simple(`1 kb`) javascript library to engance String.substring / Array.slice with `python slice style`.

[![Build Status](https://travis-ci.org/hustcc/pys.svg?branch=master)](https://travis-ci.org/hustcc/pys) [![npm](https://img.shields.io/npm/v/pys.svg?style=flat-square)](https://www.npmjs.com/package/pys) [![npm](https://img.shields.io/npm/dt/pys.svg?style=flat-square)](https://www.npmjs.com/package/pys) [![npm](https://img.shields.io/npm/l/pys.svg?style=flat-square)](https://www.npmjs.com/package/pys)


# 1. Install

> npm install pys

Then import it.

```js
var pys = require('pys');

//or

import pys from 'pys';
```

Or import it with `<script>` tag.

```html
<script type="text/javascript" src="dist/pys.min.js"></script>
```


# 2. Detail Usage

There is only one API named `pys`. Below:

```js
# for array
var arr = [1, '2', 3, '4', 5, '6', 7, '8', 9, '0'];

pys(arr)('2:5');  		// [3, '4', 5]
pys(arr)(':-2');  		// [1, '2', 3, '4', 5, '6', 7, '8']
pys(arr)('-2:');  		// [9, '0']
pys(arr)('1:5:2');  	// ['2', '4']
pys(arr)('5:1:-2');  	// ['6', '4']

# for string
var str = '1234567890';
pys(str)('2:5');  		// '345'
pys(str)(':-2');  		// '12345678'
pys(str)('-2:');  		// '90'
pys(str)('1:5:2');  	// '24'
pys(str)('5:1:-2');  	// '64'

```


# 3. Test

> npm install
> 
> npm test


# 4. LICENSE

MIT