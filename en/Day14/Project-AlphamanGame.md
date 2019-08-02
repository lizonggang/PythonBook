## AlphaMan Game

Write the following AlphaMan game.

**Game design:**

AlphaMan is a one player game. Given a maze, AlphaMan’s position and the exit location, player leads AlphaMan to the exit.

N  (number of rows) and M  (number of columns) will be given (4<=N,M<=20). The maze with contain following characters:

- “#” is for wall
- ‘.’  is for empty spots
- ‘A’ is for AlphaMan’s location
- ‘E’ is for exit
- ‘G’ is for gems
- ‘M’ is for monsters
- In each turn, print the current maze on screen. Then the program waits for the player input. Input will be lower case:

‘a’ : left
‘w’ : up
‘s’ : down
‘d’ : right
Continue asking the player move if the provided move is not valid. Otherwise make the move.

If you hit the wall print below message:

```
Ouch! You hit the wall!
```

The game finishes whenever AlphaMan reaches to the exit. Print ending message:

```
Congrats, you finished!!! 
```

### Task 1 (%60 of the total points):

Design the game described above. There will be no monsters and no gems in this task.

**Sample Input and Output:**
('>' indicates the user input)

```
>5
>6
>######
>#.##E#
>##...#
>#A.#.#
>######

######
#.##E#
##...#
#A.#.#
######
>d

######
#.##E#
##...#
#.A#.#
######
>d
Ouch! You hit the wall!

######
#.##E#
##...#
#.A#.#
######
>w

######
#.##E#
##A..#
#..#.#
######
>w
Ouch! You hit the wall!

######
#.##E#
##A..#
#..#.#
######
>d

######
#.##E#
##.A.#
#..#.#
######
>d

######
#.##E#
##..A#
#..#.#
######
>w
Congrats, you finished!!!
```

#### Task 2 (%20 of the total points):

In addition to Task1 this time there will be at least 1 gem in the maze. The player needs to collect all gems in order to be able to finish the game. If the player reaches exit before collecting all gems print below message and continue the game:

```
You first have to collect all the gems!
```

(Make sure you leave an empty line after this message)

#### Task 3 (%20 of the total points):

In addition to Task 2 this time there will be at least 1 monster in the maze. If the player touches the monster the game ends immediately with the following message:

```
Monster ate you!!!
```

