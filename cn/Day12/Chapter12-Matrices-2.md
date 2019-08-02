###### 用Python编程
---

例12.1：读取两个整数n和m，然后读取一个大小为(n，m)的矩阵输入。将每个位置的值平方并输出。矩阵的大小将不超过(100, 100)。

```
样本输入：                  样本输出：
3 4                         1 4 4 1
1 2 2 1                     16 25 25 9
4 5 5 3                     4 9 25 9
2 3 5 3
```

解决方案：

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

例12.2：读取两个整数n和m，然后读取一个大小为(n, m)的矩阵输入。水平翻转矩阵并输出。矩阵的大小不会超过(100,100)。

```
样本输入:                    样本输出:
3 4                         1 2 2 1
1 2 2 1                     3 5 5 4
4 5 5 3                     3 5 5 2
2 3 5 3
```

解决方案：

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


