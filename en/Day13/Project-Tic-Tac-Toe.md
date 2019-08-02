## Tic-Tac-Toe Game

Write a two player tic-tac-toe game.

Tic-tac-toe is a two player board game. The board is 3 x 3. The first player puts 'X' on the board and the second player puts 'O'. Whoever places three of the same mark either horizontally, or vertically or diagonally wins the game. If the board is full at the end of 9 moves and there is no winner, it is a tie.

**Game design:**
1. The board is full of dashes (-) initially. First player starts with ‘X’.
2. In each turn output the board and the player in turn
3. Program asks the player to enter a move. The player will enter two integers; row and column. Both row and column has to be between 1 and 3 inclusively. Otherwise the program will tell the move is invalid and ask the same player to make the move again. If any user selects an occupied square that is also an invalid move.
Sample tic-tac-toe board:

```
O-O
XXO
--X
```

'X' is the first player, 'O' is the second player. '-' represents empty square.



#### Task 1 (%40 of the total points):

Design the game and check for draw. In this task,  the test data will always end with a tie. You don’t need to check for the winner or tie. You can finish the game with a message “Tie!”.

**Sample Input and Output:**
('>' indicates the user input)


```
---
---
---

Player 1, please enter your move (row, col):
>1 1

X--
---
---

Player 2, please enter your move (row, col):
>2 2

X--
-O-
---

Player 1, please enter your move (row, col):
>3 4

Invalid move!

Player 1, please enter your move (row, col):
>0 2

Invalid move!

Player 1, please enter your move (row, col):
>3 2

X--
-O-
-X-

Player 2, please enter your move (row, col):
>1 2

XO-
-O-
-X-

Player 1, please enter your move (row, col):
>1 3

XOX
-O-
-X-

Player 2, please enter your move (row, col):
>2 1

XOX
OO-
-X-

Player 1, please enter your move (row, col):
>2 3

XOX
OOX
-X-

Player 2, please enter your move (row, col):
>3 3

XOX
OOX
-XO

Player 1, please enter your move (row, col):
>3 1

XOX
OOX
XXO

Tie!
```

#### Task 2 (%60 of the total points):

Design the game and check for draw and win. Finish the game whenever there is a winner. Check for tie case too.

**Sample Input and Output:**
('>' indicates the user input)

```
---
---
---

Player 1, please enter your move (row, col):
>1 1

X--
---
---

Player 2, please enter your move (row, col):
>3 4

Invalid move!

Player 2, please enter your move (row, col):
>5 6

Invalid move!

Player 2, please enter your move (row, col):
>3 1

X--
---
O--

Player 1, please enter your move (row, col):
>2 2

X--
-X-
O--

Player 2, please enter your move (row, col):
>3 2

X--
-X-
OO-

Player 1, please enter your move (row, col):
>3 3

X--
-X-
OOX

1. player won!
```

