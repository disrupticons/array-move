# array-move [![Build Status](https://travis-ci.org/sindresorhus/array-move.svg?branch=master)](https://travis-ci.org/sindresorhus/array-move)

> Move an array item to a different position


## Install

```
$ npm install --save array-move
```


## Usage

```js
var arrayMove = require('array-move');

arrayMove(['a', 'b', 'c'], 1, 2);
//=> ['a', 'c', 'b']

arrayMove(['a', 'b', 'c'], -1, 0);
//=> ['c', 'a', 'b']
```


## API

### arrayMove(input, from, to)

Returns a new array with the item moved to the new position.

### arrayMove.mut(input, from, to)

Moves the item to the new position in the input array.  
Useful for huge arrays where absolute performance is needed.

#### input

Type: `array`

#### from

Type: `number`

Index of item to move.  
If negative, it will begin that many elements from the end.

#### to

Type: `number`

Index of where to move the item.


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)
