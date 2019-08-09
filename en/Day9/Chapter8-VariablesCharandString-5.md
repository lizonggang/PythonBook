###### Variables — Char and String
---

In the code above, we wrote the name of the string variable then a dot and '``len()``' to get the size of the string. The code fragment above will write '12' on the screen (including the space and exclamation mark).

Example 8.5: Write a program that outputs the middle character of a string. If it doesn't have, write '``No middle character!``' on the screen.

```
Sample input:           Sample output:
Trial                   i
```

```
Sample input:           Sample output:
Helloworld              No middle character!
```

Solution:

```python
s = input() 
# if the size of the string is
if len(s) % 2 == 0:
    print("No middle character!")
else:
    middle = int(len(s)/2)
    print(s[middle])
```


Exercise 8.3: Write a program reads a string from the keyboard and writes the
reverse of it on the screen.

```
Sample input:           Sample output:
Trial                   lairT
```

Exercise 8.4: Write a program reads a string and an integer n from Ihe keyboard
and writes the reverse of it ``n`` times on the screen.

```
Sample input:           Sample output:
5                       lairT
                        lairT
                        lairT
                        lairT
                        lairT
```
<br>

<center> - 65 - </center>