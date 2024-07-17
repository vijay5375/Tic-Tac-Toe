# Tic Tac Toe with Minimax Algorithm

This is a console-based Tic Tac Toe game where a human plays against the computer. The computer uses the Minimax algorithm to determine its moves, ensuring either a win for the computer or a tie.

## Features

- Human vs Computer gameplay.
- Computer uses the Minimax algorithm to always find the best possible move.
- Interactive console interface.
- Clear instructions and board display.

## How to Play

1. **Run the Game:**
   Compile and run the `main.cpp` file using your preferred C++ compiler.

   ```sh
   g++ main.cpp -o TicTacToe
   ./TicTacToe
   ```

2. **Choose Who Goes First:**
   You will be prompted to decide if you want to start first. Enter `y` for yes and `n` for no.

3. **Make Your Move:**
   When it's your turn, choose a cell numbered from 1 to 9 to place your mark (`X`). The board positions are as follows:

   ```
       1 | 2 | 3 
      -----------
       4 | 5 | 6 
      -----------
       7 | 8 | 9 
   ```

4. **Game Over:**
   The game continues until either the computer wins or the game ends in a draw. The result will be displayed at the end of the game.

## Minimax Algorithm

The computer uses the Minimax algorithm to evaluate all possible moves and select the optimal one. The algorithm ensures that the computer will either win or force a draw, making it a challenging opponent.

## Code Structure

- `main.cpp` - The main file containing all the game logic and the Minimax algorithm.

## Functions

- `showBoard(char board[][SIDE])` - Displays the current state of the board.
- `showInstructions()` - Shows instructions for the player.
- `initialise(char board[][SIDE])` - Initializes the board.
- `declareWinner(int whoseTurn)` - Declares the winner of the game.
- `rowCrossed(char board[][SIDE])`, `columnCrossed(char board[][SIDE])`, `diagonalCrossed(char board[][SIDE])` - Checks if any row, column, or diagonal has been crossed.
- `gameOver(char board[][SIDE])` - Checks if the game is over.
- `minimax(char board[][SIDE], int depth, bool isAI)` - Implements the Minimax algorithm.
- `bestMove(char board[][SIDE], int moveIndex)` - Finds the best move for the computer.
- `playTicTacToe(int whoseTurn)` - Manages the gameplay loop.

## How to Contribute

If you find any issues or have suggestions for improvements, feel free to create a pull request or open an issue on GitHub.

## License

This project is open source and available under the [MIT License](LICENSE).
