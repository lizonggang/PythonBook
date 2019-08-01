# Hint for Chapter 5: Exercises - Part 2

**Reverse Indexing** is a good idea to solve some of these exercise questions. In simple words the reverse indexing can be described as using the index numbers of an array to store certain values.


Example: Imagine an exam. Minimum score is 0 and the maximum score is 10. There are 7 students

A teacher can store the scores of students in two ways:

1-)   Create an array and store the students that store scores student_scores [] =  {4, 6, 2, 10, 4, 7, 4}

2-)   Create an array for scores that stores score frequency score_frequency[]= {0,0,1,0,3,0,1,1,0,0,1}


<br>

**student_scores[]** is regular index. We just store the scores=

Student_0 has a score of 4

Student_1 has a score of 6

Student_2 has a score of 2 ... etc. and finally

Student_6 has a score of 4



On the other hand **score_frequency[]**  is reverse index which holds the data in a different way.

There is/are 0 student(s) who received 0 as a score

There is/are 0 student(s) who received 1 as a score

There is/are 1 student(s) who received 2 as a score

There is/are 0 student(s) who received 3 as a score

There is/are 3 student(s) who received 4 as a score

There is/are 0 student(s) who received 5 as a score

There is/are 1 student(s) who received 6 as a score

There is/are 1 student(s) who received 7 as a score

There is/are 0 student(s) who received 8 as a score

There is/are 0 student(s) who received 9 as a score

There is/are 1 student(s) who received 10 as a score



Pros and Cons of regular index and reverse index
- In regular index you can store any number (prō)
- In reverse index the data needs to be limited. (In this example the maximum score - was 10 So the array size needs to be at least 11.   If the data is not limited - reverse index can not be used) (contrā)
- In regular index  in order to sort the data you need a sorting algorithm  (contrā)
- In reverse index  the data is already sorted (prō)
- In regular index  you need to spend some effort to find the data frequency  (contrā)
- In reverse index  you store the frequency (prō)
- In regular index  you do not worry about the data that you store. (The data can be - negative for instance)  (prō)
- In reverse index  you can not keep negative values. Because array index always - starts from 0 and increases one by one.   (contrā) {In some cases you can overcome - this problem by shifting all the values by same amount}


Now here are the hints:

Question 1: Simple application of reverse index. All numbers are positive and the limit is 1000. (doable)

Question 2: All numbers are positive, distinct,  and the limit is 1000. (doable)

Question 3:  All numbers are positive and the limit is 1000. (doable) This time you need to consider that the numbers can repeat. They may not be distinct. When you print the result you will have a nested loop (preferable a while loop) that will continue printing the index(if the content at that index is greater then 0), decrease the index for each print. Stop printing the index once the content becomes 0

Question 4: Shift all numbers by 1000. (Because the minimum number is -1000. If you shift each and every number by 1000 then the minimum number will be stored in the 0th index of array. You need to create your array as large as 2001 in this question. Why ?
Question 5: There are 2 groups of data. The same reverse index array will be used for both groups of data. The limits are -1000 to 1000. A shift will be needed. The array size is around 2 thousands. (Doable)

Question 6: You can not use reverse indexing because the numbers are not limited as they were in Question 5. Therefore you need to find an alternative way.



Assume there are two variables. (I will call them indicator1 and indicator 2) in short Let's say i1 and i2

And there are two array. array a[] and array b[]

Array a has n numbers in it , and array b has m numbers in it.  So far so good

Now i1=0 and i2=0

In a loop of (m+n) numbers 

Compare a[i1]  versus b[i2]       If a[i1]<b[i2]  print a[i1] and increase i1 by1  else  print b[i2] and increase i2 

You need to be careful if i1 reaches its limit (which is n) and i2 reaches its limit (which is m) Try to avoid  "out of boundary" errors.

Once one array is done (I mean finished) you need to print the other array's remaining numbers. After all both arrays are sorted initially.

Last modified: Saturday, 15 June 2019, 10:23 AM