# SMACSS and Responsive Web Design
- Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.

## Responsive Web Design
**Responsive and adaptive web design are closely related, and often transposed as one in the same.** 
- **Responsive** generally means to react quickly and positively to any change, while **adaptive** means to be easily modified for a new purpose or situation, such as change.
- A combination of the two is ideal, providing the perfect formula for functional websites. Which term is used specifically doesn’t make a huge difference.

Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media.
1. **flexible layouts**, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. 
1. **Media queries** were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example.
1. **Flexible media** ensures images, videos, and other media types are scalable, changing their size as the size of the viewport changes.

## CSS Floats
*for more information, visit [All About Floats](https://css-tricks.com/all-about-floats/)*
In web design, page elements with the CSS float property applied to them are just like the images in the print layout where the text flows around them. Floated elements remain a part of the flow of the web page.

There are four valid values for the float property.
1. `Left` and `Right` float elements those directions respectively. 
1. `None` (the default) ensures the element will not float.
1. `Inherit` which will assume the float value from that elements parent element.


### Clearing a float
Float’s sister property is `clear`. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. 

### Float collapse
One of the more bewildering things about working with floats is how they can affect the element that contains them (their “parent” element).
![collapse image](https://i0.wp.com/css-tricks.com/wp-content/csstricks-uploads/collapse.png?resize=540%2C182)

We fix it by clearing the float after the floated elements in the container but before the close of the container.
