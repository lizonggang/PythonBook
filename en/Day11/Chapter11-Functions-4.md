###### Programnung with Python

Exercise 11.4: Write a program that reads three strings from the keyboard and
checks if the number of vowels in these strings are equal.

```
input:                     output:
ThBeE GOOD VoWeLs          Same number of vowels.
ThBeE equal VoWeLs         Not same number of vowels.
```

We can call functions inside a function. The order of the functions doesn't matter.
For example,

```python
def PowerOflO(k):
    return Power(10, k|

def Power (x, y):
    prod = 1
    for i in range(y):
        prod *= x
    return prod

z = int(input())
print(PowerOflO(z))
```

In the code above ``PowerOflO`` function calls Fower function hence Power function is below it.

> [!NOTE]
> As you noticed, functions are especially veiy useful when we have
to do a process many times. They also organize a messy code, makes it more
understandable.

<br>

### 11.2. Functions with No Return Value

Sometimes we don't need a return value from a function.

Example 11.2: Write a program that reads two strings and writes the number of
digits in these strings on the screen.

```python
def NumOfDigits(s):
    digits = 0
    for letter in s:
        if letter >= 101 and letter <= '9':
            digits += 1
    print(digits)

s1 = input()
s2 = input()
NumOfDigits(s1)
NumOfDigits(s2)
```

<br>

<center> - 86 - </center>