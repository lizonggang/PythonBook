###### Variables — Char and String
---
# <center>Chapter 8: Variables - Char and String</center>
  
### 8.1. Introduction

String variables can hold any characters such as letters and digits. For instance, you can put 'John' in a string variable, but not in an integer variable. Value assignment is same as integer variables:

```python
myVariable = "John"
```

puts 'John' in myvariable.

> [NOTE]
> We can use either single (') or double quotes (") before and after ``John``.

Example 8.1: Write a program that reads your name from the keyboard and prints it on the screen 5 times as ‘Your name is John.’ if the name is ‘John’.

```
Sample input:                       Sameple output: 
 John                               Your name is John.
                                    Your name is John.
                                    Your name is John.
                                    Your name is John.
                                    Your name is John.
                                    Your name is John.
```

Solution: 

```python
name = input()
for counter in range(5):
    print("Your name is " + name + ".")
```

In strings, '+' means to concatenate them.

For instance,

```python
firstname = "John"
lastname = "Doe"
fullname = firstname + " " + lastname
print(fullname)
```

the output becomes

```
John Doe
```

Note that we added a space between ``firstname`` and ``lastname``.

<br>

<center> - 61 - </center>
