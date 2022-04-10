# utils-number

[![npm version](https://img.shields.io/npm/v/axios.svg?style=flat-square)](https://fozan.gitbook.io/fozan-inc/)

Utilities for working with numbers on Node.js.

> All products of ФОЗАН inc. on the site: [click here](https://fozan.gitbook.io/fozan-inc/)

## Table of Contents

  - [Features](#features)
  - [Installing](#installing)
  - [Example](#example)
  - [Resources](#resources)
  - [License](#license)

## Features

- Make numbers readable.
- Get a random number in the selected range.
- Receive a random message from your list.
- Get the exact date and time.
- Use emoticons for success and failure.
- Converting time to milliseconds.
- Calculate interest gain.
- Place spaces after each letter in text.

## Installing

Using npm:

```bash
$ npm install utils-number
```

## Example

To connect the library utils-number, enter the following text:

```js
const utils = require('utils-number');
```

Executing `sp`&`rn` request

```js
const utils = require('utils-number');

var number = 1000; //Choose a number

console.log(utils.sp(number, "."));
console.log(utils.rn(number));
```

Executing a `random`&`pick` request

```js
const utils = require('utils-number');

var number = utils.random(1, 1000); //Set the number generation range
var word = utils.pick(['Apple', 'Node.JS', 'Table']); //We make a list of phrases.

console.log(number);
console.log(word);
```

> **NOTE.** Specifying a range is optional, you can simply enter the maximum number in the argument.

Executing a `data`&`time` request

```js
const utils = require('utils-number');

var data = utils.data(); //Date display
var time = utils.time(); //Time display

console.log(data);
console.log(time);
```

Executing a `smile` request

```js
const utils = require('utils-number');

var success = utils.smile('sucs'); //Display success emoticon
var failure = utils.smile('fail'); //Show failure emoticon

console.log(success);
console.log(failure);
```

Executing a `inmls` request

```js
const utils = require('utils-number');

var number = 100; //Choose a number

var sec = utils.inmls(number, 's'); //seconds
var min = utils.inmls(number, 'm'); //minute
var hour = utils.inmls(number, 'h'); //hours
var day = utils.inmls(number, 'd'); //days

console.log(day, hour, min, sec);
```

> **NOTE.** `d` - day; `h` - hour; `m` - minute; `s` - secunde.

Executing a `growth` request

```js
const utils = require('utils-number');

var number1 = Number(x);
var number2 = Number(y);

var res = utils.growth(number1, number2);

console.log(res);
```

> **NOTE.** `x` - outgoing value; `y` - final value.

Executing a `spacetext` request

```js
const utils = require("utils-number");

var text = `Test`;

var res = utils.spacetext(text);

console.log(res);
```

## Resources

* [website](https://fozan.gitbook.io/fozan-inc/)
* [npm](https://www.npmjs.com/package/utils-number)

## License

[MIT](LICENSE)
