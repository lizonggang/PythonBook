###### Programming with Python
---


Exercise 8.5: Write a program reads a string s and three integers a, b and n fromthe keyboard, and writes the substring of s that starting from a th position and continues b characters, n times on the screen.

```
Sample input:                   Sample output:
Helloworld!                     oworl
4                               oworl
5                               oworl
5                               oworl
                                oworl
```



In the example above, the substring starting from 4<sup>th</sup> position is ‘``oworl``’. 

We can get a part of a string similar to arrays. We can write the simplified code in the previous exercise as follows:

```python
s = input()
a = int(input())
b = int(input())
n = int(input())
substring = s[a:a+b]
for counter in range(n):
    print(substring)
```

s[a:a+b] is the substring of s from index a to index a+b (excluding a+b).


Exercise 8.6: Write a program reads two string si, s2 and two integers a, n from
the keyboard. Insert s2 at a th position of si then write the new string n times on the screen.

```
Sample input:                   Sample output:
Helloworld!                     HelloNewworld!
New 5 3                         HelloNewworld!
                                HelloNewworld!
```

> [!TIP]
> you can use substring idea.

Exerdse 8.7: Write a program reads a string s and three integers a, 6, 《 from the keyboard. Delete b characters in s starting at position a then write the new string n times on the screen.

```python
Sample input:                    Sample output:
Helloworld!                 Helld!
2 5 3                     Helld!
                            Helld!
```

> [!TIP]
> you can use substring idea.

<br>

<center> - 66 - </center>