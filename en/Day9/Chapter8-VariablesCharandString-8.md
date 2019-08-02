###### Programming with Python
---

As an example,

```python
x = int("12345")
```
will store “``123456``” in interger ``x``.

> [!NOTE]
> The string parameter of int function has to be a valid number otherwise it
 will be a error.


The opposite function also exists for converting a number into a string. For
example, ``s = str(x)`` will convert number ``x`` into string ``s``.

As an example,

```python
s = str(12345)
```

will store “``123456``” in string s.

### 8.6. Array of Strings

Remember that we declared arrays that are composed of integer values:

```python
mylntArray = [0] * 10
```

declares an array of 10 integers. Similarly, we can declare arrays with string values:

```python
myStrArray = [""] * 10
```

declares an array of 10 strings. We can read from and write to the array locations
in the same way.

Example 8.6: Read an integer n then n words from the input and write the words
in reverse order. There will be maximum 100 strings in the input.

```
Sample input:                   Sample output:   
4                               About
Helloworld!                     TryIt!
Hello                           Hello
TryIt!                          HelloWrold!
About
```

Solution:

```python
n = int(input())
words = [nn] * 100

# read n words from the input
for counter in range(n):
    words[counter 1 = input()

# write words on the screen in reverse order
for counter in range (n-1, -1, -1):
    print(words[counter])
```

<br>

<center> - 68 - </center>

