# Chart.js, Canvas 

## EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS 

```


Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.
A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page.

Setting up

The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in.

Drawing a line chart

To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart.

If you test your file in a browser you’ll now see a cool animated line graph.


Drawing a pie chart

You’ll notice that this time, we are going to supply some options to the chart.


Drawing a bar chart

Finally, let’s add a bar chart to our page.

Conclusion

The great things about Chart.js are that it’s simple to use and really very flexible.

```

## Chart.js 

```
- Installation
You can get the latest version of Chart.js from npm , the GitHub releases , or use a Chart.js CDN . Detailed installation instructions can be found on the installation page.

- Creating a Chart
It's easy to get started with Chart.js. All that's required is the script included in your page along with a single <canvas> node to render the chart.

In this example, we create a bar chart for a single dataset and render that in our page. You can see all the ways to use Chart.js in the usage documentation.
>
> <canvas id="myChart" width="400" height="400"></canvas>
> <script>
> var ctx = document.getElementById('myChart').getContext('2d');
> var myChart = new Chart(ctx, {
>    type: 'bar',
>    data: {
>        labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
>        datasets: [{
            label: '# of Votes',
            data: [12, 19, 3, 5, 2, 3],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        scales: {
            y: {
                beginAtZero: true
            }
>        }
>    }
> });
> </script>
> 
       
    
- Contributing
Before submitting an issue or a pull request to the project, please take a moment to look over the contributing guidelines first.


- License
Chart.js is available under the MIT license .


```

## Basic usage of canvas  

```
The element

At first sight a looks like the element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the element has only two attributes, width and height. The element can be styled just like any normal image . These rules, however, don't affect the actual drawing on the canvas.

We'll see how this is done in a dedicated chapter of this tutorial. When no styling rules are applied to the canvas it will initially be fully transparent.

Fallback content

The element differs from an tag in that, like for , , or elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers. Providing a useful fallback text or sub DOM helps to make the canvas more accessible.

Required tag

If fallback content is not needed, a simple is fully compatible with all browsers that support canvas at all.

The rendering context

The element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. The canvas is initially blank. The element has a method called getContext, used to obtain the rendering context and its drawing functions. The first line in the script retrieves the node in the DOM representing the element by calling the document.

Once you have the element node, you can access the drawing context using its getContext method.

Checking for support

The fallback content is displayed in browsers which do not support .

A skeleton template

Here is a minimalistic template, which we'll be using as a starting point for later examples.

```

##  Drawing shapes with canvas

```

Now that we have set up our canvas environment, we can get into the details of how to draw on the canvas.

The grid

Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. Normally 1 unit in the grid corresponds to 1 pixel on the canvas.

Drawing rectangles

All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.

In upcoming pages we'll see two alternative methods for clearRect, and we'll also see how to change the color and stroke style of the rendered shapes. Unlike the path functions we'll see in the next section, all three rectangle functions draw immediately to the canvas.

Draws a solid shape by filling the path's content area. The first step to create a path is to call the beginPath. Internally, paths are stored as a list of sub-paths which together form a shape. Every time this method is called, the list is reset and we can start drawing new shapes.

The second step is calling the methods that actually specify the paths to be drawn.

Moving the pen

One very useful function, which doesn't actually draw anything but becomes part of the path list described above, is the moveTo function.

Moves the pen to the coordinates specified by x and y. When the canvas is initialized or beginPath is called, you typically will want to use the moveTo function to place the starting point somewhere else. We could also use moveTo to draw unconnected paths.



Draws a line from the current drawing position to the position specified by x and y. This method takes two arguments, x and y, which are the coordinates of the line's end point. The starting point is dependent on previously drawn paths, where the end point of the previous path is the starting point for the following, etc. The starting point can also be changed by using the moveTo method. This is, as mentioned above, because shapes are automatically closed when a path is filled, but not when they are stroked.

arcTo

Draws an arc with the given control points and radius, connected to the previous point by a straight line. It draws 12 different arcs all with different angles and fills. The two for loops are for looping through the rows and columns of arcs. For each arc, we start a new path by calling beginPath.

In the code, each of the parameters for the arc is in a variable for clarity, but you wouldn't necessarily do that in real life. The x and y coordinates should be clear enough. radius and startAngle are fixed. Finally, the if statement makes the top half stroked arcs and the bottom half filled arcs.

Cubic Bezier curves

This example draws a heart using cubic Bézier curves.

Making combinations

So far, each example on this page has used only one type of path function per shape. So in this final example, let's combine all of the path functions to make a set of very famous game characters.

The resulting image looks like this

Here, all we're doing is using it to change the fill color for paths from the default color of black to white, and then back again.

Path2D objects

To simplify the code and to improve performance, the Path2D object, available in recent versions of browsers, lets you cache or record these drawing commands.

All path methods like moveTo, rect, arc or quadraticCurveTo, etc., which we got to know above, are available on Path2D objects. Adds a path to the current path with an optional transformation matrix.

```

## Applying styles and colors

