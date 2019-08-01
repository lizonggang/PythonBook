## Alpha Maria Game

Alpha Maria is a one player game. A two line platform will be provided on screen.
![](http://legendary.cdn.play8.io/learnpython/img/day7/p1.png)



The player uses the following keys to move: 1 - left one square, 2 - right one square, 3 - jump two squares to left, 4 - jump two squares to right.

**Example for right jump:**
Before&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;After
![](http://legendary.cdn.play8.io/learnpython/img/day7/p2.png)

Alpha Maria gets 100 points if she collects a mushroom. The game ends whenever Alpha Maria reaches the exit. Write the Alpha Maria game described above.

**Game design:**

N  (the length of the platform) will be given (4 <= N <= 80). The platform will contain the following numbers: 
  - 0: empty spots, 
  - 1: Alpha Maria, 
  - 2: mushroom, 
  - 3: wall, 
  - 4: exit.

The sample platform above will be provided as follows:

```
20
0 0 0 0 2 0 0 0 0 0 0 0 2 0 3 0 0 3 0 0
0 1 2 0 3 0 2 0 3 0 4 0 3 0 0 3 0 2 0 0
```

In each turn, print the current score and the platform on screen. Then the program waits for the player input (1, 2, 3, or 4) and makes the move. The game finishes whenever Alpha Maria reaches to the exit. Print ending message:

```
Congrats, you finished!!!
```

### Task 1 (%60 of the total points):

esign the game described above.

**Sample Input and Output:**
('>' indicates the user input)

```
>20
>0 0 0 0 2 0 0 0 0 0 0 0 2 0 0 0 0 0 0 0
>0 1 2 0 3 0 2 0 3 0 4 0 3 0 0 3 0 2 0 0
Score: 0
00002000000020000000
01203020304030030200
>4
Score: 0
00002000000020000000
00213020304030030200
>4
Score: 100
00000000000020000000
00203120304030030200
>2
Score: 200
00000000000020000000
00203010304030030200
>2
Score: 200
00000000000020000000
00203001304030030200
>4
Score: 200
00000000000020000000
00203000314030030200
>4
Score: 200
00000000000020000000
00203000304130030200
>1
Congrats, you finished!!!
```

### Task 2 (%20 of the total points):

Check if the move is valid. Alpha Maria can’t go through the walls. Whenever Alpha Maria hits a wall or tries to go outside the platform, print the message below:

```
Ouch! You hit the wall!
```

It’s guaranteed that there won’t be any walls on the top line of the platform.

### Task 3 (%20 of the total points):

Top line of the platform can have walls.

