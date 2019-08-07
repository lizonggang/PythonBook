
### Solution for "Square Pasture" 

**Let's look at the sample case from the problem:**

```
6 6 8 8
1 8 4 9
```


**We have two rectangles, one from (6, 6) to (8, 8), and another from (1, 8) to (4, 9). First, we should store this information so we can work with it. We'll store these variables starting with an x or y, whether they represent the lower-left (LL) or upper-right (UR) corner, and whether they are part of rectangle 1 or 2. We read these variables in the correct order from the input:**

```
read xLLl, yLLl, xURl, yURl
read xLL2, yLL2, xUR2, yUR2
```

**Now we need to find the smallest square that can encapsulate this. We know that the smallest rectangle goes from the minimum x-coordinate to the maximum x-coordinate and the minimum y-coordinate to the maximum y-coordinate. We know that the x and y-coordinates for the lower-left will be smaller than those for the upper-right, so we only need to consider the lower-left to find the minimums and upper-right to find the maximums. Here's an example to find the minimum x-coordinate:**

```python
declare minx
if xLLl < xLL2: //false for sample case
    minx = xLLl
else:
    minx = xLL2 //so minx = 1 for sample case
```

***In our sample case, the minimum x-coordinate would now be 1. We take a similar approach for the minimum y (6) and maximum x (8) and y (9). To solve the problem, we need the area of the square, which means we will
need the side length. Since the square must encapsulate the rectangle, the side length must be the maximum of the width and height. So, we must find the width and height and then find the side length.***

```python
width = maxx-minx //8-1 = 7 for sample case
height = maxy-miny //9-6 = 3 for sample case
declare sideLength
if width > height: //true for sample case
    sideLength = width //so sideLength = 7 for sample case
else:
    sideLength = height
```

**Now we just have to put it all together to find the area (the side length squared [for the sample case, 7*7=49]).
The full code is below.**


```python
read xLLl, yLLl, xURl, yURl
read xLL2, yLL2, xUR2, yUR2

declare minx, maxx, miny, maxy
if xLLl < xLL2:
    minx = xLLl
else:
    minx = xLL2
if xURl > xUR2:
    maxx = xURl
else:
    maxx = xUR2
if yLLl < yLL2:
    miny = yLLl
else:
    miny = yLL2
if yURl > yUR2:
    maxy = yURl
else:
    maxy = yUR2

width = maxx-minx
height = maxy-miny
declare sideLength
if width > height:
    sideLength = width
else:
    sideLength = height

output sideLength*sideLength
```



---

<br>

### Solution for "Contest Timing" 


**When we read the sample case, we see that we could find the difference in days, then the difference in hours, and finally the difference in minutes. First read the input into memory.**

read D, H, M //for the sample case, 12, 13, and 14

**The difference in days is easy to compute:**

diffDays = D-ll //for the sample case, 1

**Now we have to convert this to hours, and add the difference in hours:**

diffHours = 24*diffDays!(H-l1) //for the sample case, 24*1+2 = 26

**Finally, convert to minutes and add the difference in minutes:**

diffMins = 60*diffHours!(M-ll) //for the sample case, 60*26+3=1563

**The last thing to check is that this difference is not negative, which would mean that the time given is before Bessie's starting time. Then, we just output the answer**

```python
if diffMins < 0: //false for the sample case
    output -1
else:
    output diffMins //outputs 1563
```
**Here is the whole thing:**


```python
read D, H, M
diffDays = D-ll
diffHours = 24*diffDays+(H-ll)
diffMins = 60*diffHours+(M-ll)
if diffMins < 0:
    output -1
else:
    output diffMins
```
