## Chapter 3: Solutions
This page contains the solutions except the optional ones:

##### Question 1: Example 3.1

```python
x = int(input()) # read x from keyboard
if x > 5:   # if x is greater than 5
    print('x is greater than 5')
```

<br>

##### Question 2: Example 3.2

```python
x = int(input())    # read x from keyboard
if x > 5:       # if x is greater than 5
    print('x is greater than 5')
else:
    print('x is not greater than 5')
```

<br>

##### Question 3: Exercise 3.1

```python
x = int(input())
y = int(input())
if x > y:           # if the first number is greater
    print(x)        # write the first number
else:               # otherwise
    print(y)        # write the second number
```

<br>

##### Question 4: Exercise 3.3

```python
number = int(input())
if number % 6 == 3:
    print(number)
number = int(input())
if number % 6 == 3:
    print(number)
number = int(input())
if number % 6 == 3:
    print(number)
```

<br>

##### Question 5: Example 3.3

```python
x = int(input())    # x from the keyboard
if x > 5 and x < 10: # if x is greater than 5 and less than 10
    print('x is less than 4')
```

<br>

##### Question 6: Example 3.4

```python
x = int(input())
if x > 5 or x < 10:
    print('x is less than 4')
else:
    print('x is greater than 15')
```

<br>

##### Question 7: Exercise 3.4

```python
x = int(input())
if x > 10 and x != 15:
    print('I liked it')
else:
    print('I didn't like it')
```

<br>

##### Question 8: Example 3.6

```python
score =- int(input())
if score < 50:
    print('not good')
elif score >= 50 and score < 70:
    print('fair')
elif score >= 70 and score < 90:
    print('good')
else:
    print('awesome')
```

<br>

##### Question 9: Exercise 3.6

```python
x = int(input())
if x % 2 == 0:
    print('This is an even number')
else:
    print('This is an odd number')
```

<br>

##### Question 10: Exercise 3.7*

```python
a = int(input())
b = int(input())
c = int(input())
if a <= b and a <= c:
    print(a)
elif b <= a and b <= c:
    print(b)
elif c <= a and c <= b:
    print(c)
```

<br>

##### Question 11: Exercise 3.9

```python
x = int(input())
y = int(input())
if x % y == 0:
    print('divisible')
else:
    print('not divisible')
```

<br>

##### Question 12: Exercise 3.10*

```python
a = int(input())
b = int(input())
c = int(input())
if a + b == c or a + c == b or b + c == a:
    print('sum of two')
if a * b == c or a * c == b or b * c == a:
    print('product of two')
```

<br>

##### Question 13: Exercise 3.11**

```python
a = int(input())
b = int(input())
c = int(input())
if a <= b and b <= c:
    print(str(a) + '\n' + str(b) + '\n' + str(c))
elif a <= c and c <= b:
    print(str(a) + '\n' + str(c) + '\n' + str(b))
elif b <= a and a <= c:
    print(str(b) + '\n' + str(a) + '\n' + str(c))
elif b <= c and c <= a:
    print(str(b) + '\n' + str(c) + '\n' + str(a))
elif c <= a and a <= b:
    print(str(c) + '\n' + str(a) + '\n' + str(b))
else:
    print(str(c) + '\n' + str(b) + '\n' + str(a))

# In the above example we could have used 18 print statements (3 of them for each case)
# However we used str() function which converts integers to strings. String is like words
# You can combine words with + operator.
# Also keep in mind that "\n" means a new line
```

<br>

##### Question 14: Exercise 3.12

```python
t = int(input())
h = int(input())
if t < 60 adn h < 40:
    print('Lucy drinks coffee')
elif t >= 60 and h < 40:
    print('Lucy drinks iced tea')
else:
    print('Lucy eats ice cream')
```

<br>

##### Question 15: Exercise 3.13

```python
t = int(input())
h = int(input())
if t < 60 and h < 40:
    print('Lucy drinks coffee')
elif t < 60 and h < 60:
    print('Lucy plays tennis')
elif t < 60 and h >= 60:
    print('Lucy eats cake')
elif t >= 60 and h < 40:
    print('Lucy drinks iced tea')
elif t >= 60 and h < 60:
    print('lucy plays golf')
else:
    print('Lucy eats ice cream')
```

