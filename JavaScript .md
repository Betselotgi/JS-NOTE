# JavaScript

# JavaScript

JavaScript is a high-level, interpreted programming language used to make web pages interactive. It is one of the most popular languages in the world, and it runs on all modern web browsers. JavaScript is mainly used for adding functionality to web pages, such as form validation, dynamic effects, and interactivity.

# Variables

In JavaScript, variables are declared using the `let` or `var` keyword

Variables defined with `let` **can not be redeclared**.

Variables defined with `let` **must be declared before use**.

Variables defined with `let` **have block scope**

Variables defined with `const` cannot be Redeclared.

Variables defined with `const` cannot be Reassigned.

Variables defined with `const` have Block Scope

**There are two limitations on variable names in JavaScript:**

1. The name must contain only letters, digits, or the symbols `$` and `_`.
2. The first character must not be a digit.

Examples of valid names:

`let userName;
let test123;`

There is a [list of reserved words](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#Keywords), which cannot be used as variable names because they are used by the language itself.

For example: `let`, `class`, `return`, and `function` are reserved.

The code below gives a syntax error:

`let let = 5; // can't name a variable "let", error!
let return = 5; // also can't name it "return", error!`

**An assignment without `use strict`**

Normally, we need to define a variable before using it. But in the old times, it was technically possible to create a variable by a mere assignment of the value without using `let`. This still works now if we don’t put `use strict` in our scripts to maintain compatibility with old scripts.

`// note: no "use strict" in this example

num = 5; // the variable "num" is created if it didn't exist

alert(num); // 5`

This is a bad practice and would cause an error in strict mode:

`"use strict";

*num = 5; // error: num is not defined*`

# Operators

Operators are used to perform operations on values, such as arithmetic operations (`+`, `-`, `*`, `/`) and comparison operations (`==`, `!=`, `>`, `<`, `>=`, `<=`). JavaScript also supports logical operators (`&&`, `||`, `!`) and bitwise operators (`&`, `|`, `^`, `~`, `<<`, `>>`, `>>>`).

# **Data types**

A value in JavaScript is always of a certain type. For example, a string or a number.

There are eight basic data types in JavaScript

We can put any type in a variable. For example, a variable can at one moment be a string and then store a number:

`// no error
let message = "hello";
message = 123456;`

Programming languages that allow such things, such as JavaScript, are called “dynamically typed”, meaning that there exist data types, but variables are not bound to any of them

**There are 8 basic data types in JavaScript.**

- Seven primitive data types:
    - `number` for numbers of any kind: integer or floating-point, integers are limited by `±(2531)`.
    - `bigint` for integer numbers of arbitrary length.
    - `string` for strings. A string may have zero or more characters, there’s no separate single-character type.
    - `boolean` for `true`/`false`.
    - `null` for unknown values – a standalone type that has a single value `null`.
    - `undefined` for unassigned values – a standalone type that has a single value `undefined`.
    - `symbol` for unique identifiers.
- And one non-primitive data type:
    - `object` for more complex data structures.

**The Object Datatype**

The object data type can contain:

1. An object

2. An array

3. A date

# Control  statements

JavaScript has several control statements, including `if/else`, `switch`, `for`, `while`, and `do/while`. These statements control the flow of a program by allowing certain sections of code to be executed conditionally or repeatedly. The `if/else` statement is used to execute code based on a condition, while the `switch` statement is used to select one of several code blocks to be executed. The `for` statement is used to loop through a block of code a specified number of times, while the `while` and `do/while` statements are used to loop through a block of code while a specified condition is true.

# Functions

Functions in JavaScript are blocks of code that can be defined once and executed many times. They are used to perform a specific task and can take in arguments and return values. Functions are defined using the `function` keyword, followed by a name, a list of parameters in parentheses, and the code to be executed in curly braces. They can be called by their name followed by parentheses containing any arguments. Functions are an important part of JavaScript, and they allow for code reusability and modularity.

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

A JavaScript function is defined with the `function` keyword, followed by a **name**, followed by parentheses **()**.

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:

**(*parameter1, parameter2, ...*)**

The code to be executed, by the function, is placed inside curly brackets: **{}**

# Function Invocation

The code inside the function will execute when "something" **invokes** (calls) the function:

- When an event occurs (when a user clicks a button)
- When it is invoked (called) from JavaScript code
- Automatically (self invoked)

# Function Return

When JavaScript reaches a `return` statement, the function will stop executing.

If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

Functions often compute a **return value**. The return value is "returned" back to the "caller":

**Example**

**function showMessage() {
  alert( 'Hello everyone!' );
}**

***showMessage();***

**JavaScript objects**

JavaScript objects are containers for named values called properties and methods. They can be created using the object literal syntax (`{}`) or the `new Object()` constructor. Properties are name-value pairs, and methods are functions that are associated with an object. Objects can also be used to create complex data structures, such as arrays and maps. In JavaScript, almost everything is an object, including strings, numbers, and functions themselves. Objects are a fundamental concept in JavaScript, and understanding them is essential for developing complex applications.