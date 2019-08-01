**Question 1：Exercise 4.20\*\***

```python
x = int(input())
if (x == 0):
    print(0)
# write the number backwards
while (x > 0):
    # write ones digit on screen
    print(x % 10 , end = "")
    # get rid of ones digit
    x = int(x / 10)
```
<br>

**Question 2：Exercise 4.21\*\***

```python
n = int(input())
m = int(input())
row = 1
col = 1
while row <= n:
# write row number on screen
print(row, end="")
# increase the column
col = col + 1
# if finished the column 
if col > m :
    col = 1;            # reset column
    row = row + 1       # increase row
    print()             # go to the next line
```
<br>

**Question 3：Exercise 4.22\*\***

```python
n = int(input())
row = 1
col = 1
while row <= n :
# write column number on screen
print(col, end=" •’）
# increase the column
col = col + 1
# if finished the column
if col > row :
    col = 1             # reset column
    row = row + 1       # increase row
    print ()            # go to the next line
```
<br>

**Question 4：Exercise 4.23\*\*\***

```python
n = int(input())
row = 1
col = 1
while row <= n :
    if col == 1 :
        m = int(input())
    if col != 1 :
        print( e n d = •_，.)
# increase the column
col = col + 1
# if finished the column
if col > m + 1 :
    col = 1           # reset column
    row = row +       # reset column
    print()           # go to the next line
```

<br>

**Question 5：Exercise 4.24\*\*\***

```python
n = int(input())
m = int(input())
row = 1
col = 1
while row <= n :
print(col + row - 1, end = " " )
# increase the column
col = col + 1
# if finished the column
if col > m :
    col =1              # reset column
    row = row + 1       # reset column
    print()             # go to the next line
```
<br>

**Question 6：Exercise 4.25\*\*\***

```python
""" 
    a is a number from 2 to n
    b is for checking if "a" is a prime number or not
    b is a number from 2 to square root of "a"
    prime is 1 if "a" is prime and 0 otherwise
    initially "a" is assumed to be prime
"""

n = int(input())
a = 2
b = 2
prime = 1

while a < n:
    # whenever b reaches the square root of a
    # and a is prime, output a
    if b*b > a and prime == 1:
        print(a, end = " ")

    # whenever b more than the square root of a
    if b * b > a :
        b = 2               # reset b
        a = a + 1           # start checking the next number
        prime = 1           # reset prime to 1
    # if a is divible by b
    if a % b == 0 :
        prime = 0;          # a is not prime
```


