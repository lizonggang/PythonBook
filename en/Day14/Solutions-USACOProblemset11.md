                                                                              
### Solution for "The Robot Plow"
 
In the sample input, all the squares from (1,1) - (2,4) and (1,3) - (5,4) has been plowed. In the first instruction, 8 squares were plowed. In the second instruction, 10 squares were plowed. However, the total number of squares plowed is 14 because the regions (1,1) - (2,4) and (1,3) - (5, 4) have an overlapping region (1, 3) - (2, 4) of size 4. So the actual number of squares plowed is 14.  
 
Simulate the problem. Keep track of what is plowed and what is not (all squares are initially unplowed). Then, at the end, loop through the matrix and count the plowed squares. We use 1-indexing to correspond to the problem statement. 
 
Initially, set all entries of the matrix to false to indicate that the land is unplowed. 

```python
read X, Y, I 
array plowed[241][241] 
for x from 1 to X: 
    for y from 1 to Y: 
        plowed[x][y] = false 
```

Iterate over all the plowing instructions and mark the squares plowed as true

```python
for i from 1 to I: 
    read Xll, Yll, Xur, Yur 
    for x from Xll to Xur: 
        for y from Yll to Yur: 
            plowed[x][y] = true 
```

After processing all the plowing instructions, count the number of squares that has been marked true (plowed) 

```python
count := 0 
for x from 1 to X: 
    for y from 1 to Y: 
        if plowed[x][y]: 
            count += 1 
output count 
```

---

<br>


 

### Solution for "Parkside’s Triangle"

 
Let’s look at a sample case: 
``5 3 ``
 
In this case, we must start with the number 3 and create 5 levels where the numbers are in increasing order  mod 9. The increasing numbers are first placed vertically then horizontally as follows: 
```
3 4 6 9 4 
  5 7 1 5 
    8 2 6 
      3 7 
        8 
```

In our solution, we must simulate this process and create an array such as the following: 

```
3 4 6 9 4 
0 5 7 1 5 
0 0 8 2 6 
0 0 0 3 7 
0 0 0 0 8 
```

Then, we print the array while replacing all 0's with blanks. To create this array, we place down 1 number in the first column, then two in the second column, up to n numbers in the nth column. Each number we place down is one greater than the previous one, except we take each number mod 9 (other than 9 itself) because we only want the digits 1-9.  
 
```python
read n,s 
array[n][n] 
for i from 0 through n-1: 
    for j from 0 through i: 
        array[j][i] = s 
        s = (s+1) mod 9 
        if array[j][i]= 0: 
            array[j][i] = 9 

for i from 0 through n-1: 
    for j from 0 through n-1: 
        if array[i][j] > 0: 
            print array[i][j], " " 
        else:  
            print "  " 
    print to new line 
```

