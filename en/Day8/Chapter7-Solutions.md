## Chapter 7: Solutions - Part 1

**QueQuestion 1: Example 7.1**

```python
for number in range(10, 56):
    if number % 10 <= 5:
        print(number)
```

Alternative solution:

```python
# generate ones and tens digits separately
# then print them
for tens in range (1,6):
    for ones in range (6):
        print(tens, end = "")
        print(ones)
```

**Question 2: Example 7.1: A Better Example**

```python
for number in range(10, 56):
    if number % 10 <= 5:
        print(6 - int(number / 10), end = "")
        print(number % 10)
```

Alternative solution:

```python
# generate ones and tens digits seperately then print them
for tens in range(5J 0, -1):
    for ones in range(6):
        print(tens, end = "")
        print(ones)
```

**Question 3: Exercise 7.1**

```python
# generate ones and tens digits separately
# then print them
for tens in range(1 > 7):
    for ones in range (1,6,2):
        print(tens, end = "")
        print(ones)
```


**Question 4: Exercise 7.2\***

```python
# try all numbers from 10 to 66
for number in range (10, 67):
    # only print the odd numbers
    # that has 6 or less in ones digit
    if number % 10 <= 6 and number % 2 == 1:
        print(number)
```

**Question 5: Exercise 7.3**

```python
# generate ones, tens and hundreds digits separately
# then print them
for hundreds in range(1 , 5):
    for tens in range(5):
        for ones in range(5):
            print(hundreds, end="")
            print(tens, end="")
            print(ones)
```

**Question 6: Exercise 7.5**

```python
n, m = input().split()
n = int (n)
m = int (m)
# row keeps the current row
for row in range (1, n + 1):
    # in each line print the row number m times
    for col in range(m):
        print(row,end="")
    print()
```

**Question 7: Exercise 7.7**

```python
n = int (input())
# row keeps the current row
for row in range (1,n+l):
    # col keeps the current column
    # output the column number in each position
    for col in ranged row+1):
        print(col, end:"")
    print()
```

**Question 8: Exercise 7.9**

```python
n = int (input())
numbers = input().split()
for i in range(n):
    numbers[i] = int (numbers[i])
    stars = numbers[i]
    # output stars in one row
    for j in range(stars):
        print('*',end="")
    print() # press enter
```

**Question 9: Exercise 7.10**

```python
n = int (input())
numbers = input().split() # save the numbers to an array
for i in range(n):
    numbers[i] = int (numbers[i])
# count each number from 1 to 1000 in the array
for i in range(l,1001):
    # count the number i in the array
    cnt = 0
    for j in range(n):
        if numbers[j]==i :
            cnt+=l
    # if it’s more than one, output it
    if cnt > 1:
        print(i)
```
