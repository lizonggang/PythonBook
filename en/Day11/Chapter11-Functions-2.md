###### Pmgramming with Python
---

> [!NOTE]
> The names of functions are case sensitive as it is in the variables.


Example 11.1: Write a function that returns the number of letters in a given string.

Solution:
```python
def NumLetters(s)：
    count = 0
    for letter in s:
        if (letter >= 'A' and letter <= 'Z') or \
           (letter >= 'a' and letter <= 'z'):
            count += 1
    return count
```


This code checks all the letters in string ``s`` within the ``for`` loop. If the current character is between ‘A’ and ‘Z’(uppercase) or ‘a’ and ‘z’(lowercase) then increments ``count``. Note that we use '\' to wrap long lines.

Exercise 11.1: Write a function named ``Uppercase`` that converts all letters to uppercase in a given string. For instance,

```python
print(UpperCase("I8-10caKes!"))
```

will write "I8-10CAKES!" on the screen.

Exercise 11.2: Write a function named SameWords that checks if two givens words are the same regardless of the case differences. If the strings are equal,function returns 1, otherwise 0.

For instance,
```python
print(SameWords("Trivial", "Trival"))
```

will write “l” on the screen.

```python
print(SameWords("tRiViAl", "TrIvIaL"))
```


Exercise 11.3: Write a function named Reverse that reverses a given string. For instance,

```python
print(Reverse("!esreveR"))
```

will write ‘``Reverse!``’, on the screen.

### 11.1. How to Call Functions

We can call functions with values. For instance, the function Power at line 14 in the first example is called with two values 10 and 3:

```python
pow =Power(10, 3)
```


<br>

<center> - 84 - </center>