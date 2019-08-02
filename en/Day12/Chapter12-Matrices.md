###### Matrices
---

# <center>Chapter 12: Matrices</center>
---


## 12.1. Introduction

When we go to a post office we see mail boxes lined up in rows and columns.
Each mail box has mails in it and is referred with a number. The mail boxes can
also be referred without using these numbers on them. If we refer to a row and a
column it will correspond to a mail box. If we ask our friend to find the mail box at the 3rd row and the 5,h column, he or she will easily locate it. Just like the mail boxes in a post office, a matrix is composed of boxes which are referred by the row and the column numbers.

![](http://legendary.cdn.play8.io/learnpython/img/day12/d12-p1.png)

The matrix A above has 3 rows and 4 columns, so it has 12 boxes with numbers in them. In the matrix above, the referred position is row 1, column 2.

> [!NOTE]
> Notice that just like as in arrays, the indices start from 0.

We can define and initialize a matrix as follows:

```python
myMatrix = [0] * n
for i in range (n):
    myMatrix[i] = [0] * m
```

defines a matrix called 'myMatrix' with 3 rows and 4 columns. It is similar to the arrays; in addition matrices have two dimensional hence we need to add one more bracket when defining. The above code initializes the matrix with zeros.

We can read from and write to the matrix locations in the same way we do in arrays. For instance,

```python
print(myMatrix[1][2])
```

outputs the value at position (1,2) - row 1, column 2 - whereas,

```python
myMatrix [l] [2] = 100
```

puts the value ‘ 100’ in the same location.


<br>

<center> - 91 - </center>