###### Arrays
---

We can also use a variable to indicate the location of an array. For example,
suppose the variable x equals to 4:

```python
myArray [x] = 3
```

This code puts 3 into 4<sup>th</sup> location of ``myArray``. Note that

```python
myArray [x/2] = 3
```

will give an error since the result of division('/') in Python is not an integer.

<br>

Example 5.2: The program below defines an array of 6 locations and reads them
from the keyboard. Then it adds the 0<sup>th</sup> and 3<sup>th</sup> values, and puts into 5<sup>th</sup> location in the array. After that, it writes the 5<sup>th</sup> value to the screen.

```
Sample input:         Sample output:
3                     14
9
123
11
12
99
```

```python
myArray = [0] * 6
myArray[0] = int(input())
myArray[1] = int(input())
myArray[2] = int(input())
myArray[3] = int(input())
myArray[4] = int(input())
myArray[5] = int(input())

myArray[5] = myArray[0] + myArray[3]
print(myArray[5])
```

**Question:** If we need to read 100 numbers from the keyboard and put them into
the array, should we do it one by one?

**Hint:** No. We can use loops.

Solution: Without loops, we need to write a code similar to the following:

```python
myArray = [0] * 6
myArray[0] = int(input())
myArray[1] = int(input())
myArray[2] = int(input())
myArray[3] = int(input())
  :      :      :           # same pattern 100 times
myArray[99] = int(input())

```

Notice that the only change in the reading pattern is the location of the anav. It
goes from 0 to 99. Which means we can do it with a loop as follows:

```python
myArray = [0] * 100
for counter in range(100):
    myArray [counter] = int(input())
```


<br>

<center> - 43 - </center>
