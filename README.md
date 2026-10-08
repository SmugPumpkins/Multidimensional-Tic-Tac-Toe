# Multidimensional Lists Tic-Tac-Toe

## Basic Premise

You will be given several completed Tic-Tac-Toe boards stored as **2D lists**. Each inner list represents one row of the board, and each value inside that row represents a column.

Your task is to create two functions that can work with **any of the provided boards**:

- One function that displays a board in a clear Tic-Tac-Toe format.
- One function that examines the values in the 2D list and determines whether `X` won, `O` won, or the game ended in a tie.

Your starter file will include prefilled boards for you to use.

Your functions should not be written specifically for one of these grids. The same functions should work when any 3×3 Tic-Tac-Toe grid is passed to them.

## Basic File Structure

```text
basic/
└── main.py
```

## Basic Requirements

* [ ] Use the provided Tic-Tac-Toe boards as **3×3 2D lists**, with each inner list representing one row.
* [ ] Create a function named `display_grid(grid)` that accepts a 2D list as a parameter and displays its values as a clear Tic-Tac-Toe board.
* [ ] The values displayed by `display_grid()` must come from the 2D list using row and column positions rather than having `X` and `O` characters hardcoded into the display.
* [ ] Create a function named `determine_winner(grid)` that accepts a 2D list and checks the three rows, three columns, and two diagonals for a winner.
* [ ] `determine_winner()` must correctly identify whether `X` won, `O` won, or the game ended in a tie.
* [ ] Use both functions with **every provided grid** so that each board is displayed and its result is clearly shown.

A displayed board could look similar to:

```text
 X | X | X
---+---+---
 O | O | X
---+---+---
 O | X | O

Winner: X
```

> Fully completing the Basic Requirements earns **16/20 marks, or 80%**.

## Basic Assessment — 16 Marks

| Assessment Item | Criteria | Marks |
|---|---|---:|
| 2D List Usage | Correctly works with the provided 3×3 boards as 2D lists containing rows and columns. | 2 |
| Display Function | Creates `display_grid(grid)` and uses values from the supplied 2D list to produce a clear board display. | 4 |
| Row and Column Win Detection | Correctly checks all rows and columns for three matching values. | 4 |
| Diagonal and Tie Detection | Correctly checks both diagonals and identifies games with no winner as ties. | 4 |
| Testing Multiple Grids | Uses the same functions to display and analyze every provided board. | 2 |
|  | **Total** | **16** |


## Advanced Premise

Extend your Basic program so that two people can use the same 2D list structure to **play Tic-Tac-Toe in the terminal**.

You should be able to reuse your `display_grid()` and `determine_winner()` functions from the Basic activity. Instead of analyzing boards that have already been completed, the Advanced program will begin with an empty board and update it as the players make moves.

Player 1 will use `X` and Player 2 will use `O`.

## Advanced File Structure

```text
advanced/
└── main.py
```

You can begin by copying your completed Basic program into this file.

## Advanced Requirements

* [ ] Begin with an empty 3×3 2D list and reuse the Basic `display_grid()` and `determine_winner()` functions.
* [ ] Alternate between Player `X` and Player `O`, asking each player to enter the **row and column** where they want to play.
* [ ] Use the entered row and column to update the correct value in the 2D list.
* [ ] Prevent players from selecting coordinates outside `0–2` or choosing a space that is already occupied.
* [ ] Display the updated grid after valid moves and continue playing until `determine_winner()` identifies a winner or tie.
* [ ] Validate user input and use error handling so incorrect input does not crash the program and the player can try again.

## Advanced Assessment — 4 Marks

| Assessment Item | Criteria | Marks |
|---|---|---:|
| Player Moves | Accepts row and column input and correctly updates the selected position in the 2D list. | 1 |
| Turn Management | Correctly alternates between `X` and `O` and prevents occupied spaces from being reused. | 1 |
| Game Completion | Reuses the Basic functions to display the board and correctly end the game with a winner or tie. | 1 |
| Validation and Error Handling | Rejects invalid coordinates or input without crashing and allows the player to try again. | 1 |
|  | **Total** | **4** |