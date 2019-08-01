# Pennies in the Box Game

Pennies in boxes is a two player board game. The board is a sequence of N boxes. Initially, each box has some pennies. Players take turns. In each turn, current player picks either the leftmost or the rightmost box. The game ends when there are no remaining boxes. At the end of the game, the player who has most pennies wins the game. If both players have the same amount of pennies then the game is tied. An example game is as follows:

```
Board (N = 8)        Player turn  Player move  Player 1 score  Player 2 score
-----------------    -----------  -----------  --------------  --------------
8 12 2 4 6 3 7 10        1           Right          10              0
8 12 2 4 6 3 7           2           Right          10              7
8 12 2 4 6 3             1           Left           18              7
 12 2 4 6 3              2           Left           18             19
    2 4 6 3              1           Left           20             19
      4 6 3              2           Left           20             23
        6 3              1           Left           26             23
          3              2           Right          26             26
```

- The game is a tie!

## Task 1 (%60 of the total points):

Write a two player pennies in boxes game.

**Game design:**
1. The boss initially enter the size of the board N (1<=N<=20)  and N integers each number is greater than 0.
2. Player 1 starts the game.
3. In each turn, output the board, the player in turn and their scores.
4. Program asks the player to enter the move. The player will enter 1 for left or 2 for right. Otherwise the program will tell the move is invalid and ask the same player to make the move again.
5. If there is a winner or it is a tie, the program should output the game result and stop.

**Sample Input and Output:**
('>' indicates the user input)

```
Enter the number of boxes:
>5
Enter pennies in each box:
>1 5 8 3 17

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>1

Boxes:
5 8 3 17
Player 1 score:1
Player 2 score:0
Enter player 2 move (1 for leftmost,2 for rightmost):
>2

Boxes:
5 8 3
Player 1 score:1
Player 2 score:17
Enter player 1 move (1 for leftmost,2 for rightmost):
>7
Invalid move!

Enter player 1 move (1 for leftmost,2 for rightmost):
>7
Invalid move!

Enter player 1 move (1 for leftmost,2 for rightmost):
>8
Invalid move!

Enter player 1 move (1 for leftmost,2 for rightmost):
>1

Boxes:
8 3
Player 1 score:6
Player 2 score:17
Enter player 2 move (1 for leftmost,2 for rightmost):
>2

Boxes:
8
Player 1 score:6
Player 2 score:20
Enter player 1 move (1 for leftmost,2 for rightmost):
>1
Player 1 score:14
Player 2 score:20
Player 2 won!
```

## Task 2 (%40 of the total points):

In addition to Task 1, improve your program so that it will allow the players to undo their moves. The player will enter 1 for left, 2 for right, 3 for undo. Otherwise the program will tell the move is invalid and ask the same player to make the move again.

If the player enters 3 you need to go back the previous state. You need to cancel the last move, update the scores and update the turn accordingly. If there are no moves for undo, in other words if you reached the beginning of the game, there won’t be any changes when user enters 3.

**Sample Input and Output:**
('>' indicates the user input)

```
Enter the number of boxes:
>5
Enter pennies in each box:
>1 5 8 3 17

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>1

Boxes:
5 8 3 17
Player 1 score:1
Player 2 score:0
Enter player 2 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>5
Invalid move!

Enter player 1 move (1 for leftmost,2 for rightmost):
>6
Invalid move!

Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>1

Boxes:
5 8 3 17
Player 1 score:1
Player 2 score:0
Enter player 2 move (1 for leftmost,2 for rightmost):
>1

Boxes:
8 3 17
Player 1 score:1
Player 2 score:5
Enter player 1 move (1 for leftmost,2 for rightmost):
>2

Boxes:
8 3
Player 1 score:18
Player 2 score:5
Enter player 2 move (1 for leftmost,2 for rightmost):
>1

Boxes:
3
Player 1 score:18
Player 2 score:13
Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
8 3
Player 1 score:18
Player 2 score:5
Enter player 2 move (1 for leftmost,2 for rightmost):
>3

Boxes:
8 3 17
Player 1 score:1
Player 2 score:5
Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
5 8 3 17
Player 1 score:1
Player 2 score:0
Enter player 2 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>1

Boxes:
5 8 3 17
Player 1 score:1
Player 2 score:0
Enter player 2 move (1 for leftmost,2 for rightmost):
>1

Boxes:
8 3 17
Player 1 score:1
Player 2 score:5
Enter player 1 move (1 for leftmost,2 for rightmost):
>2

Boxes:
8 3
Player 1 score:18
Player 2 score:5
Enter player 2 move (1 for leftmost,2 for rightmost):
>2

Boxes:
8
Player 1 score:18
Player 2 score:8
Enter player 1 move (1 for leftmost,2 for rightmost):
>2
Player 1 score:26
Player 2 score:8
Player 1 won!
```


