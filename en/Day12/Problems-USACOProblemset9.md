**Question 1**

Crop Circles
\============

Bessie and her fellow herd-mates have become extremely territorial. The N (1 <= N <= 400) cows conveniently numbered 1..N have all staked out a grazing spot in the pasture. Each cow i has a spot on an integer grid (0 <= X_i <= 10,000; 0 <= Y_i <= 10,000) and an integer radius R_i that indicates the circle she is staking out (1 <= R_i <= 500).

The cows are a bit greedy and sometimes stake out territory of their herd-mates. For each cow, calculate the number of other cows whose territory overlaps her territory. By way of example, consider these six cows with indicated locations and radii (don't confuse radius with diameter!):

![](http://legendary.cdn.play8.io/learnpython/en/img/day12/d12-usaco-1.png)


By visual inspection, we can see and count the overlaps, as shown.

NOTE: the test data will avoid pathological situations like tangents
where the circles just barely touch.

PROBLEM NAME: cropcir

INPUT FORMAT:

\* Line 1: A single integer: N
\* Lines 2..N+1: Three space-separated integers: X_i, Y_i, and R_i

SAMPLE INPUT:

```
6
7 7 7
16 14 7
11 13 2
10 17 3
29 8 5
15 7 4
```

OUTPUT FORMAT:

\* Lines 1..N: Line i contains a single integer that is the number of
        other fields that overlap with cow i's field.

SAMPLE OUTPUT:
```
3
4
3
2
0
2
```


---

<br>



```
Bovine Bones
============

Bessie loves board games and role-playing games so she persuaded
Farmer John to drive her to the hobby shop where she purchased three
dice for rolling. These fair dice have S1, S2, and S3 sides
respectively (2 <= S1 <= 20; 2 <= S2 <= 20; 2 <= S3 <= 40).

Bessie rolls and rolls and rolls trying to figure out which three-dice
sum appears most often.

Given the number of sides on each of the three dice, determine which
three-dice sum appears most frequently. If more than one sum can
appear most frequently, report the smallest such sum.

PROBLEM NAME: bones

INPUT FORMAT:

* Line 1: Three space-separated integers: S1, S2, and S3

SAMPLE INPUT:

3 2 3

OUTPUT FORMAT:

* Line 1: The smallest integer sum that appears most frequently when
        the dice are rolled in every possible combination.

SAMPLE OUTPUT:

5

OUTPUT DETAILS:

Here are all the possible outcomes.
1 1 1 -> 3  1 2 1 -> 4  2 1 1 -> 4  2 2 1 -> 5  3 1 1 -> 5  3 2 1 -> 6
1 1 2 -> 4  1 2 2 -> 5  2 1 2 -> 5  2 2 2 -> 6  3 1 2 -> 6  3 2 2 -> 7
1 1 3 -> 5  1 2 3 -> 6  2 1 3 -> 6  2 2 3 -> 7  3 1 3 -> 7  3 2 3 -> 8

Both 5 and 6 appear most frequently (five times each), so 5 is the answer.
```



