# Matchstick Game
(Matchstick Game - Human vs Human)

Write the following matchstick game.

Matchstick is a two player game. There are N matches on the table initially. In each turn, current player picks 1, 2, or 3 matches from the table. The player who picks the last match on the table wins the game.

The game proceeds as follows:

1. The boss enters the number of matches, N where (1<=N<=100)
2. The boss enters an integer D. If D is 1, you need to draw the matches on screen with characters | (bar) and * (asteriks) -- see the example below. If it is 0, you will not draw them on screen.
3. Program asks the current player to pick 1, 2, or 3 matches.
4. Player enters a number. The number of matches that the player picked are removed from the table.
5. The other player takes the turn and the game continues until there are no matches left on the table.  
6. Whoever picks the last matchstick on the table, wins the game.

## Task 1 (%40 of the total points):
Read an integer number N.
Read the value of D. For Task 1, It is guaranteed that the value will be 0 so you don’t need to draw the matches on screen in this task.
Continuously read values from each player and show the current player and the number of remaining matches on screen. It is guaranteed that there will be no invalid input. For example, the players will not enter 5 to pick 5 matches.
Finish the game when there are no more matches on the screen. Show the winner on screen.
Note that the input and output format has to be exactly as in the following example.

Sample Input and Output:
('>' indicates the user input)

```python
Enter the number of matches:
>9
Enter draw value 1 for draw, 0 for not draw:
>0
Number of remaining matches: 9
Player 1: How many matches do you want to pick? (1,2 or 3)
>2
Number of remaining matches: 7
Player 2: How many matches do you want to pick? (1,2 or 3)
>3
Number of remaining matches: 4
Player 1: How many matches do you want to pick? (1,2 or 3)
>3
Number of remaining matches: 1
Player 2: How many matches do you want to pick? (1,2 or 3)
>1
Player 2 won the game!
```

## Task 2 (%40 of the total points):
In addition to Task 1, this time it is not guaranteed that the players will enter valid entries. You need to check the validity of player inputs. Remember normally the moves can be either 1 or 2 or 3. Also keep in mind that if there are only 2 matches left and the player enters 3, that’s an invalid move.


Example:

```python
>7
Enter draw value 1 for draw, 0 for not draw:
>0
Number of remaining matches: 7
Player 1: How many matches do you want to pick? (1,2 or 3)
>1
Number of remaining matches: 6
Player 2: How many matches do you want to pick? (1,2 or 3)
>4
Invalid move!
You can pick 1, 2 or 3 matches.
Number of remaining matches: 6
Player 2: How many matches do you want to pick? (1,2 or 3)
>0
Invalid move!
You can pick 1, 2 or 3 matches.
Number of remaining matches: 6
Player 2: How many matches do you want to pick? (1,2 or 3)
>3
Number of remaining matches: 3
Player 1: How many matches do you want to pick? (1,2 or 3)
>1
Number of remaining matches: 2
Player 2: How many matches do you want to pick? (1,2 or 3)
>3
Invalid move!
You can pick 1, 2 or 3 matches.
Number of remaining matches: 2
Player 2: How many matches do you want to pick? (1,2 or 3)
>1
Number of remaining matches: 1
Player 1: How many matches do you want to pick? (1,2 or 3)
2
Invalid move!
You can pick 1, 2 or 3 matches.
Number of remaining matches: 1
Player 1: How many matches do you want to pick? (1,2 or 3)
1
Player 1 won the game!
```

## Task 3 (%20 of the total points):
In addition to Task 2, you need to draw the matchsticks on screen.

**Example:**

```python
Enter the number of matches:
>6
Enter draw value 1 for draw, 0 for not draw:
>1
Number of remaining matches: 6
* * * * * *
| | | | | |
| | | | | |
| | | | | |
| | | | | |
Player 1: How many matches do you want to pick? (1,2 or 3)
>4
Invalid move!
You can pick 1, 2 or 3 matches.
Number of remaining matches: 6
* * * * * *
| | | | | |
| | | | | |
| | | | | |
| | | | | |
Player 1: How many matches do you want to pick? (1,2 or 3)
>2
Number of remaining matches: 4
* * * *
| | | |
| | | |
| | | |
| | | |
Player 2: How many matches do you want to pick? (1,2 or 3)
>3
Number of remaining matches: 1
*
|
|
|
|
Player 1: How many matches do you want to pick? (1,2 or 3)
>1
Player 1 won the game!
```


---



# Matchstick Game

Write the matchstick game that plays with a human player. The computer will be the first player.

Matchstick is a two player game. There are N matches on the table initially. In each turn, current player picks 1, 2, 3, ...M  matches from the table. The player who picks the last match on the table wins the game.

The game proceeds as follows:

1. The boss enters the number of matches, N (1<=N<=100).
2. The boss also enters M; the number of maximum matches that a player can pick  (M<=N).
3. Program asks to the current player to pick the number matches (1, 2, 3.. M).
4. Player enters a number. The number of matches that the player picked are removed from the table.
5. The other player takes the turn and the game continues until there are no matches left on the table.  
6. Whoever picks the last matchstick on the table, wins the game.

## Task 1 (%60 of the total points):
- Read an integer number N.
- Read an integer M. It is guaranteed that M will be always 3 for this task.
- Continuously read values for each player and show the current player and remaining number of matches on the screen.
- It is not guaranteed that the players will enter valid entries. You need to check validity of player inputs. Remember normally the moves can be either 1 or 2 or 3 if M=3. Also keep in mind that if there are only 2 matches left and the player enters 3, that’s an invalid move.
- Finish the game when there is no more matches on the screen. Show the winner on the screen
Note that the input and output format has to be exactly as in the following example.

**Sample Input and Output:**
('>' indicates the user input)

```python
Enter the number of matches:
>10
Enter the maximum amount that a player can pick:
>3
Number of remaining matches: 10
Player 1: How many matches do you want to pick? (1..3)
2
Number of remaining matches: 8
Player 2: How many matches do you want to pick? (1..3)
>5
Invalid move!
You can pick 1..3 matches.
Number of remaining matches: 8
Player 2: How many matches do you want to pick? (1..3)
>0
Invalid move!
You can pick 1..3 matches.
Number of remaining matches: 8
Player 2: How many matches do you want to pick? (1..3)
>2
Number of remaining matches: 6
Player 1: How many matches do you want to pick? (1..3)
2
Number of remaining matches: 4
Player 2: How many matches do you want to pick? (1..3)
>3
Number of remaining matches: 1
Player 1: How many matches do you want to pick? (1..3)
1
Player 1 won the game!
```

## Task 2 (%40 of the total points):
In addition to Task 1, this time M may be different than 3 (1<=M<=N). You need to check the validity accordingly. The computer will be first player. N and M will be given in such a way that computer always wins if plays optimally. Implement the best strategy for computer.

**Example:**


```python
Enter the number of matches:
>14
Enter the maximum amount that a player can pick:
>5
Number of remaining matches: 14
Player 1: How many matches do you want to pick? (1..5)
2
Number of remaining matches: 12
Player 2: How many matches do you want to pick? (1..5)
>9
Invalid move!
You can pick 1..5 matches.
Number of remaining matches: 12
Player 2: How many matches do you want to pick? (1..5)
>1
Number of remaining matches: 11
Player 1: How many matches do you want to pick? (1..5)
5
Number of remaining matches: 6
Player 2: How many matches do you want to pick? (1..5)
>2
Number of remaining matches: 4
Player 1: How many matches do you want to pick? (1..5)
4
Player 1 won the game!
```





























---




