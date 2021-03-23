# Reading Notes 12 Course 201

## Charts in JS

__*Line Charts*__

To draw a line chart you need to create a canvas element in html:
> < canvas id="ex" width="" height="" >

you then need to create a script to retrieve the canvas contents
> < script > let ex = document.getElementById('ex').getContext('2d) new chart(ex).Line(exData); < /script >

You then need to create data using labels and datasets (used to describe the values on the chart)

__*Pie Chart*__

To draw a pie chart you need to create a canvas element in html:
> < canvas id="ex" width="" height="" >

Then get context and instantiate the chart:
> < script > let ex = document.getElementById('ex').getContext('2d) new chart(ex).Pie(pieData,pieOptions); < /script >

The data on the chart is simpler, and only uses a value, and a color for each section

Then add pie options:
> let pieOptions = { segmentShowStroke : false, animateScale: true}

__*Bar Chart*__
To create a bar chart you need to add a canvas element to html:
> < canvas id="income" width="600" height="400">< /canvas >

Then retrieve the data in JS using:
> var income = document.getElementById("income").getContext("2d");
new Chart(income).Bar(barData);

Then add data

__*Drawing Shapes with Canvas*__

Drawing rectangles:
> fillRect(x, y, width, height) FILLED RECTANGLE
>> strokeRect(x, y, width, height) RECTANGLE OUTLINE
>>> clearRect(x, y, width, height) TRANSPARENT

__*Paths*__

A path is a list of points connected by lines to create differnt shapes, and curves of different widths and colors. To create a path you

1. Create path using beginPath()

2. Use drawing commands to draw into the path

3. Stoke or fill the path to render it once completed

beginPath() - Creates new path. Future draw commands are directed into the path to build it up

closePath() - Adds a straight line to the path, going to the start of the current subpath

stroke() - Draws the shape by creating its outline

fill() - Draws a solid shape and fills the paths content area

__*Moving Pen*__

> moveTo(x, y) - will move te pen to coordinates specified by x and y

__*Lines*__

> lineTo(x,y) - Draws a line from current drawing position to the specified x and y positions

__*Arcs*__

To draw arcs you use arc() and arcTo() methods:

> arc(x, y, radius, startAngle, endAngle, anticlockwise)
anticlockwise will indicate the direction(default clockwise)
>arcTo(x1, y1, x2, y2, radius)
Creates an arc with 4 different points and a radius

__*Bezier and quadratic curves*__

> quadraticCurveTo(cp1x, cp1y, x, y)

Creates a line from current start point to the end point of x,y. The control point to create a curve is cp1x and cp1y

> bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)

Same thing but with 2 control points to adjust the curve

Path2D Object - Allows you to cache or record drawing commands and lay them back quickly

__*Adding Color*__

> fillStyle = color
>> strokeStyle = color

[<== Back to Main Page](README.md)
