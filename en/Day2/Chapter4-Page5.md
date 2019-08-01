###### Looping
---

### 4.2. For Loops

Besides ``while`` loop we have another loop type; ``for`` loop. Let’s output the square of the even numbers between 1 and 30 inclusively. We can write the program
given at the beginning using while loop as follows:

```python
counter = 1                         # start from 1
while counter <= 30：               # loop until 30
    if counter % 2 == 0：           # if the current number is even
        print(counter * counter)    # output the square of it
    counter = counter + 1           # increase the counter
```

Another loop type is ``for`` loop.

```python
General form of for loop is:
    for counter in range(x, y):
        (expression)
        (expression)
        :  :  :        
```

Loop start with ``counter`` is equal to a: and repeats the expressions while ``counter`` is less then y. The above code can be written using ``for`` loop as follows:_

```python
for counter in range(1, 31)：       # start from 1, loop while < 31
    if counter % 2 == 0:            # if the current number is even
        print(counter * counter)    # output the square of it
```

Note that loop counter is updated at the end of each run of the expression in the
loop.

As you see, sometimes it is more practical to use ``for`` loop since it has a loop
counter, and it updates the loop counter at the end of each turn.

We can use ``range()`` in different ways. For instance,

```python
for counter in range(31)：          # start from 0, loop while < 31
    if counter % 2 == 0：           # if the current number is even
        print(counter * counter)    # output the square of it
```


When we have just one value in ``range()``, the counter starts from 0.

```python
for counter in range(8, 31, 2)：    # start from 8, loop while < 31, increase the counter by 2 each time
    if counter % 2 == 0：           # if the current number is even
        print(counter * counter)    # output the square of it
```

When we have the third value in ``range()``, the loop counter will be incremented
by that value.

We can also use variables in ``range()`` instead of values.

<br>

<center> - 33 - </center>

