# Sudoku_Solver
A complete, interactive Sudoku solver built with vanilla JavaScript that demonstrates backtracking algorithms in action.

🌟 Features
Puzzle Interaction
Editable 9×9 grid with input validation (only accepts 1-9)

Visual distinction between user-provided numbers (blue) and solver-generated numbers (green)

Clear grid functionality to reset the puzzle

Sample puzzle loader for quick testing

Solver Capabilities
Backtracking algorithm implementation

Validation checks for row, column, and 3×3 box constraints

Solution verification with error detection

Instant solving for most standard puzzles

🛠️ Technical Implementation
Core Algorithm
javascript
function solveSudokuBacktracking(grid) {
    for (let row = 0; row < 9; row++) {
        for (let col = 0; col < 9; col++) {
            if (grid[row][col] === 0) {
                for (let num = 1; num <= 9; num++) {
                    if (isValidMove(grid, row, col, num)) {
                        grid[row][col] = num;
                        if (solveSudokuBacktracking(grid)) return true;
                        grid[row][col] = 0;
                    }
                }
                return false;
            }
        }
    }
    return true;
}
Key Functions
isValidMove() - Checks row, column and 3×3 box constraints

updateGrid() - Handles user input with validation

updateDisplay() - Manages visual feedback

🚀 How to Use
Input your puzzle:

Click on cells and type numbers (1-9)

Leave empty (0) for unsolved cells

Solve options:

Solve Puzzle: Runs the backtracking solver

Clear Grid: Resets the entire puzzle

Load Example: Populates a sample puzzle

Understand the solution:

Blue numbers = Your original input

Green numbers = Computer's solution

🧮 Algorithm Complexity
Aspect	Complexity	Notes
Time	O(9^(n×n))	Worst case for backtracking
Space	O(n×n)	Recursion stack depth
Average solve	<1s	For standard puzzles
🌐 Deployment
This is a static web app that requires no server:

Clone the repository

Open index.html in any modern browser

(Optional) Host on GitHub Pages, Netlify, etc.

📚 Learning Resources
The code includes detailed comments explaining:

Backtracking algorithm implementation

Sudoku rule validation

DOM manipulation techniques

Event handling for user input


🐛 Known Issues
No input validation for unsolvable puzzles

Basic UI without advanced features

No difficulty levels or puzzle generation
