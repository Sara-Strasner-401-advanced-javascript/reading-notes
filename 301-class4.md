# CSS Grid
The grid-column property specifies a grid item's size and location in a grid layout, and is a shorthand property for the following properties:
- `grid-column-start` defines on which column-line the item will start.
- `grid-column-end` defines how many columns an item will span, or on which column-line the item will end.
- `grid-column-gap` defines the size of the gap between the columns in a grid layout.
- `grid-row-start` and `grid-column-start` let you easily position items in two dimensions: columns and rows. 
- Use `grid-column` and `grid-row` at the same time to set position in both dimensions.

```
grid-column: 2/6;
grid-row: 1/6;
``` 
The above code spans columns 2-6 and rows 1-6.

If typing out both `grid-column` and `grid-row` is too much for you, there's yet another shorthand for that. `grid-area` accepts four values separated by slashes: `grid-row-start`, `grid-column-start`, `grid-row-end`, followed by g`rid-column-end`.

One example of this would be `grid-area: 1 / 1 / 3 / 6;`.

## Order
If grid items aren't explicitly placed with `grid-area`, `grid-column`, `grid-row`, etc., they are automatically placed according to their order in the source code. We can override this using the `order` property, which is one of the advantages of grid over table-based layout.

By default, all grid items have an `order` of 0, but this can be set to any positive or negative value, similar to `z-index`.

## Grid-template
You can use `grid-template-columns` and g`rid-template-rows` to specift the width of your grid elements.
```
grid-template-columns: 20% 20% 20% 20% 20%;
grid-template-rows: 20% 20% 20% 20% 20%; 
```
Each rule has five values which create five columns, each set to 20% of the overall width of the garden.

This can be simplified as 
```
grid-template-columns: repeat(5, 20%);
```

## Fractional
Grid also introduces a new unit, the fractional `fr`. Each `fr` unit allocates one share of the available space. For example, if two elements are set to `1fr` and `3fr` respectively, the space is divided into 4 equal shares; the first element occupies 1/4 and the second element 3/4 of any leftover space.


