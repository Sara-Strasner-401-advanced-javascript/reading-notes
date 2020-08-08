# Understanding the Problem Domain
"Problem domain" refers to the scope of a given problem, which thereby defines the scope of the solution. John Sonmez in his article [Understanding The Problem Domain Is The Hardest Part Of Programming] (https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming/) states:
> "You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem."
In other words, focus in on one aspect of the problem and really understanding it before zooming out to the bigger picture. 

He also recommends trying to become better at problem domains and ensure you have a firm grasp on the problem before trying to solve it with code. 

# JS Object Literals
Objects group together a set of variables and functions to create a model of something you would recognize from the real world. In an object, variables and functions take on new names. 
- In an object, variables become known as properties.
- In an object, functions become known as methods. 
- Like variables and named functions, properties and methods have a name and a value. In an object, that name is called a key. An object cannot have two keys with the same name. 

Literal notation is the easiest and most popular way to create objects. 
You access the properties or methods of an object using dot notation. You can also access properties using square brackets. 


# The Document Object Model
The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it's in the browser window. It is not part of HTML or JS; it is a separate set of rules. 

As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it's stored in the browser's memory. DOM trees have four types of nodes.
1. document nodes
1. element nodes
1. attribute nodes
1. text nodes

You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax. Whenever a DOM query can return more than one node, it will always return a `NodeList.` From an element node, you can access and update its content using properties such as `textContent` and `innerHTML` or using DOM manipulation techniques. 

