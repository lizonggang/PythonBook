**Question 1**

```
Scavenger Hunt
==============

Farmer John has scattered treats for Bessie at special places in
the pasture.  Since everyone knows that smart cows make tasty milk,
FJ has placed the treats at locations that require Bessie to think.
He has given her two numbers, P and Q (1 <= P <= 6,000; 1 <= Q <=
6,000), and she has to check every point in the pasture whose
x-coordinate is a factor of P and whose y-coordinate is a factor
of Q to find her treat.

Suppose FJ gives Bessie P = 24 and Q = 2. Here are all of their
respective factors:

P = 24 => 1, 2, 3, 4, 6, 8, 12, 24
Q = 2 => 1, 2

Bessie would thus check grid locations: (1, 1), (1, 2), (2, 1), (2,
2), (3, 1)...

Help Bessie by printing all of the points she ought to check.

PROBLEM NAME: scavhunt

INPUT FORMAT:

* Line 1: Two space separated integers: P and Q

SAMPLE INPUT:

24 2

OUTPUT FORMAT:

* Lines 1..?: A complete list of unique pairs of space-separated
        integers sorted by the first number and, if tied, the second
        number: a factor of P followed by a factor of Q

SAMPLE OUTPUT:

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

**Question 2**

```
Claustrophobic Cows
===================

Farmer John has acquired a set of N (2 <= N <= 2,000) touchy cows
who are conveniently numbered 1..N. They really hate being too close
to other cows. A lot.

FJ has recorded the integer X_i,Y_i coordinates of every cow i (1
<= X_i <= 100,000; 1 <= Y_i <= 100,000).

Among all those cows, exactly two of them are closest together. FJ
would like to spread them out a bit. Determine which two are closest
together and print their cow id numbers (i) in numerical order.

By way of example, consider this field of cows (presented on a
typewriter grid that has slightly different proportions than you
might expect):

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

Quick visual inspection shows that cows 7 and 9 are closest together
(the distance separating them is sqrt(1*1+2*2) = sqrt(5), so the
output would be '7 9' on a single line (without quotes, of course).

PROBLEM NAME: claust

INPUT FORMAT:

* Line 1: A single integer: N

* Lines 2..N+1: Line i contains the coordinates of cow i expressed as
        two space-separated integers: X_i and Y_i

SAMPLE INPUT:

9
2 9
5 9
8 10
11 7
10 3
5 1
6 4
2 5
7 6

INPUT DETAILS:

As in the example.

OUTPUT FORMAT:

* Line 1: The two numerical IDs of the closest pair of cows (sorted)

SAMPLE OUTPUT:

7 9
```


