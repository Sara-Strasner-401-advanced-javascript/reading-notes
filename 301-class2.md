# jQuery, Events, the DOM, and Pair Programming

## jQuery
jQuery is a JavaScript file you include in your pages that makes it faster and easier to write cross-browser JavaScript, based on two steps:
  1. Using CSS-style selectors to collect one or more nodes from the DOM tree.
  1. Using jQuery's built-in methods to work with the elements in that selection. 

jQuery is used to select (query) HTML elements and perform "actions" on them.
Basic syntax is: ``$("selector").action()``
- The $ accesses jQuery.
- The (selector) finds HTML elements.
- The action() is then performed on the element(s). You can place several methods on the same selector in a process known as *chaining.*

### jQuery Selector Syntax
You can also use the following syntax for selectors:
- ``$("div.menu")``- all `<div>` elements with `class="menu"`
- ``$("p:first")``- the first `<p>` element
- ``$("h1, p")``- all `<h1>` and all `<p>` elements
- ``$("div p")``- all `<p>` elements that are descendants of a `<div>` element
- ``$("*")``- all elements of the DOM

jQuery's `.ready()` method checks that the page is ready for your code to work with. 
```
$(document).ready(function() {
  jQuery code goes here
});
``` 

#### Setting Content
The `html()` and `text()` methods can be used to change the content of HTML elements.
The content to be set is provided as a parameter to the method, for example:
```
HTML:
  <div id="test">
    <p>some text</p>
  </div>
  ```

```
JS:
  $(function() {
    $("#test").text("hello!");
  });
  ```

### Adding Content
As seen above, `html()` and `text()` methods can be used to get and set the content of a selected element. However, when these methods are used to set content, the existing content is lost.
jQuery has methods that are used to add new content to a selected element without deleting the existing content:
- `append()` inserts content at the end of the selected elements.
- `prepend()` inserts content at the beginning of the selected elements.
- `after()` inserts content after the selected elements.
- `before()` inserts content before the selected elements.

### # Manipulating CSS
jQuery has several methods for CSS manipulation.
The `addClass( )` method adds one or more classes to the selected elements. For example:
```
HTML:
  <div>Some text</div>
```

```
CSS:
  .header {
    color: blue;
    font-size:x-large;
  }
  ``` 

```
JS:
  $("div").addClass("header");
```
The above code assigns the div element the class "header".

The `toggleClass()` method toggles between adding/removing classes from the selected elements, meaning that if the specified class exists for the element, it is removed, and if it does not exist, it is added.

## Dimensions
The `width()` and `height()` methods can be used to get and set the width and height of HTML elements.

Let's set both the width and height of a div to 100px, as well as set a background color for it:
```
  $("div").css("background-color", "red");
  $("div").width(100);
  $("div").height(100);
``` 

The `width()` and `height()` methods get and set the dimensions without the padding, borders and margins.
The `innerWidth()` and `innerHeight()` methods also include the padding.
The `outerWidth()` and `outerHeight()` methods include the padding and borders.

---

## 6 Reasons for Pair Programming
1. **Greater efficiency**- pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging.
1. **Engaged collaboration**- the experience is more engaging and both programmers are more focused than if they were working alone. Additionally, pair progeammers rely more on each other and can often find a solution together without needing to ask for additional help.
1. **Learning from fellow students**- If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution. A less experienced developer benefits from the experienced developer’s knowledge and guidance, and the latter benefits from explaining the topic in their own words, further solidifying their own understanding.
1. **Social skills**- helps programmers develop their interpersonal skills, which makes them a more desirable programmers to prospective employers.
1. **Job interview readiness**- For most roles, the ability to work with and learn from others and stellar communication skills are as (or more!) important to a company than specific technical skills. Thus, a common step in many interview processes involves pair programming between a current employee and an applicant. 
1. **Work environment readiness**- Developers who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.