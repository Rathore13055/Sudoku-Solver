# Sudoku Solver

## Overview
This is a **Sudoku Solver** implemented in C++ using a backtracking algorithm. The program allows the user to input a custom Sudoku puzzle (using `0` for empty cells) and solves it if a solution exists.

## Features
- Supports 9x9 Sudoku puzzles.
- Accepts user input for custom puzzles.
- Validates the Sudoku rules (row, column, and subgrid constraints).
- Displays the solved puzzle if a solution exists.

## Requirements
- A C++ compiler (e.g., GCC or Visual Studio).

## How to Use
1. **Compile the Code:**
   ```
   g++ sudoku_solver.cpp -o sudoku_solver
   ```

2. **Run the Program:**
   ```
   ./sudoku_solver
   ```

3. **Input the Puzzle:**
   - Enter the Sudoku puzzle row by row.
   - Use numbers `1-9` for filled cells and `0` for empty cells.
   - Example input:
     ```
     5 3 0 0 7 0 0 0 0
     6 0 0 1 9 5 0 0 0
     0 9 8 0 0 0 0 6 0
     8 0 0 0 6 0 0 0 3
     4 0 0 8 0 3 0 0 1
     7 0 0 0 2 0 0 0 6
     0 6 0 0 0 0 2 8 0
     0 0 0 4 1 9 0 0 5
     0 0 0 0 8 0 0 7 9
     ```

4. **View the Output:**
   - The program will display the solved Sudoku grid if a solution exists.
   - If no solution exists, it will display:
     ```
     No solution exists!
     ```

## Example
### Input:
```
5 3 0 0 7 0 0 0 0
6 0 0 1 9 5 0 0 0
0 9 8 0 0 0 0 6 0
8 0 0 0 6 0 0 0 3
4 0 0 8 0 3 0 0 1
7 0 0 0 2 0 0 0 6
0 6 0 0 0 0 2 8 0
0 0 0 4 1 9 0 0 5
0 0 0 0 8 0 0 7 9
```

### Output:
```
5 3 4 6 7 8 9 1 2
6 7 2 1 9 5 3 4 8
1 9 8 3 4 2 5 6 7
8 5 9 7 6 1 4 2 3
4 2 6 8 5 3 7 9 1
7 1 3 9 2 4 8 5 6
9 6 1 5 3 7 2 8 4
2 8 7 4 1 9 6 3 5
3 4 5 2 8 6 1 7 9
```

## Algorithm
1. **Input Handling:** Accepts a 9x9 Sudoku puzzle from the user.
2. **Validation:** Checks if a number can be placed in a cell without violating Sudoku rules.
3. **Backtracking:** Recursively tries numbers in empty cells. If no valid number can be placed, it backtracks to try a different number in the previous cells.
4. **Output:** Prints the solved Sudoku grid or a message indicating that no solution exists.

## Notes
- Ensure that the input puzzle follows Sudoku rules; otherwise, the program may fail to find a solution.
- The program assumes that the input contains exactly 9 rows and 9 columns.



