# Class 12 Reading Notes

## Charts
Chart.js is a third-party library that is easy and convenient, as far as libraries go. It uses HTML5's canvas feature to create the charts, expediting our work. 

## Canvas

 `<canvas>` supports only two basic shapes--rectangles and lines. The MDN literature says that "all other shapes must be created by combining one or more paths (lines). Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes." 

The example given is a rectangle, using three functions:

```js
fillRect(x, y, width, height) //Creates a solid rectangle.
strokeRect(x, y, width, height) //Creates a border.
clearRect(x, y, width, height) //Removes the solid part givng us a box.
```

The line capability are actually called 'paths'. Paths have a few different functions to include (but not exhaustively), the following:

```js
beginPath() //Creates a new path. 
closePath() //"Adds a straight line to the path, going to the start of the current sub-path."
stroke() //"Draws the shape by stroking its outline."
fill() //Makes the shape solid.
```

A helpful example of using the path function is as follows, taken from the MDN site:

```js

function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.beginPath();
    ctx.moveTo(75, 50);
    ctx.lineTo(100, 75);
    ctx.lineTo(100, 25);
    ctx.fill();
  }
}

```

Of course, these capabilites do not work without the Canvas tag being added the HTML page. NOTA BENE: Depending on how the code is setup, it is possible to need a closing `</canvas>` tag. Furthermore, the canvas tag always needs a context, called a rendering context. Attached to the canvas is the method, `getContext()`, which must be invoked. On a final note, it is worth noting, and rather interesting that, someone can actually use this to draw text, instead of having it typed out. 