# Authentication

## Review, Research, and Discussion
1. Explain what a “Singleton” is (in Computer Science terms)
The singleton design pattern restricts the instantiation of a class to a single instance, typically through the use of a private constructor method. from [What Is a Singleton?](https://medium.com/better-programming/what-is-a-singleton-2dc38ca08e92)
1. Explain how the Singleton pattern can be used with Node modules, specifically with classes
Singletons are sometimes considered to be an alternative to global variables or static classes. Singletons hold an instantiated object, whereas static classes do not. from [What Is a Singleton?](https://medium.com/better-programming/what-is-a-singleton-2dc38ca08e92)
1. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
I'm not quite sure I understand the question, but I would probably start with test-driven development and first write my tests to outline what I want my middleware to do, then start writing code.

## Document the following Vocabulary Terms
- Router Middleware- middleware functions like signposts along the way for the train track of the request object. Router is a type of Express middlware that handles requests and sends them via the approproate route. 
- Dynamic Module Loading- Loading the entire program into the main memory before start of the program execution is called as static loading. Loading the program into the main memory on demand is called as dynamic loading. from [Difference between Loading and Linking](https://www.geeksforgeeks.org/difference-between-loading-and-linking/)
- Singleton Pattern- The singleton design pattern restricts the instantiation of a class to a single instance, typically through the use of a private constructor method. 
- CRUD -> REST Method- CRUD principles are mapped to REST commands to comply with the goals of RESTful architecture
- Mock Testing- Mocking is primarily used in unit testing. An object under test may have dependencies on other (complex) objects. To isolate the behavior of the object you want to replace the other objects by mocks that simulate the behavior of the real objects. In short, mocking is creating objects that simulate the behavior of real objects. from [What is mocking?](https://stackoverflow.com/questions/2665812/what-is-mocking)


## Preview
1. Which 3 things had you heard about previously and now have better clarity on?
- NoSQL databases vs SQL databases, testing, modularization
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- traversing linked lists, Big O, how mongo and mongoose interact
1. What are you most excited about trying to implement or see how it works?