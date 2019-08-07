**Question 1**

```
Another Cow Number Game
=======================

The cows are playing a silly number game again. Bessie is tired of
losing and wants you to help her cheat. In this game, a cow supplies
a number N (1 <= N <= 1,000,000). This is move 0. If N is odd, then
the number N is multiplied by 3 and incremented by 1. If N is even,
the number N is divided by 2. Each time the number is multiplied
or divided, the score increases by one point. The game ends -- and
the score is finalized -- when N becomes 1. If N is initially 1,
the score is 0.

Here's an example with N starting at 5:
 
        N     Next Value    Comment    Score
        5        16          3*5+1       1
       16         8           16/2       2
        8         4            8/2       3
        4         2            4/2       4
        2         1            2/2       5

The final score is 5.

PROBLEM NAME: acng

INPUT FORMAT:

* Line 1: A single integer, N

SAMPLE INPUT:

112


OUTPUT FORMAT:

* Line 1: A single integer that is the score for this game when
        starting at N

SAMPLE OUTPUT:

20
```

<br>

**Question 2**

```
Milk Pails
==========

Farmer John has received an order for exactly M units of milk (1 <= 
M <= 1,000) that he needs to fill right away. Unfortunately, his 
fancy milking machine has just become broken, and all he has are 
three milk pails of integer sizes X, Y, and M (1 <= X < Y < M). All 
three pails are initially empty. Using these three pails, he can 
perform any number of the following two types of operations:

- He can fill the smallest pail (of size X) completely to the top 
with X units of milk and pour it into the size-M pail, as long as 
this will not cause the size-M pail to overflow.

- He can fill the medium-sized pail (of size Y) completely to the 
top with Y units of milk and pour it into the size-M pail, as long 
as this will not cause the size-M pail to overflow.

Although FJ realizes he may not be able to completely fill the 
size-M

pail, please help him determine the maximum amount of milk he can 
possibly add to this pail.

PROBLEM NAME: pails

INPUT FORMAT:

The first, and only line of input, contains X, Y, and M, separated 
by spaces.

OUTPUT FORMAT:

Output the maximum amount of milk FJ can possibly add to the size-M 
pail.

SAMPLE INPUT:

17 25 77

SAMPLE OUTPUT:

76

In this example, FJ fills the pail of size 17 three times and the 
pail of size 25 once, accumulating a total of 76 units of milk. 
```

