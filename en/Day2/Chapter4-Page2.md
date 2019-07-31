###### Programming with Python
---

The following code also does the same work. This time counter starts from zero.
As soon as loop starts, ``counter`` is incremented by 1. So, x + 1 is written on screen in the first step. The condition is counter < 100 since the loop must end as soon as counter reaches to 100.

```python
x = int(input())            # read x from keyboard
counter = 0                 # initially the counter is 0
while counter < 100:        # while counter is less than 100
    counter = counter + 1
    print(x + counter)
```

Example 4.2: Write a program that reads numbers and outputs if they are greater
than 5. Program will stop when 0 is given.

```
Sample input:               Sample output:
11                          11
8                           8
2                           7
2
4
7
5
0
```

Solution：

```python
number = 1
while number != 0:              # while number is not equal to 0
    number = int(input())       # run this loop
        if number > 5:          # read the number from keyboard   
            print(number)       # if the number is greater than 5
```

<br>

Exercise 4.2: Write a program that finds the count of the given numbers. Program
will stop when 0 is given.

```
Sample input:               Sample output:
11                          7
8
2
2
4
7
5
0
```

<br>

<center> - 30 - </center>


