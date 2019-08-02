###### Matrices
---

You will write ‘Right path!’ if the path leads to the exit from the starting
location, otherwise write ‘wrong path! ’ on the screen.

### 12.4. Character Matrix
Example 12.3'. In exercise 4, the maze was given as an integer matrix. For
instance, we can more intuitively represent it in a character matrix; the input can be as follows:

```
Sample input:               Sample output:
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

In this representation, corresponds to walls and corresponds to empty locations. We don’t need to put space between characters. We can read the input
almost the same

```python
n, m = input().split()
n = int(n)
m = int(m)
maze = [[]]*n # create an mepty maze with n rows.

# read the maze from the input
fro row in range(m):
    maze[row] = list(input()) # read the row and convert to a array
path = input()
```


We can also use matrices to manipulate shapes. The following exercise
demonstrates how matrices can be used to manipulate shapes.

Exercise 12.5: write a program that reads a number n < 20 from the keyboard
□nd prints the spiral of asterisks on the screen as shown below.

```
样本 n = 5                      n = 8
*****                           ********
*                               *
* ***                           * ******
*   *                           * *    *
*****                           * *  * *
                                * **** *
                                *      *
                                ********
```

<br>

#### Congratulations - end of lesson reached

Well done!

<br>

<center> - 95 - </center>