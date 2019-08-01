## Chapter 5: Solutions - Part 2

**Question 1：Exercise 5.6\*\***

```python
n = int(input()) # read n. n is the number of numbers
numbers = input().split() #  here we create an array, the name of the aray is numbers
# We neec to convert array items into integer
for i in range (len(numbers)):
    numbers[i] = int (numbers[i])
# Now we will create another array called freq.
# freq[x] will keep how many times x appears in the numbers array
freq = [0] * 1001 # The maximum of numbers array can be 1000. Because 1000 is inclusive
for i in range ( n ) :
    freq[numbers[i]] = freq[numbers[i]] +1
for i in range (1001):
    if freq[i] > 1 :
        print (i)
```

<br>

**Question 2：Exercise 5.7\*\***

```python
n = int(input()) # read n. n is the number of numbers
numbers = input().split() #  here we create an array, the name of the aray is numbers # We neec to convert array items into integer
# We neec to convert array items into integer
for i in range (len(numbers)):
    numbers[i] = int (numbers[i])
# Now we will create another array called freq.
# freq[x] will keep how many times x appears in the numbers array
freq = [0] * 1001 # The maximum of numbers array can be 1000. Because 1000 is inclusive
for i in range ( n ) :
    freq[numbers[i]] = freq[numbers[i]] + 1
for i in range (1001):
    if freq[i] > 0 :
        print (i)
```

<br>

**Question 3：Exercise 5.8\*\*\***

```python
n = int(input()) # read n. n is the number of numbers
numbers = input().split() #  here we create an array, the name of the aray is numbers # We neec to convert array items into integer
# We neec to convert array items into integer
for i in range (len(numbers)):
    numbers[i] = int (numbers[i])
# Now we will create another array called freq.
# freq[x] will keep how many times x appears in the numbers array
freq = [0] * 1001 # The maximum of numbers array can be 1000. Because 1000 is inclusive
for i in range ( n ) :
    freq[numbers[i]] = freq[numbers[i]] + 1
i=0
while i<1001 :
    if freq[i] > 0 : # as long as the frequency if > 0 then print the index
        print (i)
        freq[i] = freq[i] - 1 # after each print decrease the frequency
    else :
        i = i + 1 # if the frequency is 0 then go to next one
```

<br>

**Question 4：Exercise 5.9\*\***

```python
n = int(input()) # read n. n is the number of numbers of first array
arrl = input().split() # here we create an array, the name of the aray is arrl
# We neec to convert array items into integer
for i in range (len(anrl)):
    arrl[i] = int (arrl[i])
m = int(input()) # read m. m is the number of numbers of second array
arr2 = input().split() # here we create an array, the name of the aray is arr2
# We neec to convert array items into integer
for i in range (len(arr2)):
    arr2[i] = int (arr2[ij)
# Now we will create 1 freq array to keep how many times x appears in arrl and arr2 combined
freq = [0] * 2001 # The maximum of arrays can be 1000. Because 1000 is inclusive
# However since we have negative numbers here we need to shift all numbers by 1000
for i in range ( n ) :
    freq[arrl[i]+1000] = freq[arrl[i]+1000] + 1
for i in range ( m ) :
    freq[arr2[i]+1000] = freq[arr2[i]+1000] + 1
i=0
while i<2001 : # The range is between 0 to 2000 inclusively
    if freq[i] > 0 : # checking freq
        print (i-1000 , end = " ") # shift back!
        f「eq[i] = f「eq[i] - 1
    else :
        i=i+1
```

<br>

**Question 5：Exercise 5.10\*\*\***

```python
n = int(input()) # read n. n is the number of numbers of first array
arrl = input().split() # here we create an array, the name of the aray is arrl
# We neec to convert array items into integer
for i in range (len(arrl)):
    a「rl[i] = int (a「rl[i])
m = int(input()) # read m. m is the number of numbers of second array
arr2 = input().split() # here we create an array, the name of the aray is arr2
# We neec to convert array items into integer
for i in range (len(arr2)):
    arr2[i] = int (arr2[i])
# Now we will create 1 freq array to keep how many times x appears in arrl and arr2 combined
freq = [0] * 2001 # The maximum of arrays can be 1000. Because 1000 is inclusive
# However since we have negative numbers here we need to shift all numbers by 1000
for i in range ( n ) :
    freq[arrl[i]+1000] = freq[arrl[i]+1000] + 1
for i in range ( m ) :
    freq[arr2[i]+1000] = freq[arr2[i]+1000] + 1
i=0
while i<2001 : # The range is between 0 to 2000 inclusively
    if freq[i] > 0 : # checking freq
        print (i-1000 , end = " ") # shift back!
        freq[i] = freq[i] - 1
    else :
        i=i+1
```

<br>

**Question 6：Exercise 5.110\*\*\***

```python
n = int(input()) # read n. n is the number of numbers of first array
arrl = input().split() # here we create an array, the name of the aray is arrl
# We neec to convert array items into integer
for i in range (len(anrl)):
    arrl[i] = int (arrl[i])
m = int(input()) # read m. m is the number of numbers of second array
arr2 = input().split() # here we create an array, the name of the aray is arr2
# We neec to convert array items into integer
for i in range (len(arr2)):
    arr2[i] = int (arr2[ij)
# make a position marker for each list
posl = 0
pos2 = 0
while posl < n and pos2 < m :
    # compare the numbers at current positions
    # output the smaller one and skip to the next number
    if arrl[posl] < anr2[pos2]:
        print (arrl[posl], end = " " )
        posl+= 1
    else :
        print (arr2[pos2], end = M ")
        pos2+= 1
# write the remaining numbers in the first list if any
while posl < n :
    print(arrl[posl], end = M ")
    posl+= 1
# write the remaining numbers in the second list if any
while pos2 < m :
    print(arr2[pos2], end = M ")
    pos2+= 1
```
