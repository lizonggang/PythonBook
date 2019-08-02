###### Functions
On the other hand, we can call functions using variables. For instance, the
following program writes the value of 10<sup>z</sup> to the screen where z is read from the keyboard.

```python
def Power(x, y)：
    prod = 1
    for i in range(y):
        prod *= x
    return prod

z = int(input())
pow =Power(10, z)
print(pow)
```

In the program above, note that instead of writing,
```python
pow = Power(10, z)
print(pow)
```

we can directly write,
```python
print(Power(10, z))
```

without defining the variable ``pow``.

We can also call the functions with expressions. For instance, the following
program writes the value of  10<sup>z * t + 2</sup> to the screen where ``z`` and ``t`` is read from the keyboard.


```python
def Power(x, y):
    prod = 1
    for i in range(y):
        prod *= x
    return prod

z = int(input())
t = int(input())
print(Power(10, z * t + 2))
```

In a function '``return``' command immediately returns the specified value, and the rest of the code in the function is not executed. For instance, Power function below immediately returns 0 if Ihe value of ``y``(the exponent) is a negative number.

```python
def Power (x, y):
    if y < Ot
        return 0

    prod = 1
    for i in range(y):
        prod *= x
    return prod
```

<br>

<center> - 85 - </center>