# <center>Chapter 9: Python Tips and Tricks</center>
---

### 9.1. Expressions & Arithmetic Operations

In Java, we can break long lines into multiple lines using For example, the
following codes are the same:

```python
print("There are "+ secondsInADay + " seconds in one day.")
```


```python
print("There are "+ secondsInADay + str(secondsInADay) \
      + " seconds in one day.")
```

There are some shortcut operations in place of some arithmetic operations. They
are given in the following table:

Operator|Example|Eauivalent expression
-|-|-
+=|number += 10|number = number + 10
-=|number -= 10|number = number - 10
*=|number *= 10|number = number * 10
/=|number /= 10|number = number / 10

> [!NOTE]
> Be careful about not to divide a variable or a number by zero, or your program
will fail.

<br>

### 9.2. Loops

Sometimes we need to exit a loop depending on a condition in the middle of an
operation. At that times, we use ^break' command as follows:

```python
number = int(input())
for counter in range(20):
    isEven = number % 2
    if isEven == 0:
        square = number * number
        print(square)
    if number % 11 == 0：
        break
    number += 1
```

Here, we break the loop if the number becomes divisible by 11.

<br>

<center> - 75 - </center>
