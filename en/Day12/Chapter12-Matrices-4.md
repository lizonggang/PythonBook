###### Programming with Python
---

### 12.2. Matrix Initialization

Matrices can be initialized while defining as in arrays:

```python
matrix = [[1, 2, 2, 1], [4, 5, 5, 3], [2, 3, 5, 3]]
```


### 12.3. Matrices as Mazes and Graphs

Matrices can be used for different purposes than just numbers such as representing
mazes and graphs.

*Exercise 12.4:

You will be given a map of a maze and a path. Check ifthe path is a correct way to the exit. You will start at position (1,1), and exit is at (1, m—1). An example maze of size (7, 6) is given below. Starting and exit locations
are shown as *S' and lE'. A path is shown with red color to the exit.

![](http://legendary.cdn.play8.io/learnpython/img/day12/d12-p2.png)


```
Sample input:               Sample output:
7 6                         Right path!
1 1 1 1 1 1
1 0 1 0 0 0
1 0 1 0 0 1
1 0 0 1 0 1
1 1 0 0 0 1
1 0 0 1 0 1
1 1 1 1 1 1
ddrdrruulurr
```

You will first read the size of the maze (n, m). Then the maze will be given as a matrix size of (n, m); 1 's are walls, 0's are empty locations. The size of the matrix will not be more than (100, 100). The path is given as a string composed of four different letters; 'l' means 'left', 'r' means 'right', 'u' means 'up', and 'd' means 'down'.

<br>

<center> - 94 - </center>