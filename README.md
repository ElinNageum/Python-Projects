# Python-Projects
I have recently started learning Python. I'd love to develop advanced skills by creating more projects.

Main Implementations of **Sudoku**:
1. **Sudoku Solver Functions:**
    - `find_next_empty(puzzle)`: Finds the next empty cell (represented by -1) in the Sudoku puzzle. Returns the row and column of the empty cell, or `(None, None)` if there are no empty cells left.
    - `is_valid(puzzle, guess, row, col)`: Checks if placing a `guess` in the given `row` and `col` of the Sudoku `puzzle` is a valid move. Checks for validity in the same row, column, and 3x3 square.
    - `solve_sudoku(puzzle)`: Solves the Sudoku puzzle using a backtracking algorithm. It recursively tries to fill in the empty cells with valid guesses. If a solution exists, it mutates the `puzzle` to be the solution and returns `True`. If no solution exists, it returns `False`.
2. **Example Board and Solving:**
    - The script initializes an example Sudoku board (`example_board`) that needs to be solved.
    - It then calls `solve_sudoku(example_board)` to solve the example Sudoku puzzle and prints the solution using `pprint`.
3. **Tkinter GUI (Graphical User Interface):** (need to be fixed)
    - The script creates a Tkinter window (`root`) for the GUI.
    - It creates a 9x9 grid of text entry fields (`entries`) representing the Sudoku puzzle. The initial values from the `example_board` are inserted into these entry fields.
    - The `solve_button` is a button labeled "Solve." When clicked, it calls the `solve` function.
    - The `solve` function reads the user-input values from the entry fields, validates them, solves the Sudoku puzzle using `solve_sudoku`, and updates the GUI with the solution.
    - The Tkinter event loop (`root.mainloop()`) runs, allowing the user to interact with the GUI.
  
Adapted from https://www.youtube.com/watch?v=8ext9G7xspg
