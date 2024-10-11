# Sudoku Solver

## Overview

The **Sudoku Solver** is an interactive web application built using HTML, CSS, and JavaScript that helps users solve Sudoku puzzles. By leveraging the **backtracking algorithm**, this tool allows users to input an incomplete Sudoku grid and visualizes the solving process step-by-step. The application demonstrates the power of backtracking in solving constraint satisfaction problems, particularly the widely-known Sudoku puzzle.

## Features

- **Interactive Input**: Users can input their own incomplete Sudoku puzzle.
- **Step-by-Step Visualization**: Watch the backtracking algorithm solve the puzzle in real-time, showing the process of trying different numbers and backtracking when necessary.
- **User-Friendly Interface**: A clean and simple interface to input numbers and track the solving progress.
- **Error Detection**: Ensures that the input puzzle adheres to the rules of Sudoku.

## Technologies Used

- **HTML**: To structure the application layout and create the grid for the Sudoku board.
- **CSS**: For styling the grid, creating a user-friendly interface, and providing visual feedback during the solving process.
- **JavaScript**: For implementing the backtracking algorithm, handling user interactions, and dynamically updating the grid as the puzzle is solved.

## How It Works

1. **Input the Puzzle**: The user inputs the incomplete Sudoku grid via the user interface.
2. **Backtracking Algorithm**: The algorithm attempts to place digits in the empty cells by:
   - Checking if the current placement is valid based on the Sudoku rules.
   - Recursively trying different numbers and backtracking when conflicts are found.
3. **Solution Display**: Once the algorithm finds the solution, the completed grid is displayed.

### Backtracking Algorithm Explained

- **Initialization**: The algorithm begins by identifying all empty cells in the Sudoku grid.
- **Recursive Search**: It tries placing digits (1-9) in each empty cell, checking if the placement is valid by ensuring there are no repeated numbers in any row, column, or 3x3 subgrid.
- **Backtracking**: If a placement leads to a conflict, the algorithm backtracks to the previous cell and tries the next possible number.
- **Completion**: This continues until either the puzzle is completely solved or the algorithm determines the puzzle is unsolvable.

## Data Structures Used

- **2D Array (Grid Representation)**: The Sudoku board is represented as a 9x9 2D array, where each cell holds a digit or a placeholder for an empty cell.
- **Recursive Stack**: Used to keep track of the state of the board during the backtracking process.

## Getting Started

### Prerequisites
- A modern web browser

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/sudoku-solver.git
    ```

2. Navigate to the project directory:

    ```bash
    cd sudoku-solver
    ```

3. Open the `index.html` file in your web browser:

    ```bash
    open index.html
    ```

## Usage

- Input the known numbers into the Sudoku grid.
- Click the "Solve" button to start the solving process.
- The algorithm will visualize the solution step-by-step on the grid.

## Future Enhancements

- Add support for different difficulty levels.
- Allow users to load pre-defined puzzles.
- Optimize the backtracking algorithm for faster solutions.
