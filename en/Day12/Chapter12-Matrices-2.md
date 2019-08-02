###### Programming with Python
---

Example 12.1: Read two integers n and m then a matrix of size («, m) from the
input. Square the values in each position and output it. The size of the matrix will
not be more than (100, 100).

```
Sample input:               Sample output:
3 4                         1 4 4 1
1 2 2 1                     16 25 25 9
4 5 5 3                     4 9 25 9
2 3 5 3
```

Solution:

```python
n, m = input().split()
n = int(n)
m = int(m)
matrix = [[]]*n              # create an empty matrix with n rows

# read the matrix from the input
for row in range (n):
    matrix(row) = input().split()            # read the first row
    # convert each element in the row to integer
    for col in range(m):
        matrix[row][col] = int(matrix[row][col])

# write matrix to the output
for row in range (n):
       for col in range (in):
            print(matrix[row][col]*matrix[row][col], end="")
    print("")

```

Example 12.2: Read two integers n and m then a matrix of size («, m) from the
input. Horizontally flip the matrix and output it. The size of the matrix will not be more than (100, 100).

```
Sample input:               Sample output:
3 4                         1 2 2 1
1 2 2 1                     3 5 5 4
4 5 5 3                     3 5 5 2
2 3 5 3
```


Solution:
```python
n, m = input().split ()
n = int(n)
m = int(m)

matrix = [[]]*n            # create an empty matrix with n cows

# read the matrix from the intpu
for row in range(n):
    matrix(row) = input().split() # read the first row
    # convert each element in the row to integer
    for col in range(m):
        matrix[row][col] = int(matrix[row][col])

# make flip operation
for cow in range (nl :
    for col in range(int(m / 2)):
        temp = matrix[row][col]
        matrix(row)[col] = matrix(row)[m - col - 1]
        matrix(row)[m - col - 1] = temp

# write matrix to the output
for row in range (n):
    for col in range (in):
        print(matrix[row][col], end = "")
    print("")
```


<br>

<center> - 92 - </center>