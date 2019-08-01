## Chapter 4: Solutions - Part 2
This page contains the solutions:

**Question 1：Exercise 4.8**

```python
number = int(input())
if number % 7 == 3:
    print(number)
while number != 0:
    number = int (input())
    if number % 7 == 3 :
        print(number)
```

<br>

**Question 2：Exercise 4.9**

```python
total = 0
number = int(input())
while number != 0 :
    total = total + number * number
    number = int (input())
print(total)
```

<br>

**Question 3：Exercise 4.10**

```python
n = int(input())
print(n)
while n > 1 :
    if n % 2 == 0 :
        n = n / 2
    else :
        n = n * 3 + 1
    print(int(n))
```

<br>

**Question 4：Exercise 4.11\***

```python
 number = 1
 counter = 0
 total = 0
 while number != 0 :
    number = int (input())
    if counter < 5 :        # if one of the first 5 numbers
            total = total + number
    counter = counter + 1
 print(total)
```
<br>

**Question 5：Exercise 4.12\*\***

```python
number = 1
counter = 0
total = 0
while number != 0:
    last = number       # save the last number before reading the next
    number = int(input())
    if counter < 5: # if one of the first 5 numbers
        total = total + number
    counter = counter + 1
print(total + last)
```

<br>

**Question 6：Exercise 4.13**

```python
counter = 10
while counter <= 55:
# if ones digit is less than 6 output the number
    if counter % 10 < 6:
        print(counter)
    counter = counter + 1
```

Alternatively we can use the following idea:


```python
# keep one and tens digits separately
tens =1
ones = 0
# output first tens digit then ones digit
while tens < 6 :
    print(str(tens)+str(ones))
    ones = ones +1
    # whenever ones digit is greater than 5
    # increase tens digit and reset ones digit
    if ones > 5 :
        ones =0
        tens = tens + 1
```

<br>

**Question 7：Exercise 4.14**

```python
counter = 50
while counter >= 10:
    print (counter)
    counter = counter + 1
# if ones digit is greater than 5 skip to the next number
    if counter % 10 > 5:
        counter = counter - 16
```

Alternatively we can use the following idea:


```python
# keep ones and tens digits separately
tens = 5
ones = 0
while tens > 0 :
# output first tens digit then ones digit
    print(str(tens) + str(ones))
    ones = ones + 1
    # whenever ones digit is greater than 5
    # decrease tens digit and reset ones digit
    if ones > 5 :
        ones =0
        tens = tens - 1
```
<br>

**Question 8：Exercise 4.15\***

```python
counter = 10
while counter < = 6 6:
    # if ones digit is less than 7
    # and it is odd, output the number
    if counter % 10 < 7 and counter % 2 == 1 :
        print(counter)
    counter = counter + 1
```

Alternatively we can use the following idea:

```python
# keep ones and tens digits separately
tens =1
ones = 1
while (tens < 7):
    # output first tens digit then ones digit
    print(str(tens)+str(ones))
    ones = ones + 2
    # whenever ones digit is greater than 6
    # increase tens digit and reset ones digit
    if ones > 6:
        ones = 1
        tens = tens + 1
```
<br>

**Question 9：Exercise 4.16\***

```python
for counter in range (100, 445):
    # if ones and tens digits are less than 5
    # output the number
    if counter % 10 < 5 and counter % 100 < 50 :
        print(counter)
```

Alternatively we can use the following idea:

```python
# keep ones and tens digits separately
hundreds=l
tens =0
ones =0
while hundreds < 5 :
    # output first hundreds then tens and ones digits
    print(str(hundreds)+str(tens)+str(ones))
    ones = ones + 1
    # whenever ones digit is greater than 4
    # increase ten digit and reset ones digit
    if ones > 4 :
        ones = 0
        tens = tens + 1
    # whenever tens digit is greater than 4
    # increase hundreds digit and reset tens digit
    if tens > 4 :
        tens = 0
        hundreds = hundreds + 1
```
<br>

**Question 10：Exercise 4.17\*\***
```python
# keep ones and tens digits separately
hundreds = l
tens = 0
ones = 0
while hundreds < 5 :
    # output first hundreds then tens and ones digits
    print(str(hundreds)+str(tens)+str(ones))
    ones = ones + 1
    # whenever ones digit is greater than 4
    # increase tens digit and reset ones digit
    if ones > 4 :
        ones = 0
        tens = tens + 1
    # whenever ones digit is greater than 4
    # increase hundreds digit and reset ones digit
    if tens > 4:
        tens = 0
        hundreds = hundreds + 1
```

