20-07-2023
KALADAR

# Kaladar - Canvas Utility Functions

Kaladar is an npm package that provides a comprehensive set of JavaScript functions designed to simplify common tasks when working with HTML5 Canvas. Whether you're creating games, interactive graphics, or data visualizations, Kaladar makes it easier to manage coordinates, draw shapes, generate random values, and perform various geometric calculations on the canvas.

## Installation

You can install Kaladar using npm:

```bash
npm install kaladar
```

## Usage

To harness the power of Kaladar in your JavaScript projects, import the package and access its functions as needed. Here's an example of how to import and use some of the functions:

```javascript
const kaladar = require("kaladar");

// Set canvas width and height to fit the window
kaladar.maxify();

// Draw a horizontal axis
kaladar.drawHorizontal();

// Generate a random color
const randomColor = kaladar.randomColor();

// Draw a circle on the canvas
kaladar.drawCircle(100, 100, 30, randomColor);
```

## Functions Overview

Kaladar offers a diverse range of functions, organized into the following categories:

### Canvas Size and Coordinates

- `maxify(cutBy)`: Adjust canvas dimensions to fit the window, with an optional margin.
- `middleX()`: Retrieve the X-coordinate of the canvas center.
- `middleY()`: Retrieve the Y-coordinate of the canvas center.
- `endX()`: Obtain the X-coordinate at the canvas's end.
- `endY()`: Obtain the Y-coordinate at the canvas's end.
- `fillCanvas(color)`: Fill the entire canvas with a specified color.
- `clearCanvas()`: Clear the entire canvas.
- `drawHorizontal(y, color)`: Draw a horizontal axis at the specified Y-coordinate.
- `drawVertical(x, color)`: Draw a vertical axis at the specified X-coordinate.
- `drawAxes(color)`: Draw both horizontal and vertical axes.

### Random Number Generation

- `randRange(min, max)`: Generate a random rational number within a specified range.
- `randInt(min, max)`: Generate a random integer within a specified range.
- `randItem(arr)`: Retrieve a random element from an array.
- `randomSign()`: Generate a random sign (-1 or 1).
- `randomColor(opacity)`: Generate a random RGBA color.

### Geometric Calculations

- `getDistance(x1, y1, x2, y2)`: Calculate the distance between two points.
- `isPointInsideCircle(x1, y1, x2, y2, r2)`: Determine if a point is inside a circle.
- `isPointInsideSquare(x1, y1, x2, y2, size2)`: Determine if a point is inside a square.
- `isPointInsideRectangle(x1, y1, x2, y2, length2, breadth2)`: Determine if a point is inside a rectangle.
- `getDegreeFromRadian(rad)`: Convert radians to degrees.

### Object and Array Manipulation

- `updateArray(arr)`: Update objects in an array using their `update` methods.
- `updateObject(obj)`: Update an object using its `update` method.
- `arrayOfObjects(n, class)`: Create an array of objects based on a given class.
- `newX(x, y, r, theta)`: Calculate a new X-coordinate based on polar coordinates.
- `newY(x, y, r, theta)`: Calculate a new Y-coordinate based on polar coordinates.
- `drawLineSegment(x1, y1, x2, y2, color, lineWidth)`: Draw a line segment between two points.

### Complex Drawing Functions

- `drawCircle(x, y, r, lineColor, lineWidth)`: Draw a circle on the canvas.
- `drawRectangle(x, y, length, breadth, lineColor, lineWidth)`: Draw a rectangle on the canvas.
- `fillRectangle(x, y, length, breadth, fillColor, lineColor, lineWidth)`: Fill and draw a rectangle.
- `drawBall(x, y, r, fillColor, lineColor, lineWidth)`: Draw a filled circle.
- `circleAwayFromSquare(cX, cY, cR, x2, y2, size2)`: Check if a circle is entirely outside a square.
- `circleAwayFromRectangle(cX, cY, cR, x2, y2, length2, breadth2)`: Check if a circle is entirely outside a rectangle.

## License

Kaladar is distributed under the MIT License, allowing you to freely use and modify it in your projects. Contributions and bug reports are highly welcome.

---

With Kaladar, simplifying your HTML5 Canvas-based projects becomes a breeze. Enjoy the flexibility and efficiency it brings to your canvas-related tasks!
