
Question1：Example 4.1

```python
x = int(input())            # read x from keyboard
counter = 1                 # initially the counter is 1
while counter <= 100:       # while counter is less than or
    print(x + counter)      # equal to 100 execute this loop
    counter = counter + 1   # increase the counter by 1
```

Question2：Example 4.2

```python
number = 1
while number != 0:          # while number is not equal to 0 run this loop
    number = int(input())   # read the number from keyboard
    if number > 5:          # if the number is greater than 5
        print(number)
```

Question3：Example 4.2

```python
number = int(input())       # read the number from keyboard
counter = 0
while number != 0:          # while number is not equal to 0
    counter = counter + 1
    number = int(input())
print(counter)
```

Question4：Example 4.3

```python
x = int(input())            # read x number from keyboard
number = int(input())       # read the number for the first time
while number != 0 :         # while number is not equal to 0 # execute this loop
    if number > x:          # if the number is greater than x
        print(number)
    number = int(input())
```

Question5：Example 4.4

```python
n = int(input())
counter = 1
while counter <= n:
       print(counter)
       counter = counter + 1
```

Question6：Example 4.5

```python
n = int(input())                
counter = 0                     # loop counter
power = 1;                      # the variable to keep the power of 2. Initially power is equal to 1
while counter < n:              
       power = power * 2        # multiply the current power by 2
       counter = counter + 1    
print(power)
```


Question7：Example 4.6

```python
n = int(input())                # n numbers from keyboard
counter = 0                     # loop counter
total = 0                       # the variable to keep the sum. The total is initially 0   
while counter < n:              # repeat the loop n times
       number = int(input())    # read number
       total = total + number   # add the number to the total
       counter = counter + 1    # increase counter
 print(total)                   # write the total after the loop
```

Question8：Example 4.7

```python
number = int(input())
while number <= 35 and number >= 17:
      print(number)
```

