**Question 1**

```
Perfect Squares
===============

Farmer John is playing a game with Bessie. He picks two positive
integers A and B (1 <= B <= A <= 500), and Bessie is supposed to
deduce which numbers he picked. He gave Bessie the following hint:

The numbers I chose have the property that the square of the
larger number is N (1 <= N <= 1,000) larger than the square of
the smaller number.

Being a smart cow, Bessie knows that this hint will greatly reduce the
number of possibilities for A and B. However, she is asking you to help by
writing a program to compute the exact number of solutions possible.

PROBLEM NAME: squares

INPUT FORMAT:

* Line 1: A single integer: N

SAMPLE INPUT:

15

INPUT DETAILS:

How many pairs of positive integers (A, B) satisfy A^2 = B^2 + 15?

OUTPUT FORMAT:

* Line 1: A single integer representing the number of possible
solutions

SAMPLE OUTPUT:

2

OUTPUT DETAILS:

There are two solutions: (A, B) = (4, 1) and (A, B) = (8, 7)
```

---
<br>

**Question 2**


Wheel Rotation
\==============

Farmer John has an old-time thresher (wheat harvester) that requires belts to be installed on various gears to turn the parts. The engine drives pulley 1 in a clockwise direction which attaches via a belt to pulley 2. Pulley 2 attaches via a belt to pulley 3 and so on through a total of N (1 <= N <= 1,000) pulleys (and N-1 belts).

![](http://legendary.cdn.play8.io/learnpython/en/img/day8/d8-usaco-1.png)


The diagram above depicts the two ways a belt can be installed between two gears. In this illustration, pulley 1's belt directly drives pulley 2 (a 'straight' connection) and thus they will rotate in the same direction. Pulley 3 drives pulley 4 via a 'crossed belt' that reverses the direction of the rotation.

Given a list of the belt types that connect the pulleys along with the fact that pulley 1 is driven in a clockwise direction by the engine, determine the drive direction of pulley N. Each belt is described by three integers:

  \* S_i -- the driving (source) pulley
  \* D_i -- the driven (destination) pulley
  \* C_i -- the connection type (0=straight, 1=crossed)

Unfortunately, FJ lists the belts in random order.

By way of example, consider the illustration below. N = 4, and pulley 1 is driven clockwise by the thresher engine. Straight belts drive pulley 2 and then pulley 3, so they rotate clockwise. The crosswise belt reverses the rotation direction so pulley 4 (pulley N) rotates counterclockwise.

![](http://legendary.cdn.play8.io/learnpython/en/img/day8/d8-usaco-2.png)

PROBLEM NAME: rotation

INPUT FORMAT:

\* Line 1: A single integer: N

\* Lines 2..N: Each line describes a belt with three integers: S_i,
        D_i, and C_i

SAMPLE INPUT:

4
2 3 0
3 4 1
1 2 0

INPUT DETAILS:

As in the example illustration.

OUTPUT FORMAT:

\* Line 1: A single integer that is the rotation direction for pulley N
        (0=clockwise, 1=counterclockwise)

SAMPLE OUTPUT:

1
