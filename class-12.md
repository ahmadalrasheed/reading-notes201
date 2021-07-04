## EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS
![charts](https://www.webdesignerdepot.com/cdn-origin/uploads/2013/11/featured5.jpg)

> ***Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.***

> ***A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.***

> ***To see how to use chart.js we’re going to create a set of 3 graphs; one will show the number of buyers a fictional product has over the course of 6 months, this will be a line chart; the second will show which countries the customers come from, this will be the pie chart; finally we’ll use a bar chart to show profit over the period.***

### Creating a Chart

![chart.js](https://www.codeproject.com/KB/scripting/771710/image1.png)

***after installation it's easy to get started with Chart.js. All that's required is the script included in your page along with a single <canvas> node to render the chart.***

***In this example, we create a bar chart for a single dataset and render that in our page. You can see all the ways to use Chart.js in the usage documentation.***


## Basic usage of canvas
### The <canvas> element

> `<canvas id="tutorial" width="150" height="150"></canvas>`


**At first sight a `<canvas>`looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.**


### The rendering context

***The `<canvas>` element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the 2D rendering context. Other contexts may provide different types of rendering; for example, WebGL uses a 3D context based on OpenGL ES.***

***The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it. The `<canvas>` element has a method called getContext(), used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context. For 2D graphics, such as those covered by this tutorial, you specify "2d" to get a CanvasRenderingContext2D.***


> var canvas = document.getElementById('tutorial');
> var ctx = canvas.getContext('2d');


## Drawing shapes with canvas
### Drawing rectangles


***Unlike SVG, `<canvas>` only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.***

***First let's look at the rectangle. There are three functions that draw rectangles on the canvas:***

***fillRect(x, y, width, height) Draws a filled rectangle. strokeRect(x, y, width, height) Draws a rectangular outline. clearRect(x, y, width, height) Clears the specified rectangular area, making it fully transparent. Each of these three functions takes the same parameters.x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.***

***Below is the draw() function from the previous page, but now it is making use of these three functions.***

#### Rectangular shape example

> function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');
  ctx.fillRect(25, 25, 100, 100);
  ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
  }
}


## Applying styles and colors

### Colors

***Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.***

`fillStyle = color`


***Sets the style used when filling shapes.`strokeStyle = color` Sets the style for shapes' outlines. color is a string representing a CSS `<color>`, a gradient object, or a pattern object We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black `(CSS color value #000000)`.***


### A fillStyle example

***In this example, we once again use two for loops to draw a grid of rectangles, each in a different color. The resulting image should look something like the screenshot. There is nothing too spectacular happening here. We use the two variables i and j to generate a unique RGB color for each square, and only modify the red and green values. The blue channel has a fixed value. By modifying the channels, you can generate all kinds of palettes. By increasing the steps, you can achieve something that looks like the color palettes Photoshop uses.***

> function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  for (var i = 0; i < 6; i++) {
    for (var j = 0; j < 6; j++) {
      ctx.fillStyle = 'rgb(' + Math.floor(255 - 42.5 * i) + ', ' +
                       Math.floor(255 - 42.5 * j) + ', 0)';
      ctx.fillRect(j * 25, i * 25, 25, 25);
    }
  }
}


