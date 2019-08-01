###### Nested Loops
---

Solution 2: Now, we will use nested loops instead. Using nested loops, we just
need to make a loop for 10s digit from 5 down to 1, and for each decrement in 10s
digit, we make an inner loop for Is digit from 0 to 5.

```python
for tens in range(5, 0, -1):
    for ones in range (6):
        print(tens, end ="")
        print(ones)
```

Compared to the first solution, the second solution is much easier to think.

Exercise 7.1: Write a program which prints all two-digit odd numbers that can be
composed of {0, 1,2, 3,4, 5, 6} using nested loops.

*Exercise 7.2: Solve the same problem without using nested loops.

Exercise 7.3: Write a program which prints all three-digit numbers that can be
composed of {0, 1,2, 3,4} using nested loops.

*Exercise 7.4: Solve the same problem without using nested loops.

Exercise 7.5: Write a program that reads two numbers N and M from the input.
Then, your program will print a figure that has N number of rows and M number
of columns. The first row will have with M number of Is, and the second row will
have M number of 2s. It will continue until the Nth row will have M number of
Ns. See the example below for clarity.

```
Sample input:
3 4
```

```
Sample output:
1111
2222
3333
```

** Exercise 7.6: Solve the same problem without using nested loops.

<br>

<center> - 57 - </center>