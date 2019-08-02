**Question 1**

从键盘读取两个整数n和m，然后读取一个大小为(n，m)的矩阵。 将每个位置的值平方并将其写入输出。 矩阵的大小不会超过(100,100)。

**For example:**

```
Input                   Result
3 4                     1 4 4 1
1 2 2 1                 16 25 25 9
4 5 5 3                 4 9 25 9
2 3 5 3
```

**Question 2**

Read two integers n and m then a matrix of size (n, m) from the input. Horizontally flip the matrix and write it to output. The size of the matrix will not be more than (100, 100).

**For example:**


**For example:**

```
Input                   Result
3 4                     1 2 2 1
1 2 2 1                 3 5 5 4
4 5 5 3                 3 5 3 2
2 3 5 3
```

**Question 3**

Read two integers n and m then a matrix of size (n, m) from the input. Vertically flip the matrix and write it to output. The size of the matrix will not be more than (100, 100).

**For example:**

```
Input                   Result
3 4                     2 3 5 3
1 2 2 1                 4 5 5 3
4 5 5 3                 1 2 2 1
2 3 5 3
```

**Question 4**

Read an integer n and m then two matrices of size (n, m) from the input. Add the values at the same positions of these matrices, and write the summation matrix to output. The size of the matrices will not be more than (100, 100).

**For example:**

```
Input                   Result
3 4                     10 10 9 7
1 2 2 1                 5 5 9 2
4 5 5 3                 5 6 8 6
2 3 5 3

9 8 7 6
1 0 4 -1
3 3 3 3
```

**Question 5**

Read an integer n then a matrix of size (n, n) from the input. Flip the matrix 90 degrees clockwise and write it to output. The size of the matrix will not be more than (100, 100).

**For example:**

```
Input                   Result
4                       9 2 4 1
1 2 2 1                 8 3 5 2
4 5 5 3                 7 5 5 2
2 3 5 3                 6 3 3 1
9 8 7 6
```

**Question 6**

You will be given a map of a maze and a path. Check if the path is a correct way to the exit. You will start at position (1, 1), and exit is at (1, m - 1). An example maze of size (7, 6) is given below. Starting and exit locations are shown as 'S' and 'E'. A path is shown with red color to the exit.

![](http://legendary.cdn.play8.io/learnpython/img/day12/d12-p2.png)


You will first read the size of the maze (n, m). Then the maze will be given; 1's are walls, 0's are empty locations. The size of the maze will not be more than (100, 100). The path is given as a string composed of four different letters; 'l' means left, 'r' means right, 'u' means 'up', and 'd' means 'down'.

You will write 'Right path!' if the path leads to the exit from the starting location, otherwise write 'Wrong path!' on the screen.

**For example:**

```
Input                   Result
7 6                     Right path!
1 1 1 1 1 1 
1 0 1 0 0 0 
1 0 1 0 0 1 
1 0 0 1 0 1 
1 1 0 0 0 1 
1 0 0 1 0 1 
1 1 1 1 1 1 

ddrdrruulurr
```


**Question 7**

Write a program that reads a number n <= 20 from the keyboard and prints the spiral of asterisks on the screen as shown below.

**For example:**

```
Input                   Result
5                       *****
                        *     
                        * *** 
                        *   *
                        ***** 
--------------------------------
8                       ********
                        *
                        * ******
                        * *    *
                        * *  * *
                        * **** *
                        *      *
                        ********
```

