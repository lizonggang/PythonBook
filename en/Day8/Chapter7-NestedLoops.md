###### Nested Loops
---

# <center>Chapter 7: Nested Loops</center>


Loops are used when we want to do the same job more than once. It might be completely the same or might have slight differences. But we can do each job by
running the same piece of code. For example, the code on the left prints 10
asterisks ‘*’ which is basically the same job at each loop. The code on the right
prints the numbers from 1 to 10 which is the same job with different parameters.
In both cases the pieces of code run in each loop are the same.

```python
for i in range(10):           for i in range(10):
    print ("*")                   print(i+1)
```

What if in each loop instead of doing one job, we want to do several jobs which
are again basically the same.‘The hands of an analog clock’ is a good example to
this. From noon to midnight, the hour hand of a clock shows 12 different numbers
in this interval. If we consider 0 and 12 means the same for the hour hand, we can
get all those values by using a ``for`` loop.

```python
for hourhand in range (12):
    print(hourhand)
```

Suppose we would like to write all the minutes in an analog clock. We know that
there are 60 minutes in an hour, and for each number the hour hand points in the
clock, the long hand points 60 different numbers. Incrementing the minute by one
is a job. Doing it 60 times is a loop of the same kind of job. In other words,
incrementing the hour 12 times, and incrementing the minute 60 times whenever
the hour is incremented is a loop of jobs in another loop. This is called nested
loops. For instance, the code below prints all the minutes between 00:00 and
11:59.

```python
for hourhand in range (12):
    for minutehand in range(60):
        print (hourhand, ":", minutehand)
```

Example 7.1 Write a program which prints all two-digit numbers that can be
composed of {0, 1, 2,3,4, 5}.


<br>

<center> - 55 - </center>

