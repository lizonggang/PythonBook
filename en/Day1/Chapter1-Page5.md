###### Introduction
---

Exercise 1.1: Write your name to the screen.   
Open a new file, name il as ‘``myname.py``’, save it on the desktop and run it.

> [!NOTE]
> You can use single and double quotations inside the parenthesis. 

Exercise 1.2: Write your name twice to the screen.

Open a new file, name it as ‘``mynamek.py``’, save it on the desktop and run it.

Example 1.2: Write '``1232``' on the screen.
Open a new file, write the code below, name it as ‘``number.py``’, save it on the
desktop and run it.

```python
print(1232)
```

Exercise 1.3: Write your lucky number on the screen.

Open anew file, name it as ‘``lucky.py``’, save it on the desktop and run it.

The “``print``” statement automatically ends the line. The next time we use it, the ouput starts from the beginning of the next line. For example,

```python
print("quick brown fox")
print("jumped over the lazy dog")
```

will write;

```python
quick brown fox
jumped over the lazy dog
```
On the other hand,

```python
print("quick brown fox", end = "")
print("jumped over the lazy dog")
```

will output;

```python
quick brown foxjumped over the lazy dog
```

Note that there is no space between ‘fox’ and ‘jumped’. If we use end variable in
``print()``, it indicates what to print at the end of the line instead of pressing enter.
In this example, we used ``end = ""`` which mean not to put anything. Another
common usage is to put a space; ``end = " "``.

<br>

<center> - 9 - </center>


