### Solution for "Math Practice"

In this problem, 2 integers A, B are given as the input. The goal is to find the smallest integer E such that 2 A ^ E > A and the first digit of 2 ^ E = B.

In the sample case, A = 1 and B = 6. As shown in the problem statement, a table can be generated like this:

```
E       2^E         First digit of 2^E
---     ---         ------------------
2       4           4                 
3       8           8                 
4       16          1                 
5       32          3                 
6       64          6                 
```


When E = 6; 2 ^ E = 64. This is the smallest value of E such that 2 ^ E is bigger than A (64 > 1) and the first digit of 64 is equal to B (6), so the answer is E.


This can be done with an enumeration of all the possible values of E, since E is in the range 1..62. For checking if the first digit is B, one way is to convert the number to a string, and take the first character, and convert the character back to an integer.


Python|C++|Java
-|-|-
ord(str(X)[0]) - ord('0')|to_string(X)[0] - '0'|("" + X).charAt(0) - '0'



Another way is to divide by decreasing powers of 10 until the first non-zero answer has been found.

```python
function firstDigitof(X)
    num = 10AY where 10AY is very large
    while int(X / num) == 0:
        num = num / 10
    return int(X / num)
```


If there's no answer that satisfies the above conditions, output 0. Note that 2 ^ e may overflow the integer type (use long long in C++ or something similar in other languages)

```c++
read A, B

for e in 1 . . 62 :                               
    if 2 ^ e > A and firstDigitof(2 ^ e) == B:
        output e                              
        end the program                       
output 0                                         
```


There's another solution that makes calculating the first digit easier -- without using the loop in the firstDigitOf function. Within the outer loop, keep track of the largest power of 10 that is smaller or equal to 2 ^ e. With that information stored, calculating the first digit only requires a single integer division operation. See the implementation below.

```python
read A, B                                 
pow10 = 1                                 
for e in 1..62:                           
    if 2 ^ e > pow10 * 10:                   
        pow10 *= 10        
    if 2 ^ e > A and int(2 ^ e / pow10) == B:       
        output e                                  
        end the program                           
output 0
```

---
<br>

### Solution for "Why Did the Cow Cross the Road?"


We know that a cow has crossed the road when we observe him on one specific side of the road at some time and on the other side of the road some time later. Therefore, we must track the locations of the 10 cows and increment the appropriate counter when we notice that a cow has crossed the road.

Let’s examine a sample case:
```
8
3 1
3 0
6 0
2 1
4 1
3 0
4 0
3 1
```

In this case, there are 8 observations regarding the 10 cows. We spot cow 3 on side 1, then side 0, then side 0 again, and finally side 1. With these observations, we can be sure that cow 3 switched sides at least twice. We only observe cows 6 and 2 once, so we cannot be sure if they switch sides at all. With cow 4, we observe him on side 1 and then on side 0, so we know that he switched sides at least once. Thus, in total, the number of switches we can confirm is 3.

```python
read n
answer = 0
declare array[] of size 10 and initialize all with -1

for i from 0 to n:
    read cowName,sideOfRoad
    if (array[cowname] is not 0) and (array[cowname] is not sideOfRoad):
        answer = answer + 1

    array[cowName] = sideOfRoad

print answer
```


