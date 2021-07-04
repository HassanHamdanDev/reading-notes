
# Operators and Loops

## 1. Operators

JavaScript has the following types of operators. This section describes the operators and contains information about operator precedence.

```
For example, 3+4 or x*y.

For example, x++ or ++x.
```
An assignment operator assigns a value to its left operand based on the value of its right operand.

*Like most expressions, assignments like x = y have a return value. It can be retrieved by e.g. assigning the expression or logging it:*
```
const z = ; // Or equivalently: const z = x = y;
console.log; // Log the return value of the assignment x = y.
console.log; // Or log the return value directly.
```
*The return value matches the expression to the right of the = sign in the «Meaning» column of the table above. That means that returns y, returns the resulting sum x + y, returns the resulting power x ** y, and so on.*


* Destructuring

For more complex assignments, the destructuring assignment syntax is a JavaScript expression that makes it possible to extract data from arrays or objects using a syntax that mirrors the construction of array and object literals.

*A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. Strings are compared based on standard lexicographical ordering, using Unicode values. In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison. This behavior generally results in comparing the operands numerically*.


* OperatorUsageDescription

Logical AND expr1 && expr2Returns expr1 if it can be converted to false; otherwise, returns expr2. Thus, when used with Boolean values, && returns true if both operands are true; otherwise, returns false.
Logical OR expr1 || expr2Returns expr1 if it can be converted to true; otherwise, returns expr2.

* Short-circuit evaluation

As logical expressions are evaluated left to right, they are tested for possible «short-circuit» evaluation using the following rules: false && anything is short-circuit evaluated to false.
true || anything is short-circuit evaluated to true.
The rules of logic guarantee that these evaluations are always correct. Note that the anything part of the above expressions is not evaluated, so any side effects of doing so do not take effect.
```

The conditional operator is the only JavaScript operator that takes three operands. The operator can have one of two values based on a condition.

This statement assigns the value «adult» to the variable status if age is eighteen or more. Otherwise, it assigns the value «minor» to status.
The comma operator evaluates both of its operands and returns the value of the last operand. This operator is primarily used inside a for loop, to allow multiple variables to be updated each time through the loop.
```
* **Expressions**

An expression is any valid unit of code that resolves to a value.
Every syntactically valid expression resolves to some value but conceptually, there are two types of expressions: with side effects and those that in some sense evaluate and therefore resolve to a value.
The expression x = 7 is an example of the first type.

JavaScript has the following expression categories

Arithmetic: evaluates to a number, for example 3.14159.
String: evaluates to a character string, for example, «Fred» or «234».
Logical: evaluates to true or false.

```
Use the this keyword to refer to the current object. In general, this refers to the calling object in a method.

The grouping operator controls the precedence of evaluation in expressions.

Left values are the destination of an assignment.


The super keyword is used to call functions on an object's parent.
```

## 2. Loops and iteration


*Loops offer a quick and easy way to do something repeatedly. This chapter of the JavaScript Guide introduces the different iteration statements available to JavaScript.*

*You can think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another*.

A for loop repeats until a specified condition evaluates to false.


*The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.*

*The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. If the value of condition is false, the for loop terminates.
The statement executes.*

*The do...while statement repeats until a specified condition evaluates to false.*

*A do...while statement looks as follows: do while ;
statement is always executed once before the condition is checked.
If condition is true, the statement executes again.*

*If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.
The condition test occurs before statement in the loop is executed.*

```
The value of label may be any JavaScript identifier that is not a reserved word.

Use the break statement to terminate a loop, switch, or in conjunction with a labeled statement.


The first form of the syntax terminates the innermost enclosing loop or switch.

```
*The continue statement can be used to restart a while, do-while, for, or label statement.*

*When you use continue without a label, it terminates the current iteration of the innermost enclosing while, do-while, or for statement and continues execution of the loop with the next iteration.*
```
A statement labeled checkiandj contains a statement labeled checkj. If continue is encountered, the program terminates the current iteration of checkj and begins the next iteration. Each time continue is encountered, checkj reiterates until its condition returns false.

The for...in statement iterates a specified variable over all the enumerable properties of an object. For each distinct property, JavaScript executes the specified statements.
```

* Arrays

Although it may be tempting to use this as a way to iterate over Array elements, the for...in statement will return the name of your user-defined properties in addition to the numeric indexes.

**Useful Links :**

>1. [Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
>2. [Loops and iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)
