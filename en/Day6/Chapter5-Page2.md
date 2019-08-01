
###### Programming with Python
---


puts 3, 5, and 123 in the array in order. Similarly we can split the array above into
variables as follows:

```python
[a, b, c] = numbers
```


Then the variables a, b and c will be 3, 5 and 123 respectively. We can merge
arrays, add to the front or to the end of an array using '+’ operator:

```python
numbers = [11, 2] + numbers
```


will make numbers [11,2,3,5,123]。

We can get a part of an array as follows:

```python
  a = numbers[1：4]
  b = numberst[:3]
  c = numbers[2:]
```

Then a will be [2, 3, 5] which is the elements from position 1 to position 4
(excluding position 4). b will [11, 2, 3]; the elements from starting position to 3rd whereas c will [3, 5, 123]; the elements from 2ⁿd position to the end.

We can also initialize an array with different patterns such as:

```python
  myArray = [1, 5] * 3
```

This one repeats 1 and 5 three times. This is equivalent to:

```python
  myArray =[1, 5, 1, 5, 1, 5]
```

Sometimes we may need the size of an array. We can learn the size of an array as
follows:

```python
print(len(myArray))
```

``len()`` returns the size of an array.

<br>

### 5.3. Writing and Reading Arrays

We can use arrays similar to the variables. Suppose we have an array named
myArray with the size 10. In order to put 7 into 5,h location of the array, we write
the following code:

```python
  myArray[5] = 7
```

The only difference from variables is we always indicate the location in the arrays.
In this example location is indicated in square brackets.

We can use the number in a location of the array similar way. Suppose we have a
variable named apple and an array named banana. To assign the value 6 more
than the 4lh value of banana, we write the following code:

```python
  apple = banana [4] + 6
```
  
We can use all arithmetic operations we learned before on the values of an array.

<br>

<center> - 42 - </center>