## Toads and Frogs

Write the following toads and frogs game.

Toads and frogs is a one player game. Given a board of size N (where N is odd), left side of the board is filled with toads and right side is with frogs and the middle square is empty. Here is the initial board configuration for N=7: 

```TTT-FFF```

'T': toad, 'F': frog, '-': empty

A toad can slide right or jump over one square to the right. Similarly, a frog can slide left or jump over one square to the left. The objective of the game is to move the toads to the right side and frogs to the left side of the board in minimum number of moves. The final configuration should be as follows: 

```FFF-TTT```

##### Game design:

1. The player will enter the board size N. N is an odd number (3 <= N <= 21). Then you will setup the board with respect to N.
2. In each turn, print the current board and number of moves on screen.
3. Then the program waits for the player input, a number between 1 to N. The number indicates to move the element in that square.
- Example: 3 moves the toad at position 3 to position 4.
- Example: 6 moves the frog at position 6 to the position 4.

4. Continue asking the player move if the provided move is not valid. Otherwise make the move.

5. The game finishes whenever all frogs are on the left side and all toads are on the right side and the empty square is in the middle.

**Sample Input and Output for N=5:**
('>' indicates the user input)

```
>5

TT-FF
>4

TTF-F
Number of moves:
1

>2

T-FTF
Number of moves:
2

>1

-TFTF
Number of moves:
3

>3

FT-TF
Number of moves:
4

>3
Invalid entry!

>5

FTFT-
Number of moves:
5

>4

FTF-T
Number of moves:
6

>2

F-FTT
Number of moves:
7

>3

FF-TT
Number of moves:
8

You win!
```

#### Task 1 (%40 of the total points):

The board size N will be always be 7.

#### Task 2 (%40 of the total points):
The board size N can change (N is an odd number)

#### Task 3 (%20 of the total points):
In addition to Task 2, add the undo move option; '0' means undo. The player should be able to undo till the beginning of the game.

**Sample Input and Output**
('>' indicates the user input)

```
>15

TTTTTTT-FFFFFFF
>7

TTTTTT-TFFFFFFF
Number of moves:
1

:  :  :
:  :  :

TTTTFT-TFTFFFFF
Number of moves:
7

>9

TTTTFTFT-TFFFFF
Number of moves:
8

>0

TTTTFT-TFTFFFFF
Number of moves:
7

:  :  :
:  :  :

FFFFFFFT-TTTTTT
Number of moves:
62

>8

FFFFFFF-TTTTTTT
Number of moves:
63

You win!
```
