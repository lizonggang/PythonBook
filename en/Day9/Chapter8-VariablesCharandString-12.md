###### Programming with Python 
---

```
Sample input:                   Sample output:
4 #                             ####
                                ####
                                ####
                                ####
```

8.20*) Write a program that reads a numbers ``x`` and a character ``c`` from the keyboard. The program outputs an empty square with the size ``x`` and border with character ``c``.

```
Sample input:                   Sample output:
4 #                             ####
                                #  #
                                #  #
                                ####
```

8.21**)
You will be given a map of a maze and a path. Check if the path is a correct way to the exit. You will start at position (1, 1), and exit is at (1, m - 1). An example maze of size (7, 6) is given below. Starting and exit locations are shown as 'S' and 'E'. A path is shown with red color to the exit.

![](http://legendary.cdn.play8.io/learnpython/img/day9/p1.png)

 
```
Sample input:                    Sample output:
7 6                              Right path! 
######                       
#.#...
#.#..#
#..#.#
##...#
#..#.#
######   
ddrdrruulurr                                              
```


You will first read the size of the maze (n, m). Then the maze will be given; ‘#’s are walls, ‘.’s are empty locations. The size of the maze will not be more than (20, 20). The path is given as a string composed of four different letters; ‘l’ means ‘left’，‘r’ means ‘right’， u means ‘up’， and ‘d’ means ‘down’.

You will write '``Right path!``' if the path leads to the exit from the starting
location, otherwise write '``wrong path!``' on the screen.


#### Congratulations - end of lesson reached

Well done!


<br>

<center> - 72 - </center>