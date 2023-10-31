# Creating a Tic Tac Toe Game in the Terminal

### Project Description:

In this project, we will create a simple version of the classic game "Tic Tac Toe". The game will be played in the terminal, and two players will take turns to mark the spaces in a 3x3 grid. The player who succeeds in placing three of their marks in a horizontal, vertical, or diagonal row wins the game. The game will end in a draw if all nine squares are filled and no player has three marks in a row.

### Learning Objectives:

- Understand and use basic Python syntax
- Work with functions and loops
- Implement conditional statements
- Manage the game state
- Handle user input and validate it

### Example:

Here's a simple example of what the output might look like in the terminal:

```
Player 1 (X)  -  Player 2 (O)

     0   1   2
   ------------- 
0 | X | O | X | 
   -------------
1 | O | X | O | 
   -------------
2 |   |   |   | 

Player 2's turn. Choose your position (row, column): 2,1
```

### Project Structure:

1. **Display the Board**: Create a function to print out the board in a 3x3 grid.
2. **Player Input**: Allow the players to enter their moves.
3. **Check for Win or Tie**: After every move, check if there is a winner or if the game is a tie.
4. **Switch Turns**: Alternate between players after each turn.
5. **Main Game Loop**: Combine all functions to create the main game loop.

### Test Cases:

- Player 1 wins by filling the top row.
- Player 2 wins with a diagonal from top left to bottom right.
- The game is a draw when all spaces are filled without a winner.

### Sample Data:

Use this sample data to test your game. It represents a game state where Player 1 (X) has just won with a vertical line:

```python
board = [
    ['X', 'O', ' '],
    ['X', 'O', ' '],
    ['X', ' ', ' ']
]
```

### Script to Generate More Test Cases and Data:

Here's a script to generate random game states for testing:

```python
import random

def generate_random_board():
    symbols = ['X', 'O', ' ']
    return [[random.choice(symbols) for _ in range(3)] for _ in range(3)]

# Generate a random game state
random_board = generate_random_board()

# Print the board
for row in random_board:
    print(row)
```

This script will generate a random 3x3 grid filled with 'X', 'O', or empty spaces.

---

This project outline gives you a blueprint for creating the Tic Tac Toe game. Start by implementing each section step-by-step, and then combine them to complete your game. Good luck, and have fun coding!