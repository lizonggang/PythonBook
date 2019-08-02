###### Programming with Python
---


Exercise 8.2: Sort given three strings according to alphabetical order.

```
Sample input:            Sample output:
hello                    Try
about                    about
Try                      hello
```

### 8.3. Strings as Character Arrays

We can in fact consider strings as an array of characters. That is, we can reach a specific character of a string similar to the arrays as follows:

```python
print(name[3])
```

The code above will print the 4lh character of the string name on the screen. Note
that the first character of the string is located at the position 0 - the same as arrays.

However the following code produces an error:

```python
name[3] = 'z'
```

To change a character in a string, we cannot do it as above. We will revisit how
to change a string later.

We can convert a string to a character array using ``list()`` function. For instance:

```python
s = "testing"
chararray = list(s)
```

chararray will be ['t', 'e', 's', 't, 'i ', 'n', 'g']。

Similarly, we can also convert a character array to a string using ``join()`` function:

```python
s = "".join(chararray)
```

Here the value inside tells join n how to merge the elements of the array. For
instance:

```python
s = "-".join(chararray)
```

``s`` becomes “t-e-s-t-i-n-g”。

### .4. String Functions

Strings have different useful functions. One of them is len function that gives the number of characters in a string. Remember that we used ``len()`` to get the size of an array too. It can be used as follows:

```python
s = "Hello world!"
theLength = len(s)
print(theLength)
```

<br>

<center> - 64 - </center>