```

A strokeStyle example

This example is similar to the one above, but uses the strokeStyle property to change the colors of the shapes' outlines.

Transparency

This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.

The globalAlpha property can be useful if you want to draw a lot of shapes on the canvas with similar transparency, but otherwise it's generally more useful to set the transparency on individual shapes when setting their colors. Because the strokeStyle and fillStyle properties accept CSS rgba color values, we can use the following notation to assign a transparent color to them. // Assigning transparent colors to stroke and fill style ctx. The rgba function is similar to the rgb function but it has one extra parameter.

A globalAlpha example

On top of these, we'll draw a set of semi-transparent circles. The globalAlpha property is set at 0.2 which will be used for all shapes from that point on. The final result is a radial gradient.

An example using rgba

Using rgba gives you a little more control and flexibility because we can set the fill and stroke style individually. // Draw background // Draw semi transparent rectangles ctx.

A lineWidth example

This property sets the current line thickness. The line width is the thickness of the stroke centered on the given path. In other words, the area that's drawn extends to half the line width on either side of the path. Because canvas coordinates do not directly reference pixels, special care must be taken to obtain crisp horizontal and vertical lines.

In the images below, the grid represents the canvas coordinate grid. The squares between gridlines are actual on-screen pixels. If you consider a path from to with a line thickness of 1.0, you end up with the situation in the second image. The actual area to be filled only extends halfway into the pixels on either side of the path.

An approximation of this has to be rendered, which means that those pixels being only partially shaded, and results in the entire area being filled in with a color only half as dark as the actual stroke color. This is what happens with the 1.0 width line in the previous example code. To fix this, you have to be very precise in your path creation. See the next two sections for demonstrations of these additional line styles.

For even-width lines, each half ends up being an integer amount of pixels, so you want a path that is between pixels that is, to , instead of down the middle of pixels. While slightly painful when initially working with scalable 2D graphics, paying attention to the pixel grid and the position of paths ensures that your drawings will look correct regardless of scaling or any other transformations involved. A 1.0-width vertical line drawn at the correct position will become a crisp 2-pixel line when scaled up by 2, and will appear at the correct position.

A lineCap example

The lineCap property determines how the end points of every line are drawn.



The ends of lines are squared off by adding a box with an equal width and half the height of the line's thickness. In this example, we'll draw three lines, each with a different value for the lineCap property. This adds a semicircle to the end that has a radius half the width of the line. This adds a box with an equal width and half the height of the line thickness.

A lineJoin example

The lineJoin property determines how two connecting segments with non-zero lengths in a shape are joined together . By default this property is set to miter.

A demo of the miterLimit property

As you've seen in the previous example, when joining two lines with the miter option, the outside edges of the two joining lines are extended up to the point where they meet. The miterLimit property determines how far the outside connection point can be placed from the inside connection point. It can equivalently be defined as the maximum allowed ratio of the distance between the inside and outside points of jonction of edges, to the total line width. A miter limit equal to √2 ≈ 1.4142136 will strip miters for all acute angles, keeping miter joins only for obtuse or right angles.

A miter limit equal to 1.0 is valid but will disable all miters. Values below 1.0 are invalid for the miter limit. Here's a little demo in which you can set miterLimit dynamically and see how this effects the shapes on the canvas. // Clear canvas ctx.

MiterLimit = parseFloatdocument.

Using line dashes

The setLineDash method accepts a list of numbers that specifies distances to alternately draw a line and a gap and the lineDashOffset property sets an offset where to start the pattern.

The position is a number between 0.0 and 1.0 and defines the relative position of the color in the gradient, and the color argument must be a string representing a CSS , indicating the color the gradient should reach at that offset into the transition. You can add as many color stops to a gradient as you need. Below is a very simple linear gradient from white to black.

A createLinearGradient example

In this example, we'll create two different gradients. As you can see here, both the strokeStyle and fillStyle properties can accept a canvasGradient object as valid input. The first is a background gradient. As you can see, we assigned two colors at the same position.

A createRadialGradient example

In this example, we'll define four different radial gradients. Because we have control over the start and closing points of the gradient, we can achieve more complex effects than we would normally have in the "classic" radial gradients we see in, for instance, Photoshop . This isn't very obvious from the code because it uses two different CSS color methods as a demonstration, but in the first gradient #019F62 = rgba.

A createConicGradient example

In this example, we'll define two different conic gradients. A conic gradient differs from a radial gradient as, instead of creating circles, it circles around a point.

image is a CanvasImageSource that is, an HTMLImageElement, another canvas, a element, or the like.

We use this method to create a CanvasPattern object which is very similar to the gradient methods we've seen above. Once we've created a pattern, we can assign it to the fillStyle or strokeStyle properties.

A createPattern example

In this last example, we'll create a pattern to assign to the fillStyle property. Src = 'canvas_createpattern.

A shadowed text example

We will look at the font property and fillText method in the next chapter about drawing text.


```


## Drawing text


```

The canvas rendering context provides two methods to render text: fillText

Fills a given text at the given position.

Strokes a given text at the given position.

Styling text

The current text style being used when drawing text.

Text alignment setting.

Baseline alignment setting. The default value is alphabetic.

The top of the em square is roughly at the top of the glyphs in a font, the hanging baseline is where some glyphs like आ are anchored, the middle is half-way between the top of the em square and the bottom of the em square, the alphabetic baseline is where characters like Á, ÿ, f, and are anchored, the ideographic baseline is where glyphs like 私 and 達 are anchored, and the bottom of the em square is roughly at the bottom of the glyphs in a font.

Gecko-specific notes

In Gecko , some prefixed APIs were implemented in earlier versions to draw text on a canvas


```