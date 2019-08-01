
###### Nested Loops
---

Solution 2: Now, we will use nested loops instead. Using nested loops, we just
need to make a loop for 10s digit from 5 down to 1, and for each decrement in 10s
digit, we make an inner loop for Is digit from 0 to 5.

```python
for number in range (10, 56):
    if number % 10 <= 5:
        print(number)
```

Solution 2: Now, we will use nested loops instead- Using nested loops, we just
need to make a loop for 10s digit from 1 to 5, and for each increment in 10s digit,
we make an inner loop for Is digit from 0 to 5.

```python
for tens in range (1, 6):
    for ones in range (6):
        print(tens, end = " ")
        print(ones)
```

The second code seems easier to think than the first one. The first code uses an
indirect way to solve the problem, whereas in the second code the solution method
is obvious.

A Better Example: Write a program which prints all two-digit numbers that can
be composed of {0, 1,2,3, 4, 5} in the following order:

```python
            50 51 52 53 54 55 40 41 42 43 44 45 ... 10 11 12 13 14 15
```

Be careful that Is digit increases while 10s digit decreases.


Solution 1: The solution is much harder than the previous one. We have to create
a formula to do that. We will again start from 10 and go up to 55. However, this
time we will write ‘``6 - tens digit``’ and Is digit together so the 10s digit
decreases while Is digit increases.

```python
for number in range (10, 56):
    if number % 10 <= 5:
        print(6 - int(number / 10), end = nn)
        print(number % 10)
```

<br>

<center> - 56 - </center>
