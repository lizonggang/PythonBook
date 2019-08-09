**Question 1**

```
Promotion Counting
==================

Bessie the cow is helping Farmer John run the USA Cow Olympiad 
(USACO), an on-line contest where participants answer challenging 
questions to demonstrate their mastery of bovine trivia.

In response to a wider range of participant backgrounds, Farmer 
John recently expanded the contest to include four divisions of 
difficulty: bronze, silver, gold, and platinum. All new 
participants start in the bronze division, and any time they score 
perfectly on a contest they are promoted to the next-higher 
division. It is even possible for a participant to be promoted 
several times within the same contest. Farmer John keeps track of a 
list of all contest participants and their current divisions, so 
that he can start everyone out at the right level any time he holds 
a contest.

When publishing the results from his most recent contest, Farmer 
John wants to include information on the number of participants who 
were promoted from bronze to silver, from silver to gold, and from 
gold to platinum. However, he neglected to count promotions as they 
occurred during the contest. Bessie, being the clever bovine she 
is, realizes however that Farmer John can deduce the number of 
promotions that occurred solely from the number of participants at 
each level before and after the contest. Please help her perform 
this computation!

PROBLEM NAME: promote

INPUT FORMAT:

Input consists of four lines, each containing two integers in the 
range 0..1,000,000. The first line specifies the number of bronze 
participants registered before and after the contest. The second 
line specifies the number of silver participants before and after 
the contest. The third line specifies the number of gold 
participants before and after the contest. The last line specifies 
the number of platinum participants before and after the contest.

OUTPUT FORMAT:

Please output three lines, each containing a single integer. The 
first line should contain the number of participants who were 
promoted from bronze to silver. The second line should contain the 
number of participants who were promoted from silver to gold. The 
last line should contain the number of participants who were 
promoted from gold to platinum.

SAMPLE INPUT:

1 2
1 1
1 1
1 2

SAMPLE OUTPUT:

1
1
1

In this example, 1 participant was registered in each division 
prior to the contest. At the end of the contest, 2 participants 
were registered in bronze and platinum. One way this could have 
happened is that 2 new participants joined during the contest; one 
was promoted all the way to platinum, and the other stayed in 
bronze.
```


<br>

**Question 2**

```
Bedtime Reading, I
==================

Farmer John was performing his nightly bedtime reading duties for
Bessie. "Oh, this gives me a headache," moaned Bessie.

"But it's just simple number theory," replied FJ. "Let's go over
it again. The sigma function of a number is just the sum of the
divisors of the number. So, for a number like 12, the divisors are
1, 2, 3, 4, 6, and 12. Summing them we get 28."

"That's all there is to it?" asked Bessie.

"Yep." replied FJ. "Perhaps someone will write a program to calculate
the sigma function of an integer I (1 <= I <= 1,000,000)."

PROBLEM NAME: br1

INPUT FORMAT:

* Line 1: A single integer, I

SAMPLE INPUT:

12

OUTPUT FORMAT:

* Line 1: The sum of all of I's divisors.

SAMPLE OUTPUT:

28
```
