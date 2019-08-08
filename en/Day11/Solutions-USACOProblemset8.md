                                                                              
### Solution for "Scavenger Hunt"
 
In the sample input, P and Q and 24 and 2, respectively.  
P has 8 factors: 1, 2, 3, 4, 6, 8, 12, 24 
Q has 2 factors: 1, 2 
There are 2 * 8 = 16 possible pairings (in sorted order): 
```
       1 1 
       1 2 
       2 1 
       2 2 
       3 1 
       3 2 
       4 1 
       4 2 
       6 1 
       6 2 
       8 1 
       8 2 
       12 1 
       12 2 
       24 1 
       24 2 
```

 
Read in the inputs (the P and Q locations). First find the factors P and Q. This can be done by checking all the  numbers <= N. After obtaining the factors of P and Q, find all pairs (i, j) such that i is a factor of P and j is a  factor of Q. Notice that this approach ensures that the output is sorted according to the specification of the problem.  


```python
read P, Q 

array p_factors[] 
for i from 1 to P:  
    if P % i == 0 
        add i to p_factors 

array q_factors[] 
for j from 1 to Q: 
    if Q % j == 0 
        add j to q_factors         
for i in p_factors 
    for j in q_factors 
        print i, j 
```

There's another implementation that doesn't involve using arrays to store the factors of P and Q first: 

```python
read P, Q 
for i from 1 to P: 
    // if i is a factor of P 
    if P % i == 0: 
        for j from 1 to Q: 
            // if j is a factor of Q 
            if Q % j == 0: 
                print i, j 
```
 
---


<br>


                                                                              

### Solution for "Claustrophobic Cows"  

 
The goal is to find the closest pair of cows. The distance is defined as sqrt(xdifference ^ 2 + ydifference ^ 2). In  the sample test data, the closest pair of cows are cows with index 7 and 9, which is obvious from a quick visual inspection of the graph given in the problem statement: 

```
10 | . . . . . . . 3 . . . . . 
 9 | . 1 . . 2 . . . . . . . . 
 8 | . . . . . . . . . . . . . 
 7 | . . . . . . . . . . 4 . . 
 6 | . . . . . . 9 . . . . . . 
 5 | . 8 . . . . . . . . . . . 
 4 | . . . . . 7 . . . . . . . 
 3 | . . . . . . . . . 5 . . . 
 2 | . . . . . . . . . . . . . 
 1 | . . . . 6 . . . . . . . . 
 0 --------------------------- 
                       1 1 1 1 
   0 1 2 3 4 5 6 7 8 9 0 1 2 3 
```

Check all pairs of cows with a nested for loop; update the stored values every time a smaller distance is found. After determining the pair of cows with the minimum distance, output the answer. 
 
In addition, note that the multiplication process may overflow an integer (use long long or something in C++). As another implementation tip, we don’t need square root function since we don’t need the actual distance but we just compare them. So, comparing the square root of two numbers is the same as comparing without square root.  

```python
read N 
array xcord[], ycord[] 
for i from 1 to N: 
    read xcord[i], ycord[i] 

// check the distance between all pairs 
minDist = very large number 
a = -1, b = -1 
for i from 1 to N: 
    for j from (i + 1) to N: 
        curDist = (xcord[i] - xcord[j])^2 + (ycord[i] - ycord[j])^2 
        if(curDist < minDist): 
            minDist = curDist 
            a = i, b = j 
print a, b 

```

