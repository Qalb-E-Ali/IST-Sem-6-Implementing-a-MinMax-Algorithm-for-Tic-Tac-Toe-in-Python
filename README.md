# IST-Sem-6-Implementing-a-MinMax-Algorithm-for-Tic-Tac-Toe-in-Python
Objective:
 Is to implement the MinMax algorithm for building a Tic Tac Toe game. This assignment demonstrates an understanding of MinMax algorithm and its application to build a game using AI.

Tic Tac Toe Game
This code is a Python implementation of the popular Tic Tac Toe game. The game can be played by two players or against the computer. The computer uses the minimax algorithm to choose its moves.

Functions:
printBoard(board)
This function takes a dictionary named board as input and prints the current state of the game board. The board is displayed as follows:

1|2|3
-+-+-
4|5|6
-+-+-
7|8|9

Each number represents a cell on the board.
spaceIsFree(position)
This function takes an integer position as input and returns a boolean indicating whether the specified position on the game board is free or not.
insertLetter(letter, position)
This function takes a string letter ("X" or "O") and an integer position as input. It checks if the specified position on the game board is free. If the position is free, it inserts the specified letter at that position and displays the updated board. If the position is not free, it prompts the user to enter a new position. If the game is won by the current move, the function displays a message indicating the winner and exits the program. If the game ends in a draw, the function displays a message indicating that the game is a draw and exits the program.
checkForWin()
This function checks whether the current state of the game board represents a win for either player. If a win is found, the function returns True. Otherwise, it returns False.
checkWhichMarkWon(mark)
This function takes a string mark ("X" or "O") as input and checks whether the current state of the game board represents a win for that mark. If a win is found, the function returns True. Otherwise, it returns False.
checkDraw()
This function checks whether the game has ended in a draw. If the board still contains any empty cells, the function returns False. Otherwise, it returns True.
playerMove()
This function prompts the user to enter a position for their move and inserts their mark ("O") at that position on the game board.
compMove()
This function uses the minimax algorithm to select the best possible move for the computer player. It then inserts the computer player's mark ("X") at that position on the game board.
minimax(board, depth, isMaximizing)
This function recursively applies the minimax algorithm to determine the best possible move for the computer player. It takes a dictionary board, an integer depth, and a boolean isMaximizing as input. The depth variable keeps track of the depth of the recursion. The isMaximizing variable indicates whether the current player is maximizing or minimizing the score. If the computer player wins, the function returns 1. If the human player wins, the function returns -1. If the game ends in a draw, the function returns 0. If the current player is maximizing, the function returns the maximum score that can be obtained from the current state of the board. If the current player is minimizing, the function returns the minimum score that can be obtained from the current state of the board.
board
This dictionary represents the current state of the game board. Each key in the dictionary represents a cell on the board. The value associated with each key represents the mark ("X" or "O") currently occupying that cell. An empty cell is represented by a space character (" ").

How to play
To play the game, simply call the ‘playerMove’ using the playerMove() and compMove() functions.
At each turn, the program checks for a winner by calling checkForWin(), checkWhichMarkWon(), and checkDraw() functions. If a winner is found, the game ends and the winner is declared.
If there is no winner yet, the program asks the user to input a position for their move using playerMove(). The program then checks for a winner again, and if there is none, the program allows the computer to make its move by calling compMove(). The program then checks for a winner again, and the game continues until a winner is found or a draw is declared.
Finally, at the end of the game, the program asks the user if they want to play again or exit.
Overall, this program implements a simple tic-tac-toe game that can be played between a user and the computer.

Source:https://github.com/javacodingcommunity
