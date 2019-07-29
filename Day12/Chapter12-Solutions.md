**问题1: 练习12.1**

```python
n, m = input().split()
n = int(n)
m = int(m)
matrix = [[]]*n # create an empty matrix with n rows
#  read the matrix from the input
for row in range(n):
    matrix[row] = input().split() # read the first row
    # convert each element in the row to integer
    for col in range(m):
        matrix[row][col] = int(matrix[row][col])

#  write matrix to the output
for row in range(n):
    for col in range(m):
        print(matrix[row][col]*matrix[row][col], end=" ")
    print("")
```

<br>

**问题2: 练习12.2**

```python
n, m = input().split()
n = int(n)
m = int(m)
matrix = [[]]*n # create an empty matrix with n rows
#  read the matrix from the input
for row in range(n):
    matrix[row] = input().split() # read the first row
    #  convert each element in the row to integer
    for col in range(m):
        matrix[row][col] = int(matrix[row][col])

#  make flip operation
for row in range(n):
    for col in range(int(m / 2)):
        temp = matrix[row][col]
        matrix[row][col] = matrix[row][m - col - 1]
        matrix[row][m - col - 1] = tmep

# write matrix to the output
for row in range(n):
    for col in range(m):
        print(matrix[row][col], end = " ")
    print("")
```

<br>

**问题3: 练习 12.1**

```python
n, m = input().split()
n = int(n)
m = int(m)
matrix = [[]]*n # create an empty matrix with n rows
#  read the matrix from the input
for row in range(n):
    matrix[row] = input().split() # read the first row
    #  convert each element in the row to integer
    for col in range(m):
        matrixfrow][col] = int(matrix[row][col])

#  make flip operation
for row in range(int(n/2)) :
    for col in range(m) :
        temp = matrixfrow][col]
        matrix[row][col] = matrix[n-row-l][col]
        matrix[n-row-l][col] = temp

#  write matrix to the output
for row in range(n):
    for col in range(m):
        print(matrix[row][col], end=" ")
    print("")
```

<br>

**问题4: Exercise 12.2**

```python
n, m = input().split()
n = int(n)
m = int(m)
matrix1 = [[]]*n # create empty matrix1 with n rows
#  read matrix1 from the input
for row in range(n):
    matrix1[row] = input().split() # read the first row
    #  convert each element in the row to integer
    for col in range(m):
        matrix1[row][col] = int(matrix1[row][col])

emptyline = input() #There is a space between matrix1 and matrix2

matrix2 = [[]]*n # create empty matrix2 with n rows
#  read matrix2 from the input
for row in range(n):
    matrix2[row] = input().split() # read the first row
    #  convert each element in the row to integer
    for col in range(m):
        matrix2[row][col] = int(matrix2[row][col])

#  write summation matrix to the output
for row in range(n):
    for col in range(m):
    print(matrix1[row][col]+matrix2[row][col], end=" ")
    print("")
```


<br>

**问题5: Exercise 12.3***

```python
n = input()
n = int(n)

matrix1 = [[]]*n # create empty matrix1 with n rows
#  read the matrix1 from the input
for row in range(n):
    matrix1[row] = input().split() # read the first row
    #  convert each element in the row to integer
    for col in range(n):
        matrix1[row][col][row][col] = int(matrix1[row][col])

matrix2 = [[0]*n for i in range(n)] # create empty matrix2 with n rows and n columns


"""
Be careful, shortening this to something like
n*[n*[0]] doesn't really work because you end up with
n copies of the same list,
so when you modify one of them they all change
"""


#  make "rotate 90 degrees clockwise" operation and save it to matrix2
for row in range(n) :
    for col in range(n) :
        matrix2[col][n-row-1] = matrix1[row][col]
#  write matrix2 to the output
for row in range(n):
    for col in range(n):
        print(matrix2[row][col], end=" ")
    print("")
```


<br>

**问题6: Exercise 12.4***

```python
n, m = input().split()
n = int(n)
m = int(m)
maze = [[0 for j in range(m)] for i in range(n)] # create empty matrix2 with n rows and m columns
for row in range(n):
    maze[row] - input().split() # read the first row
    # convert each element in the row to integer
    for col in range(m):
        maze[row][col] = int(maze[row][col])
emptyline = input() #There is a space between maze and path
path = input()
#  (r,c) is the loca问题in the maze
#  valid: stores the validity of the path
r=l
c=l
valid=l
#  walk through the path
for ch in path:
    # update the loca问题in the maze  
    if ch==’u' : r-=l                 
    if ch=='d' : r+=l                 
    if ch==’l’ : c-=l                 
    if ch=='r' : c+=l                 
    # check if reached the exit        
    if r==l and  c==m-l :             
        # if still remaining path
        if ch!=path[len(path)-l] :
            valid=0
        break
        # it’s invalid path if hits to wall
        if maze[r][c]==1:
            valid=0
            break
# the path has to finish at (1,m-1) without hitting any walls
if valid==0 or r!=l or cl=m-1:
    print("Wrong pathl")
else :
    print("Right path!")
```


<br>

**问题7: Exercise 12.6\*\***

```python
# draw a spiral of size n x n # we will draw the spiral in canvas matrix
n = int(input())

# create and reset the canvas matrix n’n
canvas = [(0 for j in range(n)] for i in range(n)]
# 0 i:- empty ; is star

#   draw the spiral # the pattern is
#   1) N - on the top row
#   2) continues :#ith two N-l ’"’s
#   3) then length of '** reduces by 2
#   4) drawing continues until length is 2 if N is odd
#        or length is 1 if N is even

#   draw the top bar
for i in range(n):
    canvas(0][i)=l

# dir: direction, len: length of the itraight drawing,
# (r,c): row and column while drawing
dir = 0
len = n-l
r = 0
c = 0
while len>0 :
    for j in range(len):
        9 move on the direction
        if dir == 0 :
            r+=l # down
        if dir == 1 :
            c+sl # right
        if dir == 2 :
            r-=l # up
        if dir == 3 :
            c-=l # left
        canvas(r][c] = 1
    # if N is odd, draw only one '*' with length 1
    if len == 1:
        break
    dir = (dir + 1) % 4         # update direction
        # if the drawing is in the even step
    if dir % 2 == 0:
        # reduce the length of straight drawing
        len-=2
#write canvas to the output
for row in range(n):
    for col in range(n):
        if canvas[row][col] == 1:
            print("B", end="")
        else :
            print(" ", end="")
    print("")
```

