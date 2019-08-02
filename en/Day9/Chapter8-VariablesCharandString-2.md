###### Programming with Python
---

Exercise 8.1: Write a program that reads your name and a number n from the
keyboard and prints your name on the screen n times, shifting one space each
time.

```
Sample input:        Sample output:
Jane                Jane
4                    Jane
                      Jane
                       Jane
```

### 8.2. String Operations

We can also put numbers in strings. However, they are not values, and you cannot
make arithmetic operations on them.

```python
numberl ="21"
number2 ="34"
sum = int(number1 + number2)
print(sum)
```
This prints 2134 because when strings are added, they combine into one big string.

We can do some operations with strings as mentioned above. We have already
seen, how to assign a value in a string such as:

```
name ="Jane"
```

We can also use addition (+) and (+=) operators to concatenate strings:

```
name ="Jane"
string ="Hello" + name
```
The string string will have "Hello Jane" in it.

Example 8.2: Write a program that reads a name and a number n from the
keyboard and prints the name on the screen n times as follows:

```
Sample input:        Sample output:
Jane                *Jane !
4                   **Jane !!
                    ***Jane !!!
                    ****Jane !!!!
```

Solution:

```python
name = input()
n = int(input())
name = " " + name + " "
for counter in range(n):
    name = "*" + name + "!"
    print(name)
```

<br>

<center> - 62 - </center>

