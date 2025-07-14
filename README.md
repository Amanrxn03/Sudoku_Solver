# Simple Sudoku Solver

A clean, interactive web-based Sudoku solver built with vanilla HTML, CSS, and JavaScript. Solve puzzles manually or let the computer solve them for you using a backtracking algorithm!

## 🎯 Features

- *Interactive Grid*: Click and type numbers directly into the 9×9 Sudoku grid
- *Automatic Solver*: Uses backtracking algorithm to solve any valid Sudoku puzzle
- *Visual Feedback*: 
  - Blue numbers = your input
  - Green numbers = computer-solved
  - Clear 3×3 box divisions
- *Example Puzzles*: Load a sample puzzle to get started
- *Input Validation*: Only accepts numbers 1-9
- *Clear Grid*: Reset the entire puzzle with one click

## 🚀 Quick Start

1. *Clone the repository*
   bash
   git clone https://github.com/Amanrxn03/sudoku-solver.git
   cd sudoku-solver
   

2. *Open in browser*
   bash
   open index.html
   
   Or simply double-click the index.html file!

## 📖 How to Use

1. *Enter Numbers*: Click on any empty cell and type a number (1-9)
2. *Solve Puzzle*: Click "Solve Puzzle" to let the computer complete it
3. *Load Example*: Click "Load Example" to try a sample puzzle
4. *Clear Grid*: Click "Clear Grid" to start over

## 🧠 Algorithm

The solver uses a *backtracking algorithm*:

1. Find the first empty cell
2. Try numbers 1-9 in that cell
3. For each number, check if it's valid (no conflicts in row, column, or 3×3 box)
4. If valid, place the number and recursively solve the rest
5. If no solution found, backtrack and try the next number
6. Repeat until solved or all possibilities exhausted

## 🛠 Technical Details

- *Pure JavaScript*: No external libraries or frameworks
- *Responsive Design*: Works on desktop and mobile devices
- *Clean Code*: Well-commented and easy to understand
- *Error Handling*: Validates input and handles unsolvable puzzles

## 📁 Project Structure


sudoku-solver/
├── index.html          # Main HTML file with embedded CSS and JavaScript
├── README.md           # This file
└── LICENSE             # MIT License (optional)


## 🎨 Customization

The code is designed to be easily customizable:

- *Colors*: Modify the CSS variables for different themes
- *Grid Size*: Easy to adapt for different puzzle sizes
- *Algorithms*: Add different solving techniques (naked singles, hidden pairs, etc.)
- *Features*: Add timer, difficulty levels, or puzzle generation

## 🤝 Contributing

Contributions are welcome! Here are some ideas:

- Add puzzle generation functionality
- Implement additional solving techniques
- Add difficulty levels
- Create a mobile-friendly version
- Add animations for the solving process


## 🔧 Future Enhancements

- [ ] Puzzle generation with difficulty levels
- [ ] Timer and scoring system
- [ ] Hint system
- [ ] Save/load puzzles
- [ ] Multiple solving algorithms
- [ ] Mobile app version

---
