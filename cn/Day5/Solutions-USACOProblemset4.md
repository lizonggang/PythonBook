### Solution for "Teleport"

**In this problem, there are three cases. First, Farmer John can get from point a to point b without using a single teleport. Second, Farmer John can get from point a to point b by using the teleport in the x to y direction. Finally, FJ can use the teleport in the y to x direction. The solution for this problem involves testing all three cases and finding the shortest one.**

**The sample problem uses the following values:**
```
3 10 8 2
```

**This means that FJ is trying to get from point 3 to point 10 by using the teleport that connects point 2 to point 8. Essentially, he has three options: go from point 3 to point 2, teleport to point 8, and then go to point 10; go from point 3 to point 8, teleport to point 2, and then to point 10; or go directly from point 3 to point 10. The three options require travel distance 3, 13, and 7. Clearly, 3 is the shortest so it is the correct answer. Once again, in general, FJ must test all three cases and take the shortest one.
**
```
read a,b,x,y
distance = absoluteValue(a - b)
distance = min(distance, absoluteValue(a-x) + absoluteValue(b-y))
distance = min(distance, absoluteValue(a-y) + absoluteValue(b-x))
print distance
```

---

<br>

### Solution for "Counting Beads"



**Before I present the solution, let’s examine how we would solve the sample case:**

```
6
10 0 111
```

**In this case, as we iterate through the 6 beads, we count how many times two adjacent beads are of different colors. Here, bead 1 is of a different color than bead 2, and bead 3 is of a different color than bead 4. Therefore, there are 2 occurrences of adjacent beads with different colors.**


**Now, we must extend this idea to n beads of arbitrary colors. To do this, we can use a variable called "previous." As we read in each bead, we check if its color is different than previous; if it is, we increment a counter. Then, we set the value of "previous" to the color of the current bead. This way, we can track the number of times two adjacent beads are of different colors.**

```
read n
read a
previous = a
for i from 2 through n:
    read a
    if previous != a:
        counter++
    previous = a

print counter
```
