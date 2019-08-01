###### Programming with Python
---

Exercise 5.1: Write a program that reads numbers from the keyboard, and outputs
the number in the middle. The program stops when the user enters 0. It is
guaranteed that the user inputs odd number of numbers, and there are at most 21
numbers (including 0).

```
Sample input:         Sample output:
3                       11
9
123
11
12
99
0
```

<br>

Exercise 5.2: Write a program that reads n numbers from the keyboard where n =<
20. Then it writes these numbers to the screen in reverse order. The user will enter
n from the keyboard.

```
Sample input:         Sample output:
6                       99
3                       12
9                       11
123                     123
11                      9
12                      3
99
```

In the input, sometimes the numbers are given in one line as follows:
```python
3 9 123 11 12 99
```

There is an easy way to read and store them in an array:
```python
 myArray = input().split()
```

``input()`` reads everything in one line and ``split()`` splits at spaces in the input and provides the input as an array. However, we have a small problem here. As
you remember, we were converting an input to an integer after reading it. We
need to do the same thing here - convert each element of the array to an integer.
As the next step:

```python
for counter in range(len(myAccay):
    myArray[counter] = int(myArray[counter])
```

<br>

<center> - 44 - </center>
