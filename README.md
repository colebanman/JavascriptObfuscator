# Javascript Obfuscator

JS Obfuscator built with Babel. Does a series of transformations to make code much harder to read or reverse-engineer. 

Feel free to make any changes as there's a lot more that can be done

## Features

The obfuscator applies the following transformations:

- variable name obfuscation
- function name obfuscation
- control flow obfuscation
- proxy functions
- dead code
- more

## Usage

To use the obfuscator, create an instance of the `JavascriptObfuscator` class and call the `obfuscate` method on it. The `obfuscate` method takes a string of Javascript code as input and returns a string of obfuscated Javascript code.

## Dependencies

This project depends on the following npm packages:

- @babel/generator
- @babel/parser
- @babel/traverse
- @babel/types

These dependencies are specified in the `package.json` file.

## Example

`const obfuscator = new JavascriptObfuscator();`

`const code = ``
const a = 5
    function test() {
        console.log(a)
    }
    test()
``;`

`const obfuscatedCode = obfuscator.obfuscate(code);`
``

Output Code:

`function _922143f6(str) {
  return eval(str);
}
var _2a9e011b = [];
_2a9e011b = 5;
const _fa5f821f = _2a9e011b;
function _proxy__5fa24c6f() {
  try {
    _e3daba8c();
  } catch (e) {}
  return _original__5fa24c6f();
}
function _original__5fa24c6f() {
  try {
    _44ecd9f1();
  } catch (e) {}
  _922143f6([[99].map(c => String.fromCharCode(c)).join(""), [111].map(c => String.fromCharCode(c)).join(""), [110].map(c => String.fromCharCode(c)).join(""), [115].map(c => String.fromCharCode(c)).join(""), [111].map(c => String.fromCharCode(c)).join(""), [108].map(c => String.fromCharCode(c)).join(""), [101].map(c => String.fromCharCode(c)).join("")].join(""))[[108, 111, 103].map(c => String.fromCharCode(c)).join("")](_fa5f821f);
}
_original__5fa24c6f();`


## License

This project is licensed under the ISC license.
