# FUNCTIONAL PROGRAMMING


## Functional Programming Concepts


1. What is functional programming?

```

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

```


2. What is a pure function and how do we know if something is a pure function?

```

Pure functions are stable, consistent, and predictable. Given the same parameters, pure functions will always return the same result. We don’t need to think of situations when the same parameter has different results — because it will never happen.

- It returns the same result if given the same arguments (it is also referred as deterministic)
- It does not cause any observable side effects

```


3. What are the benefits of a pure function?

```

The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:
Given a parameter A → expect the function to return value B
Given a parameter C → expect the function to return value D

```


4. What is immutability?

```

Unchanging over time or unable to be changed.

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

We can handle this mutation by doing function composition, or function chaining. In other words, the result of a function will be used as an input for the next function, without modifying the original input string.

```


5. What is Referential transparency?

```

Basically, if a function consistently yields the same result for the same input, it is referentially transparent.
pure functions + immutable data = referential transparency

```



## Node JS Tutorial for Beginners #6 - Modules and require()


What is a module?

```

Module in Node. js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node.  Each module in Node. js has its own context, so it cannot interfere with other modules or pollute global scope. Also, each module can be placed in a separate 

```


What does the word ‘require’ do?

```

require() is used to consume modules. It allows you to include modules in your app. You can add built-in core Node. js modules, community-based modules (node_modules), and local modules too 

```


How do we bring another module into the file the we are working in?

```

To import Node JS module. var module = require("./module");

```


What do we have to do to make a module available?

```
module.exports = module;


```

## Things I want to know more about

```

Referential transparency

```

