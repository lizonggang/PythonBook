###### Conditionals
---

# <center>Chapter 3: Conditionals</center>
---

###　3.1. If statement

Suppose Katy says “If it rains, I use my umbrella”.

Similarly, we can have conditional statements in Python.

For example, we can put a condition like:

&nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; If x is greater than 5, write ‘x is greater than 5’.

Example 3.1: Write a program that reads a number from the keyboard and writes
‘x is greater than 5’ if the given number is greater than 5.

```python
x = int(input())
if x > 5:
    print("x is greater than 5")
```

> [!NOTE]
> The line starting with print is indented (have typically 4 spaces or a tab).
> It will be an error if it is not indented.


### 3.2. If-else

Suppose Taylor says “If it rains, I use my umbrella else I wear my sunglasses”.

Similarly, in a conditional statement in our program, we can tell the computer
what to do if the condition is **false**.

For example,
&nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; If x is greater than 5, write ‘x is greater than 5’ else write ‘x is not greater than 5’


Example 3.2: Write a program that reads a number from the keyboard and writes
‘x is greater than 5’ if the given number is greater than 5. Otherwise, it writes ‘x
is not greater than 5’.

```python
x =  int(input())
if x > 5:             # if x is greater than 5
    print  ("x is greater than 5")

else:                 # otherwise
    print  ("x is not greater than 5")
```
    
<br>

<center> - 21 - </center>

