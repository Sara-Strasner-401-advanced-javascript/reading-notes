# MUSTACHE and FLEXBOX

## Templating with Mustache
- Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source.
- Mustache is often referred to as “logic-less” because there are no if statements, else clauses, or for loops.
- mustache.js is an implementation of the mustache template system in JavaScript. It is often considered the base for JavaScript templating

```
Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });
// returns: Hello, Sherlynn
``` 
In the above, we see two braces around {{ name }}. This is Mustache syntax to show that it is a placeholder

**Mustache is NOT a templating engine.**
Mustache is a specification for a templating language. In general, we would write templates according to the Mustache specification, and it can then be compiled by a templating engine to be rendered to create an output.

### Mustache-Express
If you intend you use mustache with Node and Express, you can use mustache-express. Mustache Express lets you use Mustache and Express together easily.

## Flexbox
[*A Complete Guide to Flexbox*](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- The flex container becomes flexible by setting the display property to flex:

```
.container {
  display: flex; /* or inline-flex */
}
```
- The flex container properties are:
  - flex-direction
  - flex-wrap
  - flex-flow
  - justify-content
  - align-items
  - align-content

- The direct child elements of a flex container automatically becomes flexible (flex) items.
- The flex item properties are:
  - order
  - flex-grow
  - flex-shrink
  - flex-basis
  - flex
  - align-self


