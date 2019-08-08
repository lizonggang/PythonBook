**Question 1**

```
Even? Odd?
==========

Bessie's cruel second grade teacher has assigned a list of N (1 <= N <=
100) positive integers I (1 <= I <= 10^60) for which Bessie must determine
their parity (explained in second grade as "Even... or odd?"). Bessie is
overwhelmed by the size of the list and by the size of the numbers. After
all, she only learned to count recently.

Write a program to read in the N integers and print 'even' on a single line
for even numbers and likewise 'odd' for odd numbers.

PROBLEM NAME: evenodd

INPUT FORMAT:

* Line 1: A single integer: N

* Lines 2..N+1: Line j+1 contains I_j, the j-th integer to determine
        even/odd

SAMPLE INPUT:

2
1024
5931

INPUT DETAILS:

Two integers: 1024 and 5931

OUTPUT FORMAT:

* Lines 1..N: Line j contains the word 'even' or 'odd', depending on
        the parity of I_j

SAMPLE OUTPUT:

even
odd

OUTPUT DETAILS:

1024 is eminently divisible by 2; 5931 is not
```

---

<br>


**Question 2**

```
Adding Commas
=============

Bessie is working with large numbers N (1 <= N <= 2,000,000,000) 
like 153920529 and realizes that the numbers would be a lot easier
to read with commas inserted every three digits (as is normally     
done in the USA; some countries prefer to use periods every three
digits). Thus, she would like to add commas: 153,920,529 .  Please
write a program that does this.

PROBLEM NAME: commas

INPUT FORMAT:

* Line 1: A single integer: N

SAMPLE INPUT:

153920529

OUTPUT FORMAT:

* Line 1: The integer N with commas inserted before each set of three
        digits except the first digits (as traditionally done in many
        cultures)

SAMPLE OUTPUT:

153,920,529
```

---

<br>

**Question 3**

```
String Function Encoding
========================

Bessie discovered a new function that the entire herd can apply to
its character strings.

Given both a number N (1 <= N <= 15) and a string S, with length
strictly greater than N, define f(N, S) as a new string composed
of the concatenation of the substring from character N (zero based
-- first character is number 0) through the end of S and the string
S itself.

For example, with N = 2, and S = "COW", f(N, S) = "W" + "COW" =
"WCOW". Also, f(3, "USACO") = "CO" + "USACO" = "COUSACO".

Bessie is enthralled with this function and wants to iterate it
several times. For example, if she iterates the function once for
"COW" and N = 2, she will get "WCOW". If she applies the function
with N = 2 again to that string, she will get "OWWCOW", and if she
applies it one more time with N = 2, she will get "WCOWOWWCOW".

Help Bessie encode a total of Z (1 <= Z <= 100) strings, str_1,
str_2, and so on.  Each str_i has length in the range 2..100 and
contains only upper case letters. Each string is presented with its
own N_i (0 <= N_i < length(str_i), and iteration count C_i (1 <= C_i
<= 12).

PROBLEM NAME: stringe

INPUT FORMAT:

* Line 1: A single integer: Z

* Lines 2..Z+1: Line i+1 contains two space-separated integers, a
        space, and string to be encoded: N_i, C_i, and str_i

SAMPLE INPUT:

2
2 3 COW
3 2 USACO

OUTPUT FORMAT:

* Lines 1..Q: Line j contains the iterated, encoded version of str_j

SAMPLE OUTPUT:

WCOWOWWCOW
SACOCOUSACO

OUTPUT DETAILS:

The arrow denotes an iteration of the function
COW -> WCOW -> OWWCOW -> WCOWOWWCOW
USACO -> COUSACO -> SACOCOUSACO
```

