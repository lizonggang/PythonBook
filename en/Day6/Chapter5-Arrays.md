###### Arrays
---

# <center>Chapter 5: Arrays</center>

### 5.1. Introduction

**Question:** Suppose user enters odd number of numbers from keyboard, and
program stops when she enters 0. The program writes the number she entered in
the middle. How can you write the program?

```
Sample input:               Sample output:
3                           11
9
123
11
12
99
0
```

In the example above user enters 7 numbers (including 0). The number in the
middle is 11 since it is the 4<sup>th</sup> number.

An array is a sequence of boxes. An array has a name and size like a variable. The
size of the array is the number of boxes in the array. The boxes are numbered from
0 to n - 1 where n is the size of the array.
Example 5.1:

```python
        myArray
        0  1  2  3  4  5
        3  7  12 4  8  11
```

An array is shown above. The name of the array is ``myArray`` and its size is 6.0<sup>th</sup>
value of the array is 3, and 4<sup>th</sup> value is 8.

### 5.2. Declaring Arrays

We declare arrays similar to variables. The only difference is that the size is
indicated in square brackets.

```python
myArray =[0] * 20
```

This creates an array of 20 spots with a 0 in each spot. The zeros can be changes to anything of any type including decimals and strings.

Array initialization is a little different. For instance:

```python
numbers = [3, 5, 12]
```

<br>

<center> - 41 - </center>
