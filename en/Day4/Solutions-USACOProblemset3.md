### Solution for "Another Cow Number Game"

**Our strategy will be to just simulate the game, keeping track of the number of steps as we go. As always, we read the input first. We should also keep a counter for the answer, which will count the number of steps**

```
read N
steps = 0
```

**Now the problem tells us that the game is finished when N=1. That means we have to continue while N is not 1, which we can do using a while loop.**
```
while N != 1:
```


**Next, we need to actually simulate the game. According to the rules, if N is even, we divide N by 2. We know that N is even if it has no remainder when we divide it by two, so:**

```
if N%2 = 0:
    N /= 2
```

**Otherwise (else), N is odd. In this case, the problem says to multiply N by 3 and add 1:**
```
else :
    N = 3*N+1
```
**Finally, we need to update our steps variable, since every time we make a move it counts as a step.**
```
steps = steps + 1
```

**We are now ready to output our answer! Here is the full code:**

```
read N
steps = 0
while N != 1:
    if N%2 = 0:
        N /= 2
    else :
        N = 3*N+1
    steps = steps + 1
output steps
```


---

<br>

### Solution for "Milk Pails"

**For this problem, we are given the three pails with sizes X, Y, and M. The goal of this problem is to add exactly either X or Y units of milk at a time to the pail of size M to fill the pail as much as possible. In the sample case, the big pail (size M) has a capacity of 77, and the two smaller pails have sizes 17 and 25. To fill the big pail as much as possible, FJ uses the pail of size 17 three times and the pail of size 25 one time, so that the total amount of milk in the big pail after this process is 17 * 3 + 25 * 1 =76 units.**

**Read in the inputs (the capacities of the pails). For a general solution, the approach is to find the maximum value of a * x + b*y such that a * x + b* y <= m. This can be done with a nested loop checking all combinations of a and y satisfying the above constraint.**

```
read x, y, m

answer = 0
a = 0
while a * x <= m:
    b = 0
    while b * y <= m:
        answer = max(answer, a * x + b * y)
        b += 1
    a += 1
print(answer)
```

**For an additional challenge, this can be accomplished without using nested loops. Instead of finding the maximum amount of milk that can be reached. Find the minimum of the modulus and subtract from the capacity of m.**

```
read x, y, m

answer = m
a = 0
while a * x <= m:
    answer = min(answer, (m - a * x) % y)
    a += 1
print(m - answer)
```

**Using this solution, for example, when a = 3, (m - a * x) % y = (77 - 3 * 17) % 25 = 26 % 25 = 1. The minimum modulus that can be obtained is 1, so the maximum amount to which the pail can be filled is the total capacity subtracted by the modulus: 77 - 1 = 76, which is consistent with the answer obtained by the other solution.**

