Here’s a draft README for your `MacMohan-24-Squares-Puzzle` project:

---

# MacMohan 24 Squares Puzzle

Welcome to the MacMohan 24 Squares Puzzle repository! This project features a JavaScript-based interactive puzzle game that involves arranging and rotating squares to solve the puzzle. 

## Overview

The MacMohan 24 Squares Puzzle is a grid-based puzzle game where the objective is to arrange squares with different color patterns to meet specific constraints. This project includes functionalities for shuffling, rotating, and interacting with the puzzle, providing an engaging way to test spatial reasoning and problem-solving skills.

## Features

- **Interactive Grid**: 6x4 grid of squares that can be moved and rotated.
- **Dynamic Shuffling**: Randomly shuffle the squares to create new puzzle states.
- **Rotation Mechanism**: Rotate squares to fit the desired pattern.
- **Real-time Drawing**: Visual feedback as you interact with the puzzle.

## Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/krishnapatel36/MacMohan-24-Squares-Puzzle.git
   ```

2. **Navigate to the Project Directory**:

   ```bash
   cd MacMohan-24-Squares-Puzzle
   ```

3. **Open the `index.html` File**:

   Open the `index.html` file in your browser to view and interact with the puzzle.

## Usage

1. **Interact with the Puzzle**:
   - **Click and Drag**: Click and drag squares to move them around the grid.
   - **Rotate**: Quickly click on a square to rotate it if it’s not moving.

2. **Shuffle**:
   - The puzzle can be shuffled using the shuffle function in the code.

3. **Check the Puzzle**:
   - The puzzle will provide visual feedback and scoring based on the arrangement of the squares.

## Code Description

### CanvasHelper

- **`lineRel(x1, y1, dx, dy)`**: Draws a line from `(x1, y1)` to `(x1 + dx, y1 + dy)`.
- **`line(x1, y1, x2, y2)`**: Draws a line from `(x1, y1)` to `(x2, y2)`.
- **`circle(x, y, r)`**: Draws a filled circle with center `(x, y)` and radius `r`.
- **`posFromEvent(e)`**: Calculates the position of a mouse event relative to the canvas.
- **`poly(pts)`**: Draws a polygon based on an array of points.
- **`fillPoly()`**: Fills the polygon defined in `poly()`.
- **`drawPoly()`**: Strokes the polygon defined in `poly()`.
- **`rand(seed)`**: Generates a pseudo-random number based on a seed.

### Squares24

- **`init()`**: Initializes the puzzle, sets up the canvas, and starts the animation loop.
- **`initialSetup()`**: Generates and shuffles the squares.
- **`genSquares()`**: Creates the initial set of square patterns.
- **`shuffle()`**: Randomly shuffles the squares.
- **`shuffleAndDraw()`**: Shuffles the squares and redraws the puzzle.
- **`setupGeometry(canvas)`**: Sets the canvas dimensions based on the puzzle size.
- **`draw()`**: Draws the puzzle on the canvas.
- **`drawSquare(index, dx, dy, da)`**: Draws an individual square with optional translation and rotation.
- **`drawTriangle(cx, cy, a, color, stricken)`**: Draws a colored triangle with optional border.
- **`coordsByIndex(index)`**: Calculates the coordinates for a given index in the grid.
- **`rotate(index)`**: Rotates the square pattern at a given index.
- **`recalculate()`**: Recalculates the puzzle score and updates the display.
- **`recalculateVert()`**: Scores vertical matches in the grid.
- **`recalculateHorz()`**: Scores horizontal matches in the grid.
- **`recalculateBorder()`**: Scores border matches.
- **`mouseDown(event)`**: Handles mouse down events to start moving squares.
- **`mouseUp(event)`**: Handles mouse up events to drop squares or rotate them.
- **`mouseMove(event)`**: Updates the position of moving squares.
- **`animator()`**: Updates the rotation animation.
- **`nearestSquare(pos)`**: Finds the nearest square to a given position.

## Contributing

Contributions are welcome! If you’d like to contribute to the project, please fork the repository and submit a pull request with your changes. Ensure your code adheres to the existing style and includes appropriate tests.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

For any questions or support, please contact:

- **Krishna Patel**: [krishnapatel36@gmail.com](mailto:krishnapatel36@gmail.com)

---

Feel free to modify any sections to better fit your project’s specifics!
