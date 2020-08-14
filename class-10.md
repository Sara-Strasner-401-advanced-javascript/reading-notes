# Debugging
Debugging is the process of finding errors. It involves a process of deduction. If you understand execution contexts (which have two stages) and stacks, you are more likely to find the error in your code. A great resource in debugging is the console. The console helps narrow down the area in which the error is located, so you can try to find the exact error. 

Every statement in a script lives in one of three execution contexts:
- global context: code that is in the script, but not in a function. There is only one global context in any page.
- function context: code that is being run within a function.
- eval context (not shown): text is executed like code in an internal function called `eval()` (which is not covered in the Duckett book).

The same scopes apply to variables, which are either global or have a function-level scope. 

JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error. 

If you know that you may get an error, you can use the `try`, `catch`, and `finally` statements. Use them to give your users helpful feedback. 
- The `try...catch` statement marks a block of statements to try and specifies a response should an exception be thrown.
- `finally` statements are executed after the try statement completes. These statements execute regardless of whether an exception was thrown or caught.

## A Debugging Workflow
### Where is the problem?
Narrow down the area where the problem seems to be. 
1. Look at the error message. It tells you the relevant script, line number, and type of error. 
1.  Check how far the script is running. Use tools to write messages to the console to tell how far your script has executed.
1. Use breakpoints where things are going wrong. They let you pause execution and inspect the values that are stored in variables.

## What exactly is the problem? 
One you know the area in which the problem is located, you can then try to find the actual line of code that is causing the error.
1. When you have set breakpoints, you can see if the variables around them have the values you would expect them to. If not, look earlier in the script.
1. Break down/break out parts of the code to test smaller pieces of the functionality.
1. Check the number of parameters for a function, or the number of items in an array. 