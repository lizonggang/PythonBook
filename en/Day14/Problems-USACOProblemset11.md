**Question 1**

```
The Robot Plow
==============

Farmer John has purchased a new robotic plow in order to relieve
him from the drudgery of plowing field after field after field. It
achieves this goal but at a slight disadvantage: the robotic plow
can only plow in a perfect rectangle with sides of integer length.

Because FJ's field has trees and other obstacles, FJ sets up the
plow to plow many different rectangles, which might end up overlapping.
He's curious as to just how many squares in his field are actually
plowed after he programs the plow with various plow instructions,
each of which describes a rectangle by giving its lower left and
upper right x,y coordinates.

As usual, the field is partitioned into squares whose sides are
parallel to the x and y axes. The field is X squares wide and Y
squares high (1 <= X <= 240; 1 <= Y <= 240). Each of the I (1 <= I
<= 200) plow instructions comprises four integers: Xll, Yll, Xur,
and Yur (1 <= Xll <= Xur; Xll <= Xur <= X; 1 <= Yll <= Yur; Yll <=
Yur <= Y) which are the lower left and upper right coordinates of
the rectangle to be plowed. The plow will plow all the field's
squares in the range (Xll..Xur, Yll..Yur) which might be one more
row and column than would initially be assumed (depending on how
you go about your assumptions, of course).

Consider a field that is 6 squares wide and 4 squares high. As FJ
issues a pair of plowing instructions (shown), the field gets plowed
as shown by '*' and '#' (normally plowed field all looks the same,
but '#' shows which were most recently plowed):

    ......             **....             #####.
    ......  (1,1)(2,4) **....  (1,3)(5,4) #####.
    ......             **....             **....
    ......             **....             **....

A total of 14 squares are plowed.

PROBLEM NAME: rplow

INPUT FORMAT:

* Line 1: Three space-separated integers: X, Y, and I

* Lines 2..I+1: Line i+1 contains plowing instruction i which is
        described by four integers: Xll, Yll, Xur, and Yur

SAMPLE INPUT:

6 4 2
1 1 2 4
1 3 5 4

INPUT DETAILS:

As in the task's example.

OUTPUT FORMAT:

* Line 1: A single integer that is the total number of squares plowed

SAMPLE OUTPUT:

14
```

**Question 2**

```
Parkside's Triangle
===================

Bessie taught the cows to make Parkside's Triangle. It is generated from
two numbers: the size and the seed. The size N (1 <= N <= 20) determines
how many rows are in the triangle and the seed S (1 <= S <= 9) determines
the first number in the triangle. Here are two examples:

 N=5, S=3                  N=6, S=1  

3 4 6 9 4                1 2 4 7 2 7    
  5 7 1 5                  3 5 8 3 8    
    8 2 6                    6 9 4 9    
      3 7                      1 5 1   
        8                        6 2  
                                   3

The first line of any triangle has no blanks at its front.

Analyze the above examples, discover the rule, and write a program
that will generate Parkside's Triangle given any size N (1 <= N <=
20) and any seed S (1 <= S <= 9).

PROBLEM NAME: pktri1

INPUT FORMAT:

* Line 1: Two space-separated integers: N and S

SAMPLE INPUT:

5 3

OUTPUT FORMAT:

* Lines 1..N: Parkside's Triangle as above; no trailing blanks on any
        line.

SAMPLE OUTPUT:

3 4 6 9 4
  5 7 1 5
    8 2 6
      3 7
        8
```

