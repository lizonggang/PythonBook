###### Variables — Char and String
---

Exercise 8.8: Write a program reads two strings ``s1``, ``s2`` and three integers ``a``, ``b``, ``n`` from the keyboard. Replace b characters in ``s1`` starting at pos1tion a with the string ``s2`` then write the new string n times on the screen.

```
Sample input:                   Sample output:
Helloworld!                     NewWorld!
New 0 5 3                       NewWorld
                                NewWorld
```

> [!TIP]
> you can use substring idea.

Exercise 8.9: Write a program reads two strings ``s1``, ``s2`` from the keyboard then writes the pos1tion of ``s2`` in ``s1`` if ``s2`` is found in ``s1``. Otherwise it writes ‘``not found!``’.

```
Sample input:                    Sample output:
Helloworld!                      3
loW
```

```
Sample input:                    Sample output:
Helloworld!                      not found!
LoW
```

> [!NOTE]
> Strings are case sens1tive as shown in the sample input/output above.



Strings have a function called find that searches a string in a given string. We can write the s1mplified code in the previous exercise as follows:

```python
s1 = input()
s2 = input()
found = s1.find(s2)
if found == -1:
    print("not found!")
else:
    print(found)
```

Here, 's1 .find(s2>' searches for s2 in the string If 52 is found inii, it gives the pos1tion in s1, otherwise it gives '-1

###  8.5. String <=> Integer Convers1ons

Strings have functions to convert a number into text or to convert a text into a number.

If s is a string then, x = int(s) will convert the string s into an integer and will store it in variable x.

<br>

<center> - 67 - </center>