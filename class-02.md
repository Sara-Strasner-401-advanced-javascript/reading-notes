# CSS

CSS properties affect how elements are displayed. CSS associates style rules with HTML elements. A CSS rule contains two parts: a selector and a declaration.
 - **Selectors** indicate which element the rule applies to. The same rule can apply to more than one element if you separate the names with commas. 
 - **Declarations** indicate how the element referred to in the selector should be styled. Declarations are split into two parts (a property and a value) and are separated by a colon. 

![CSS Diagram](https://upload.wikimedia.org/wikipedia/commons/5/53/CSSsyntax.JPG)

### How CSS Rules Cascade
If there are two or more rules that apply to the same element, it is important to understand which will take precedence. 
- If two selectors are identical, the latter of the two will take precedence. 
- If one selector is more specific than the others, the more specific rule will take precedence over more general ones. 
- You can add `!important` after any property value to indicate that it should be considered more important than the other rules that apply to the same element. 

### Why use external style sheets?
CSS rules usually appear in a separate document, although they may appear within an HTML page. By putting your CSS rules in a separate style sheet, all of your web pages can share the same style sheet. If you are just creating a single page, you might decide to put the rules in the same file to keep everything in one place. However, many authors would consider it better practice to keep the CSS in a separate file. 

For commonly used CSS selectors, see [MDN CSS Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors).


## Color
Color not only brings your site to life, but also helps convey the mood and evokes reaction. There are three ways to specify color in CSS: RBG values, hex codes, and color names. 

Color pickers can help you find the color you want. [Adobe Color](https://color.adobe.com/create/color-wheel) is a great resource. 

It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content). 

CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as *RGBA.* CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA. 

# Programming with JavaScript

### Scripts
A **script** is a series of step-by-step instructions that a computer can follow to achieve a goal. Each time a script runs, it might only use a subset of all the instructions. To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help). 


## Expressions and Operators
An expression evaluates into (results in) a single value. There are two types of expressions.
1. Expressions that just assign a value to a variable. In order for a variable to be useful, it needs to be given a value. This is done using the assignment operator (the equals sign):
```var color - `beige`;```
The value of color is now beige. This expression is an example of an assignment operator.

1. Expressions that use two or more values to return a single value. 
You can perform operations on any number of individual values to determine a single value:
```var area = 3 * 2;```
The value of area is now 6. This expression is an example of an arithmetic operator. 

Expressions rely on things called operators, which allow programmers to create a single value from one or more values. 

#### Arithmetic Operators #### 
- Addition +
- Subtraction -
- Division /
- Multiplication *
- Increment ++ (adds 1 to the current number)
- Decrement -- (subtracts 1 from the current number)
- Modulus % (divides two values and returns the remainder)
Don’t forget order of operations! 

#### String Operators #### 
There is just one string operator, the plus symbol. It is used to join the strings on either side of it. 
Keep in mind:
- When you place quotes around a number, it is a string (not a numeric data type). 
- If you try to add a numeric data type to a string, then the number becomes part of the string. 
- If you try to use any of the other arithmetic operators on a string, then the value that results is usually a value called NaN (Not a Number). 

## Functions
Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements). 

To create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces. This is known as a function declaration. 

## Parameters
Sometimes a function needs specific information to perform its task. In such cases, when you declare the function you give it **parameters.** Inside the function, the parameters act like variables. 

# Operators

## Comparison Operators: Evaluating Conditions
You can evaluate a situation by comparing one value in the script to what you expect it might be. The result will be a Boolean: true or false. 

Common Comparison Operators
- `==` equal to
- `===` strictly equal to
- `!=` not equal to
- `!==` strictly not equal to
- `>` greater than
- `<` less than
- `>=` greater than or equal to
- `<=` less than or equal to


## Logical Operators
Comparison operators usually return a single value of true or false. Logical operators allow you to compare the results of two or more comparison operators. 

Commong Logical Operators
- `&&` **Logical And.** checks to see whether both expressions on either side of it return true. It only returns true if both expressions are true.  
- `||` **Logical Or.** It only returns false of both expressions are false.
- `!` **Logical Not.** It takes a single Boolean value and inverts it. 

```((5 < 2) && (2>=3))```
The above examle would return a value of false.

# Loops
Loops check a condition. If it returns true, a code block will run. Then the condition will be checked again and if it still returns true, the code block will run again. It repeats until the condition returns false. There are three common types of loops.
1. **For.** If you need to run a code a specific number of times, use a for loop. It is the most common loop.
1. **While.** If you do not know how many times the code should run, you can use a while loop. Here the condition can be something other than a counter, and the cone will contine to loop as long as the condition is true. 
1. **Do while.** This loop is very similar to the While loop, but it has one key difference: it will always run the statements inside the curly braces at least once, even if the condition evaluates to false. 