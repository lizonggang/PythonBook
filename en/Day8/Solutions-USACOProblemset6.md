### Solution for "Perfect Squares"


In the sample input, there are 2 solutions for (a, b) such that a ^ 2 - b ^ 2= 15:
(4, 1): 16-1 = 15
(8, 7): 64-49 = 15

Read in the inputs, which is the difference of the two squares (N). Check all the possible combinations of a and b such that aA2-bA2 = N. If a satisfying pair is found, increment the count by 1. Finally, print the total number of pairs.

```python
read N
answer = 0
for b from 1 to 500:
    for a from b + 1 to 500
        if a * a - b * b == N
            answer = answer + 1

output answer
```

Instead of using nested loops to check all combinations of a and b, this can be done with one loop enumerating the values of a and constructing the possible values of b.

```python
read N
answer = 0
for a from 1 to 500
    if isPerfectSquare(a * a - N)
        answer = answer + 1

output answer
```

For example, when a = 4, a possible value of b can be calculated by checking if b is an integer, b = sqrt(a A 2 - N) = sqrt(16 -15). The value 1 is a perfect square, so b can be obtained and the answer is incremented by 1.

We check if a number is a perfect square in different ways. A perfect number’s root has to be an integer. An easy implementation is as follows:

```python
function isPerfectSquare(X):
    Y = int(sqrt(X))
    if Y ^ 2 == X:
        return true
    else
        return false
```

**An alternative solution** to solve this problem is to find the divisors of N elegantly. Since N = aA2-bA2, this can be rewritten as N = (a + b) * (a - b). For each pair of divisors such that p * q = N and p >= q, solve the
system (a + b = p, a - b = q) -> (a = (p + q) / 2). If a is an integer (p + q is divisible by 2) then a pair (a, b) satisfying the condition stated in the problem statement exists.

In the sample case, N = 15. One possible factorization is p = 5 and q = 3; In this case, a can be solved to be (3 + 5) / 2 = 4; and b is then 1. This is consistent with the aforementioned solutions.

```python
read N
answer = 0
for i from 1 to sqrt(N):
    // if i and (N/i) is the divisor pair and
    //if (i + N / i) is divisible by 2
    // Note that always i <= (N / i)
    if N % i == 0 and (i + N / i) % 2 == 0:
        answer = answer + 1
```

---

<br>



### Solution for "Wheel Rotation"

In the sample test case, pulley 1 is connected to pulley 2 with a straight belt, so pulley 2 is the same direction as pulley 1 (clockwise). Pulley 3 is connected to pulley 2 with a straight belt, so it's also in the clockwise direction. Pulley 4 is connected to pulley 3 with a cross belt, so it's the opposite direction as that of pulley 3, which makes it counterclockwise (1).

**A simple idea is as follows:** store the belt information in arrays. Starting from the first pulley, use a nested loop to find the belt that drives the next pulley. Then determine direction of next pulley. Repeat until the direction of the last pulley is determined.

```python
read N
numCross = 0
for i from 1 to N-l:
    read s[i] d[i] c[i]

eDir = 0
for i from 1 to N-l:
    for j from 1 to N-l:
        if s[j] == i:
            if c[j] == 1:
                if eDir = 1:
                    eDir = 0
                else :
                    eDir = 1
print eDir
```

**Alternate solution:**

In the previous solution, we don’t need to search for the pulley since it’s from 1 to N. We just need to store the pulley direction information in an array for pulley from 1 to N. Then we can determine the direction of rotation of each pulley from the start.

```python
read N
numCross = 0
for i from 1 to N-l:
    read s d c
    type[s] = c

eDir = 0
for i from 1 to N-l:
    if type[i] == 1:
        if eDir = 0:
            eDir = 1
        else:
            eDir = 0
print eDir
```

**Alternate solution:**

Here is a nice observation: in fact the order of the pulleys does not matter.

If two pulleys are connected by a straight belt, the direction of rotation of the driven pulley is the same as the driving pulley. However, if two pulleys are connected by a crossed belt, the direction of rotation of the driven
pulley is the opposite of the driving pulley. Therefore, we can count the number of crossed pulleys to count the number of times the direction is flipped. If the number is even, the direction of the final pulley will be the same as the direction of the first pulley. If the number is odd, the direction of the final pulley will be the opposite of the direction of the last pulley. Note that the order of the pulleys does not matter.

```python
read N
numCross = 0
for i from 1 to N-l:
    read s d c
    if c == 1:
        numCross += 1

if numCross is divisible by 2:
    print 0
else :
    print 1
```
