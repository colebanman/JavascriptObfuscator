# Javascript Obfuscator

This project provides a Javascript Obfuscator, a tool that transforms Javascript code into an equivalent, harder to understand version. This is done by applying a series of transformations to the code that preserve its functionality while making it more difficult to reverse engineer.

## Features

The obfuscator applies the following transformations:

- Variable Name Obfuscation: The `obfuscateVariableNames` function renames variables to random strings, making the code harder to understand.
- Control Flow Obfuscation: The `obfuscateControlFlow` function modifies the control flow of the program, making it harder to follow.
- Function Call Hiding: The `hideFunctionCalls` function hides function calls in the code, making them harder to find and understand.
- Proxy Function Creation: The `createProxyFunctions` function creates proxy functions that replace direct calls to functions, making the code harder to understand.
- Dead Code Insertion: The `addDeadCodeBranches` function inserts dead code branches into the code, making it harder to understand and analyze.
- String and Call Obfuscation: The `obfuscateStringsAndCalls` function obfuscates strings and function calls in the code, making them harder to understand.
- Constant Variable Obfuscation: The `obfuscateConstantVariables` function obfuscates constant variables in the code, making them harder to understand.
- Object Key Obfuscation: The `obfuscateObjectKeys` function obfuscates object keys in the code, making them harder to understand.
- Eval Replacement: The `replaceEval` function replaces instances of `eval` in the code with a function call, making the code harder to understand.
- Custom Eval Function Creation: The `createEvalFunction` function creates a custom eval function that is used to replace instances of `eval` in the code.

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


## License

This project is licensed under the ISC license.
