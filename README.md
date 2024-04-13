### ES5 Global Constants
```
var PI = 3.14;
PI = 42; // stop me from doing this!
```
-----
### ES2015 Global Constants
```
/* Write an ES2015 Version */
let PI = 3.14;
PI = 42;
///Uncaught SyntaxError: Identifier 'PI' has already been declared
```
-----

# Quiz
## What is the difference between var and let?
    var allows you to redeclare, while let prevents this. var is used within a function scope and let is relative to the block.

## What is the difference between var and const?
    var can be reassigned and redeclared while const cannot. var is used in a function scope while const is relative to the block scope.

## What is the difference between let and const?
    let can be reassigned to a new variable while const cannot.

## What is hoisting?
    Hoisting is a process in javascript in which both functions and variables are put to the top of the corresponding scope during compilation.
    This happens usually if you reference a variable in a function before it is declared - and the variable is declared before the function calls that specific variable.
    One important note is that the variable is only declared but not initialized, meaning that the code accessing it before initialization will be working with an undefined.
    Hoisted functions can be called before definition but function expressions (setting a function to a a variable expression) are not, resulting in an error.