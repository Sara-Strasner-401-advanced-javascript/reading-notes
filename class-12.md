# Chart.js, Canvas


## Chart.js
A great way to get started with charts is with Chart.js, which is a JavaScript plugin that renders graphs. To use Chart.js, you need to download it into the directory you'll be using and import the script into your HTML page. Then, add a `<canvas>` element to you HTML page and a `<source>` link to your JS page, where you will create the data.

For more information about Chart.js, see [this article from SquareSpace](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/). 

[HERE](https://www.chartjs.org/docs/latest/) are additional Chart.js documents. 

## Canvas.API
- The `<canvas>` element is used to draw graphics on a web page.It is only a container for graphics. You must use JavaScript to actually draw the graphics.

## Drawing Shapes with Canvas
- `<canvas>` only supports two primitive shapes: rectangles and paths (lists of points connected by lines. 
- Rectangles 
  - `fillRect(x, y, width, height)`
    Draws a filled rectangle.
  - `strokeRect(x, y, width, height)`
    Draws a rectangular outline.
  - `clearRect(x, y, width, height)`
    Clears the specified rectangular area, making it fully transparent.
- Paths
  - A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. 
  - `beginPath()`
    Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
  - Path methods
    Methods to set different paths for objects.
  - `closePath()`
    Adds a straight line to the path, going to the start of the current sub-path.
  - `stroke()`
    Draws the shape by stroking its outline.
  - `fill()`
    Draws a solid shape by filling the path's content area.

## Applying styles and colors
There are two important properties tha can apply colors to a shape: `fillStyle` and `strokeStyle`.
- `fillStyle = color`
  Sets the style used when filling shapes.
- `strokeStyle = color`
  Sets the style for shapes' outlines.

## Drawing Text
The canvas rendering context provides two methods to render text:
- `fillText(text, x, y [, maxWidth])`
  Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
- `strokeText(text, x, y [, maxWidth])`
  Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
