# Refactoring
[Concepts of Functional Programming in Javascript](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

## What is functional programming?
Functional programming is a style of building the structure and elements of computer programs that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

**What is a pure function?**
- It returns the same result if given the same arguments (it is also referred as deterministic)
- It does not cause any observable side effects (ncluding modifying a global object or a parameter passed by reference).
- If our function reads external files, it’s not a pure function — the file’s contents can change.
- Any function that relies on a random number generator cannot be pure.


## Immutable Data
When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

**pure functions + immutable data = referential transparency**

## Functions as First-Class Entities
The idea of functions as first-class entities is that functions are also treated as values and used as data.
Functions as first-class entities can:
- refer to it from constants and variables
- pass it as a parameter to other functions
- return it as result from other functions

## Higher-order functions
When we talk about higher-order functions, we mean a function that either:
- takes one or more functions as arguments, or
- returns a function as its result

# [Strategies to Refactor JavaScript for Performance and Readability](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)
1. Return early from functions
1. Cache variables so functions can be read like sentences
1. Check for Web APIs before implementing your own functionality