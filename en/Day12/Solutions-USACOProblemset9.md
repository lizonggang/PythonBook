 ### Solution for "Crop Circles"
 
First, we need to read all the input and store it in an array. 

```python
read N 
array X[401], Y[401], R[401] 
for i from 1 to N: 
    read X[i], Y[i], R[i] 
```

The problem tells us we need to count something for each cow, meaning we will iterate through them and start a count: 

```python
for cow1 from 1 to N: 
    count = 0 
```

Then, we need to count the number of cows who overlap. We'll move that to a helper function, so for now we will just say that two cows i and j overlap if overlap(i, j) is true. We need to iterate through all the cows to check if they overlap, and then add to the count if they do. Remember that a cow cannot overlap with itself! 

```python
for cow2 from 1 to N: 
    if cow == cow2:                         // a cow can't overlap with itself 
        continue 
    if overlap(cow, cow2): 
        count += 1 
```

And we finish the loop by outputting the number of cows that overlap with it. Here's the code for the main function:

```python
read N 
array X[401], Y[401], R[401] 
for i from 1 to N: 
    read X[i], Y[i], R[i] 

for cow1 from 1 to N: 
    count = 0 
    for cow2 from 1 to N: 
        if cow1 == cow2:                  // a cow can't overlap with itself 
            continue 
        if overlap(cow, cow2): 
            count += 1 
    output count 
```
 
Now we just have to write the overlap function. We will need the X, Y, and R for each cow, but we can access  those from our function as long as we make sure to declare those arrays globally. 
 
When do two cows overlap? The cutoff should be when they are just touching, meaning that the sum of their  radii is equal to the distance between them, which we can calculate using the Pythagorean theorem. If the sum of their radii is any smaller, they don't overlap; otherwise, they do. 
 
We also want to avoid the square-root from the Pythagorean theorem, so we'll compare the distance squared with the sum of the radii squared. Here's the final overlap function 

```python
function overlap(i, j): 
    // Pythagorean Theorem 
    distSquared = (X[i]-X[j])^2 + (Y[i]-Y[j])^2 
    sumOfR = R[i] + R[j] 
    sumOfRSquared = sumOfR * sumOfR 
    if sumOfRSquared > distSquared: 
        return true 

    return false 
```

Notice that we returned false without an else clause. This is because if the if statement runs, the code below it never will, so the else clause is not necessary. Usually, this is better practice because it ensures that the function will return something. 

---

<br>


                                                                              

### Solution for "Bovine Bones"
 
In the sample input, with 3 dice of 3, 2, and 3 sides, all the possible outcomes are listed below: 
```
1 1 1 -> 3  1 2 1 -> 4  2 1 1 -> 4  2 2 1 -> 5  3 1 1 -> 5  3 2 1 -> 6 
1 1 2 -> 4  1 2 2 -> 5  2 1 2 -> 5  2 2 2 -> 6  3 1 2 -> 6  3 2 2 -> 7 
1 1 3 -> 5  1 2 3 -> 6  2 1 3 -> 6  2 2 3 -> 7  3 1 3 -> 7  3 2 3 -> 8 
```

The table below shows the possible sums are their numbers occurrences

sums|3|4|5|6|7|8 
-|-|-|-|-|-|-
occurrence|1|3|5|5|3|1 
 
Both 5 and 6 appear most frequently -- 5 times. Since the problem is asking for the smallest integer sum, in  this case when a tie occurs, 5 is chosen as the answer. 
 
To determine which sum appears the most frequently, we consider each of the equiprobable cases for which  the dice can land on. To do so, we loop over the possible values for the first dice, the values for the second  dice, and the values for the third dice. Inside the three loops, we calculate the sum and note its occurrence in  an array. Afterwards, we scan through the array looking for the sum with the most number of occurrences. 

```python
read S1 S2 S3 

for i from 1 to S1: 
    for j from 1 to S2: 
        for k from 1 to S3: 
            cSum = i + j + k 
            count[cSum] += 1 

mostFrequent = 0 

for i from 1 to S1 + S2 + S3: 
    if count[i] > count[mostFrequent]  
        mostFrequent = i 

print mostFrequent 
```

**Alternate Solution:** Alternatively, we can first loop over the sums. Then we can loop over the combinations of ​dice and count how many result in that sum. We keep track of which sum has the most ways to add up to that number. 
 

```python                                                                 
read S1 S2 S3 

mFSum = 0           // sum of maximum frequency 
mFFreq = 0          // maximum frequency 

// loop through all possible sums 
for cSum from 3 to S1 + S2 + S3: 
    cFreq = 0 
    // check all possible rolls 
    for i from 1 to S1: 
        for j from 1 to S2: 
            for k from 1 to S3: 
                if i + j + k == cSum: 
                    cFreq += 1 
    // update the maximum frequency 
    if cFreq > mFFreq 
        mFSum = cSum 
        mFFreq = cFreq 

print mFSum 
```

