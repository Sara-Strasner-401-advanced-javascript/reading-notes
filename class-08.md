# CSS
For a few preliminary notes on CSS, see [Daily Reading Assignment 4: Links & Layout](class-04.md). 

## CSS Layout
CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box. Block level elements start on a new line. Inline elements flow in between surrounding text. If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element. 

## Key Terms
- `position:static` every element has a static position by default, so the element will stick to the normal page flow
- `position:relative` moves an element in relation to where it would have been in normal flow
- `position: absolute` takes an element out of normal flow and no longer affects the position of other elements on the page
- `position: fixed` positions an element relative to the viewport, which means it always stays in the same place even if the page is scrolled
- `z-index`  specifies the stack order of an element
- `float` allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible. Float can be used to place elements side by side. 
- `clear` specifies on which sides of an element floating elements are not allowed to float.


## CSS Resources
- For a list of common CSS selectors, see [MDN CSS Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors).
- For practice with CSS, visit [CSS Diner](https://flukeout.github.io/). 
- For inspiration, see [CSS Zen Garden](http://www.csszengarden.com/).
- To test simple CSS code online, utilize [CodePen](https://codepen.io/). 