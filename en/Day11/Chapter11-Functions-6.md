###### Programming with Python
---

The variables defined in the main code are accessible from all functions. For
instance,

```python
def Power (x, y):
        global prod
        prod = 1
        for i in range (y):
            prod *= x

x = int(input())
Power(10, x)
print(prod)
```

``prod`` is defined in line 2 using the keyword "global". This time, ``prod`` is the same box that is used by both the main code and ``Power`` function. These type of variables are called **global** variables whereas the others are **local**. Note that if we don't use the definition in line 2, Python will consider prod belongs to only ``Power`` function and will give an error in line 9.

> [!NOTE]
> Avoid defining a global variable with the same name of a local variable.
That makes more confusion in the code.

Exercise 11.7: What is the output of the following program if user enters
``‘I8cakes’`` and ``‘try911``' from the keyboard respectively.

```python
global y
y = 0

def NumOfDigits(s, x):
    digits = 0

    for letter in s:
        if letter >= 101 and letter <= 191:
            digits += 1
    return digits + x

x = 3
s = input()
t = input()
print(NumOfDigits(t, 19))
y = x * 2
```

> [!NOTE]
> REMARK: It is better to define local variables as much as possible. We mostly
define global variables when we need to use the same variable in many functions.

<br>

#### Congratulations - end of lesson reached

Well done!

<br>

<center> - 88 - </center>