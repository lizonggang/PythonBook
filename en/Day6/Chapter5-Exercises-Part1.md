**Question 1**
Write a program that reads numbers from the input, and outputs the number in the middle. The program stops when the user enters 0. It is guaranteed that the user inputs odd number of numbers, and there are at most 21 numbers (including 0).

**For example:**

Input|Result
-|-
3|11
9|
123|
11|
12|
99|
0|

<br>

**Question 2**
Write a program that reads N then N numbers from the input where N<=20. Then it writes these numbers to the screen in reverse order.

**For example:**

Input|Result
-|-
6|99
3|12
9|11
123|123
11|9
12|3
99|


**Question 3**
Read N then N numbers (N <= 20) from the input and put them into an array. Then read A and B and write the numbers in the array that are divisible by A or B in the same order.

**For example:**

Input|Result
-|-
7|15
15|21
19|6
7|18
21|
6|
37|
18|
3|
5|


**Question 4**
Given N then N numbers (N <= 20) find if the sequence of numbers is symmetric or not. If the sequence of numbers is symmetric, write "symmetric", otherwise write "not symmetric" on the screen.

**For example:**

Input|Result
-|-
8|not symmetric
15|
19|
7|
21|
6|
37|
18|
1|
7|symmetric
15|
19|
7|
21|
7|
19|
15|


**Question 5**
Find the index of the first occurrence of a number K, or -1 if it could
not be found. You will be supplied with a list of N numbers (1 <= N <=
20000).

For example, suppose you were given the following array as input.

```python
2 3 4 4 9 11 12
```

Searching for 4 should return 2, searching for 9 should return 4, and
searching for 10 should return -1.

INPUT FORMAT:

* Line 1: The integer N.

* Line 2: N sorted integers.

* Line 3: The integer K.

SAMPLE INPUT:

```python
7
2 3 4 4 9 11 12
9
```

OUTPUT FORMAT:

* Line 1: The index of the first occurrence of K in the supplied array, or -1 if not found.

SAMPLE OUTPUT:

```
4
```

OUTPUT DETAILS:


The index of 9 is 4.

<br>

**Question 6**
Read N then N numbers (N <= 200) from the input and put them into an array. Then
write the numbers out again, but with all the 0s moved to the front.

**For example:**

Input|Result
-|-
8|0 0 82 82 9 42 100 23
82|
82|
9|
42|
0|
100|
23|
0|

<br>

**Question 7**
Read N then N numbers (N <= 200) from the input and put them into an array. Then write the numbers out again, but with all the negative numbers moved to the front in the same order.

**For example:**
Input|Result
-|-
5|-32 -11 48 26 47
48|
26|
47|
-32|
-11|
