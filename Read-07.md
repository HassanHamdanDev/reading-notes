# Programming with JavaScript



## Function 

The name of the function.
A list of parameters to the function, enclosed in parentheses and separated by commas.


The function square takes one parameter, called number. The function consists of one statement that says to return the parameter of the function multiplied by itself. The statement return specifies the value returned by the function:


While the function declaration above is syntactically a statement, functions can also be created by a function expression.


Function expressions are convenient when passing a function as an argument to another function. The following example shows a map function that should receive a function as first argument and an array as second argument.

```
Function returns: [0, 1, 8, 125, 1000].


myFunc = function {
```
In addition to defining functions as described here, you can also use the Function constructor to create functions from a string at runtime, much like eval.


* Calling functions

Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.
Calling the function actually performs the specified actions with the indicated parameters.
The preceding statement calls the function with an argument of 5. The function executes its statements and returns the value 25.
Functions must be in scope when they are called, but the function declaration can be hoisted , as in this example:
```
 console.logsquare; /* ... */ function square { return n * n }

```
The arguments of a function are not limited to strings and numbers. You can pass whole objects to a function.

There are other ways to call functions. There are often cases where a function needs to be called dynamically, or the number of arguments to a function vary, or in which the context of the function call needs to be set to a specific object determined at runtime.


* Function scope

Variables defined inside a function cannot be accessed from anywhere outside the function, because the variable is defined only in the scope of the function. However, a function can access all variables and functions defined inside the scope in which it is defined.
In other words, a function defined in the global scope can access all variables defined in the global scope.

A function that calls itself is called a recursive function. In some ways, recursion is analogous to a loop. Both execute the same code multiple times, and both require a condition .

Compared to the function loop, each recursive call itself makes many recursive calls here.
It is possible to convert any recursive algorithm to a non-recursive one, but the logic is often much more complex, and doing so requires the use of a stack.


* Nested functions and closures

You may nest a function within another function. The nested function is private to its containing function.
It also forms a closure. A closure is an expression that can have free variables together with an environment that binds those variables .


### To summarize

The inner function can be accessed only from statements in the outer function.


Notice how x is preserved when inside is returned. A closure must preserve the arguments and variables in all scopes it references. Since each call provides potentially different arguments, a new closure is created for each call to outside.

Multiply-nested functions

A function contains a function , which itself contains a function .
Both functions B and C form closures here. So, B can access A, and C can access B.

```
In this example, C accesses B's y and A's x.

This can be done because

B forms a closure including A .
C forms a closure including B.
Because B's closure includes A, C's closure includes A, C can access both B and A's arguments and variables. In other words, C chains the scopes of B and A, in that order.

```
* Name conflicts

When two arguments or variables in the scopes of a closure have the same name, there is a name conflict. More nested scopes take precedence. So, the inner-most scope takes the highest precedence, while the outer-most scope takes the lowest.

The name conflict happens at the statement return x * 2 and is between inside's parameter x and outside's variable x.

* Closures

Closures are one of the most powerful features of JavaScript. JavaScript allows for the nesting of functions and grants the inner function full access to all the variables and functions defined inside the outer function .
However, the outer function does not have access to the variables and functions defined inside the inner function. This provides a sort of encapsulation for the variables of the inner function.

```

myPet; // Returns «Vivie»

It can be much more complex than the code above.

pet.getName; // Vivie pet.setName;
pet.
pet.getSex; // male pet.getName; // Oliver


getCode; // Returns the apiCode
```
If an enclosed function defines a variable with the same name as a variable in the outer scope, then there is no way to refer to the variable in the outer scope again.


* Using the arguments object

where i is the ordinal number of the argument, starting at 0. So, the first argument passed to a function would be arguments[0]. The total number of arguments is indicated by arguments.length.
Using the arguments object, you can call a function with more arguments than it is formally declared to accept. This is often useful if you don't know in advance how many arguments will be passed to the function.

Note: The arguments variable is «array-like», but not an array. It is array-like in that it has a numbered index and a length property.

* Default parameters

In JavaScript, parameters of functions default to undefined.

Without default parameters

In the past, the general strategy for setting defaults was to test parameter values in the body of the function and assign a value if they are undefined.


With default parameters

For more details, see default parameters in the reference.

Rest parameters

The rest parameter syntax allows us to represent an indefinite number of arguments as an array.


## Control flow


The control flow is the order in which the computer executes statements in a script.

Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops. 

For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else, so that different code executes depending on whether the form is complete or not:
```
if (field==empty) {
    promptUser();
} else {
    submitForm();
}
```
A typical script in JavaScript or PHP (and the like) includes many control structures, including conditionals, loops and functions. Parts of a script may also be set to execute when events occur.

## JavaScript Functions

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

Example
```
function myFunction(p1, p2) {
  return p1 * p2;   // The function returns the product of p1 and p2
}
```
JavaScript Function Syntax
A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)

The code to be executed, by the function, is placed inside curly brackets: {}
```
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```
Function parameters are listed inside the parentheses () in the function definition.

Function arguments are the values received by the function when it is invoked.

Inside the function, the arguments (the parameters) behave as local variables.

A Function is much the same as a Procedure or a Subroutine, in other programming languages.

Function Invocation
The code inside the function will execute when "something" invokes (calls) the function:

When an event occurs (when a user clicks a button)
When it is invoked (called) from JavaScript code
Automatically (self invoked)
You will learn a lot more about function invocation later in this tutorial.

## JavaScript Operators

* Example
Assign values to variables and add them together:
```
let x = 5;         // assign the value 5 to x
let y = 2;         // assign the value 2 to y
let z = x + y;     // assign the value 7 to z (5 + 2)
```
The assignment operator (=) assigns a value to a variable.

* Assignment
```
let x = 10;
```
The addition operator (+) adds numbers:

* Adding
```
let x = 5;
let y = 2;
let z = x + y;
```
The multiplication operator (*) multiplies numbers.

* Multiplying
```
let x = 5;
let y = 2;
let z = x * y;
```