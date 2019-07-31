###### Programming with Python
---

Consider the conditional statement below:


    If x is greater than 5 or less than 10, write ‘x is less than 4’ else write ‘x is greater than 15’.


Example 3.4: Write a program that reads a number from the keyboard and writes ‘x is less than 4’ if the given number is greater than 5 or less than 10. Otherwise it writes ‘x is greater than 15’.

```python
x = int(input())  # read x from keyboard

if x > 5 or x < ID:  # if x is greater than 5 or less than 10
    print("x is less than 4")
else:
    print("x is greater than 15")
```

Exercise 3.4: Write a program that reads a number from the keyboard and writes
‘I liked it’ if the given number is greater than 10 and not equal to 15. Otherwise it writes ‘I didn’t like it’.

Exercise 3.5: In the following program, to see “x is greater than 15” on the screen
what number the user has to enter?

```python
x = int(input())
if x == 5 or x < 10:
    print("x is less than 4")
else:
    print("x is greater than 15")
```

You can also have more than one expression in case of the condition is **true** or
**false**.

Example 3.5: Suppose that given a number x, we will write ‘small’ and multiply
x by 2 if x is less than 10. Otherwise, write ‘large’ on the screen and divide x by
2.


```python
if x < 10:
    print("small")
    x = x * 2
else:
    print ("large")
    x = x / 2
```

Here, we write the block of expressions in indented form as indicated before.

<br>

<center> - 24 - </center>

