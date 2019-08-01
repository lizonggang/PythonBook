## Chapter 5: Solutions - Part 1

**Question 1：Exercise 5.1**

```python
myArray = [0] * 21
counter = 0
number = int(input())
while number != 0 :             # store number in an array
    myArray[counter] = number
    counter = counter + 1
    number = int(input())
middle = int(counter / 2)       # middle location of the array. has to be int
print(myArray[middle])          # write the number in the middle
```

**Question 2：Exercise 5.2**

```python
myArray = [0] * 20
n = int(input)  # read n from keyboard
# read n numbers in reverse order
for counter in range(n) :
    number = int(input())
    myArray[counter] = number
 # write numbers in reverse order
 for counter in range(n - 1, -1 , -1) :
    print(myArray[counter])
```

An alternative way:

```python
myArray = [0] * 20
n = int(input)# read n from keyboard
# read n numbers from keyboard and reverse store them
for counter in range(n - 1, -1 , -1) :
    number = int(input)
    myArray[counter] = number
 # write numbers
 for counter in range(n):
    print(myArray[counter])
```

**Question  3:**

```python
myArray = [0] * 20
n = int(input) # read n from keyboard
# read n numbers in reverse order
for counter in range(n):
    myArray [counter] = int(input)
# read a and b from keyboard
a = int(input)
b = int(input)
for counter in range(n);
    # output the counter'th number in the array if it is divisible by a or b
    if myArray[counter] % a == 0 or myArray[counter] % b == 0 :
        print(myArray[counter])
```


**Question 4：Exercise 5.5\*\***

```python
arr = [0] * 20
    # read n and then n numbers into an array
n = int(input)
for i in range(n) :
    arr[i] = int(input())
# check numbers at position 0 and n-1, 1 and n-2, ...
# until the middle of the array
symmetric = 1
left = 0
right = n-1
while left<right :
    if arr[left] != a r r [ r i g h t ] :
        symmetric =0
    left = left + 1
    right = right - 1
# if array is not symmetric, output "not" first
if symmetric == 0 :
    print("not", end = •_ •，）
print("symmetric")
```


An alternative way:

```python
arr = [0] * 20
rev = [0] * 20
    # read n and then n numbers into an array
n = int(input)
for i in range(n):
    arr[i] = int(input)
    # save the numbers in reverse order
    rev[n-i-l]=arr[i]
# if array is not symmetric, output "not" first
symmetric = 1
for i in range(n):
    if arr[i] != rev[i]:
        symmetric =0
# if array is not symmetric, output "not" first
if symmetric == 0:
    print("not", end=" ")
print("symmetric")
```

**Question  5:**

```python
arr = [0] + 20000
n = int(input)
# read numbers into an array
for i in range(n):
    arr[i] = int(input)
k = int(input)
pos = -1 # position of k in the array
# check if k is in the array
for i in range(n):
    if arr[i] == k :
        pos = i
        break
        # break command must be used here for first occurance
print(pos)
```


**Question  6:**

```python
arr = [0] * 200
n = int(input)
# read numbers into an array
for i in range(n):
    arr[i] = int(input)
    if arr[i] == 0:   # output 0's first
        print(0, end=" ")

# output the array except 0's
for i in range(n):
    if arr[i] != 0 :
        print(arr[i], end=" ")
```


**Question  7:**

```python
arr = [0] * 200
n = int(input())
# read numbers into an array
for i in range(n) :
    arr[i] = int(input())
    if arr[i] < 0 :   # output negative numbers first
        print( arr[i] , end=" ")

# out the array except negative numbers
for i in range(n):
    if arr[i] >= 0 :
        print( arr[i] , end=" ")
```

