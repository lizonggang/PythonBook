**Question 1**


```
Math Practice
=============

One lovely afternoon, Bessie's friend Heidi was helping Bessie
review for her upcoming math exam.

Heidi presents two integers A (0 <= A <= 45) and B (1 <= B <= 9)
to Bessie who must respond with an integer E in the range 1..62.
E is the smallest integer in that range that is strictly greater
than A and also has B as the first digit of 2 raised to the E-th
power. If there is no answer, Bessie responds with 0.

Help Bessie correctly answer all of Heidi's questions by calculating
her responses.

By way of example, consider A=1 and B=6. Bessie might generate a table
like this:
         E         2^E    First digit of 2^E
         2          4            4
         3          8            8
         4         16            1
         5         32            3
         6         64            6      <-- matches B

Thus, E=6 is the proper answer.

NOTE: The value of 2^44 does not fit in a normal 32-bit integer.

PROBLEM NAME: mathprac

INPUT FORMAT:

* Line 1: Two space-separated integers: A and B

SAMPLE INPUT:

1 6

OUTPUT FORMAT:

* Line 1: A single integer E calculated as above

SAMPLE OUTPUT:

6
```


**Question 2**

```
Why Did the Cow Cross the Road
==============================

While the age-old question of why chickens cross roads has been 
addressed in great depth by the scientific community, surprisingly 
little has been published in the research literature on the related 
subject of cow crossings. Farmer John, well-aware of the importance 
of this issue, is thrilled when he is contacted by a local university 
asking for his assistance in conducting a scientific study of why 
cows cross roads. He eagerly volunteers to help.

As part of the study, Farmer John has been asked to document the 
number of times each of his cows crosses the road. He carefully logs 
data about his cows' locations, making a series of N
observations over the course of a single day. Each observation 
records the ID number of a cow (an integer in the range 1...10, since 
Farmer John has 10 cows), as well as which side of the road the cow 
is on.

Based on the data recorded by Farmer John, please help him count the 
total number of confirmed crossings. A confirmed crossing occurs when 
a consecutive sightings of a cow place it on different sides of the 
road.

PROBLEM NAME: crossroad

INPUT FORMAT:

The first line of input contains the number of observations, N, a 
positive integer at most 100. Each of the next N lines contains one 
observation, and consists of a cow ID number followed by its position 
indicated by either zero or one (zero for one side of the road, one 
for the other side).

OUTPUT FORMAT:

Please compute the total number of confirmed crossings.

SAMPLE INPUT:

8
3 1
3 0
6 0
2 1
4 1
3 0
4 0
3 1

SAMPLE OUTPUT:

3

In this example, cow 3 crosses twice -- she first appears on side 1, 
then later appears on side 0, and then later still appears back on 
side 1. Cow 4 definitely crosses once. Cows 2 and 6 do not appear to 
cross. 
```

