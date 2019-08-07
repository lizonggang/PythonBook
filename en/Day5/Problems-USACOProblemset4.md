**Question 1**

```
Teleportation
=============

One of the farming chores Farmer John dislikes the most is hauling 
around lots of cow manure. In order to streamline this process, he 
comes up with a brilliant invention: the manure teleporter! Instead 
of hauling manure between two points in a cart behind his tractor, he 
can use the manure teleporter to instantly transport manure from one 
location to another.

Farmer John's farm is built along a single long straight road, so any 
location on his farm can be described simply using its position along 
this road (effectively a point on the number line). A teleporter is 
described by two numbers x and y, where manure brought to location x 
can be instantly transported to location y, or vice versa.

Farmer John wants to transport manure from location a to location b, 
and he has built a teleporter that might be helpful during this 
process (of course, he doesn't need to use the teleporter if it 
doesn't help). Please help him determine the minimum amount of total 
distance he needs to haul the manure using his tractor.

PROBLEM NAME: teleport

INPUT FORMAT:

The first and only line of input contains four space-separated 
integers: a and b, describing the start and end locations, followed 
by x and y, describing the teleporter. All positions are integers in 
the range 0...100, and they are not necessarily distinct from 
each-other.

OUTPUT FORMAT:

Print a single integer giving the minimum distance Farmer John needs 
to haul manure in his tractor.

SAMPLE INPUT:

3 10 8 2

SAMPLE OUTPUT:

3

In this example, the best strategy is to haul the manure from 
position 3 to position 2, teleport it to position 8, then haul it to 
position 10. The total distance requiring the tractor is therefore 1 
+ 2 = 3. 
```

---

<br>

**Question 2**

```
Counting Beads
==============

Bessie has spilled her collection of N (1 <= N <= 80) blue and orange
cowbeads (represented as 1s and 0s, respectively, in the human world) on
the floor. She cleans up the mess by arranging the beads into a long line.
She then counts the number of times a blue bead is next to an orange bead
and vice versa, but is not sure if she is correct. Write a program to
validate Bessie's count.

PROBLEM NAME: countbead

INPUT FORMAT:

* Line 1: A single integer: N

* Line 2: Line 2 contains N integers, each of which is 0 or 1

SAMPLE INPUT:

6
1 0 0 1 1 1

INPUT DETAILS:

There are six beads in total: the first bead in the line is a blue bead,
followed by two orange beads, and finally by three blue beads.

OUTPUT FORMAT:

* Line 1: A single integer describing the number of occurrences that a
        blue bead is next to an orange bead and vice versa.

SAMPLE OUTPUT:

2

OUTPUT DETAILS:

There are two times in the line that two differently colored beads are next
to each other.
```
