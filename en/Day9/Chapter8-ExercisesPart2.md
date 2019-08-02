**Question 1**

Lucy wants to calculate her bonus points she earned while shopping. She knows how much she spent in her last N <= 100 shopping, and all of them are bakery, produce, or drinks. 
- If they are bakery, she earns 5 points per dollar.
- If they are produce, she earns 2 points per dollar.
- If they are drinks, she earns 1 point per dollar.

She earns bonus points when she spends more than M dollars in one shopping. You will first read N then N numbers corresponding to the money Lucy spend. At the end, you will read M then the type of shopping items. Write the total bonus points on the screen.

**For the example below: **
Lucy receives bonus points for shopping more than $50 hence $88 and $72 are qualified for bonus. Her shopping was on bakery which brings 5 points per dollar. In total, she got (88 + 72) * 5 = 800 bonus points.

**For example:**

```
Input                       Result
5                           800
41 13 88 50 72              
50 bakery
```

<br>

**Question 2**

Write a program that outputs the number of letters in a given string.

**For example:**

```
Input                       Result
I8-10caKes!                 6
```

<br>

**Question 3**

Write a program that converts all letters to uppercase in a given string.

**For example:**

```
Input                       Result
I8-10caKes!                 I8-10CAKES!
```

<br>

**Question 4**

Write a program that checks if two given strings are the same regardless of the case differences. If the strings are same, write '``same``' otherwise '``not same``' on the screen.

**For example:**

```
Input                       Result
Trivial Trival              not same
tRiViAl TrIvIaL             same
```

<br>

**Question 5**

Write a program that outputs the number of digits in a given string.

**For example:**

```
Input                       Result
I8-10caKes!                 3
```

<br>

**Question 6**

Write a program that reads two strings from the keyboard and checks if the number of vowels in these strings are equal.

**For example:**

```
Input                       Result
ThReE VoWeLs                Same number of vowels.
twO VoWeLs                  Not same number of vowels.
```

<br>

**Question 7**

Write a program that reads a number x and a character c from the keyboard. The program outputs a square with the size x filled with character c.

**For example:**

```
Input                       Result
4 #                         ####
                            ####
                            ####
                            ####
```

<br>

**Question 8**

Write a program that reads a number x and a character c from the keyboard. The program outputs an empty square with the size x and border with character c.

**For example:**

```
Input                       Result
4 #                         ####
                            #  #
                            #  #
                            ####
```

<br>

**Question 9**

You will be given a map of a maze and a path. Check if the path is a correct way to the exit. You will start at position (1, 1), and exit is at (1, m - 1). An example maze of size (7, 6) is given below. Starting and exit locations are shown as 'S' and 'E'. A path is shown with red color to the exit.

![](http://legendary.cdn.play8.io/learnpython/img/day9/p2.png)

You will first read the size of the maze (n, m). Then the maze will be given; '#'s are walls, '.'s are empty locations. The size of the maze will not be more than (20, 20). The path is given as a string composed of four different letters; 'l' means left, 'r' means right, 'u' means 'up', and 'd' means 'down'.

You will write 'Right path!' if the path leads to the exit from the starting location, otherwise write 'Wrong path!' on the screen.

**For example:**

```
Input                       Result
7 6                         Right path!
######
#.#...
#.#..#
#..#.#
##...#
#..#.#
######
ddrdrruulurr
```

