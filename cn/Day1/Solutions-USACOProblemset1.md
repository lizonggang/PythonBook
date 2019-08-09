
### “广场牧场”的解决方案

**让我们看看问题的示例案例：**

```
6 6 8 8
1 8 4 9
```


**我们有两个矩形，一个来自（6,6）到（8,8），另一个来自（1,8）到（4,9）。 首先，我们应该存储这些信息，以便我们可以使用它。 我们将以x或y开头存储这些变量，无论它们代表左下角（LL）还是右上角（UR），以及它们是否是矩形1或2的一部分。我们在正确的位置读取这些变量 从输入订单：**

```
read xLLl, yLLl, xURl, yURl
read xLL2, yLL2, xUR2, yUR2
```

**现在我们需要找到可以封装它的最小正方形。 我们知道最小的矩形从最小x坐标到最大x坐标，最小y坐标到最大y坐标。 我们知道左下角的x和y坐标将小于右上角的x和y坐标，因此我们只需要考虑左下角找到最小值，右上角找到最大值。 以下是查找最小x坐标的示例：**

```python
declare minx
if xLLl < xLL2: //false for sample case
    minx = xLLl
else:
    minx = xLL2 //so minx = 1 for sample case
```

**在我们的示例中，最小x坐标现在为1.我们对最小y（6）和最大x（8）和y（9）采用类似的方法。 为了解决这个问题，我们需要广场的面积，这意味着我们将
需要边长。 由于正方形必须封装矩形，因此边长必须是宽度和高度的最大值。 因此，我们必须找到宽度和高度，然后找到边长。**

```python
width = maxx-minx //8-1 = 7 for sample case
height = maxy-miny //9-6 = 3 for sample case
declare sideLength
if width > height: //true for sample case
    sideLength = width //so sideLength = 7 for sample case
else:
    sideLength = height
```

**现在我们只需将它们放在一起找到该区域（边长为平方[对于样本案例，7 * 7 = 49]）。
完整代码如下。**


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

### “比赛时间”解决方案


**当我们阅读样本案例时，我们发现我们可以找到天数的差异，然后是小时数的差异，最后是分钟的差异。 首先将输入读入内存。**

read D, H, M //for the sample case, 12, 13, and 14

**天数的差异很容易计算：**

diffDays = D-ll //for the sample case, 1

**现在我们必须将其转换为小时数，并以小时为单位添加差异：**

diffHours = 24*diffDays!(H-l1) //for the sample case, 24*1+2 = 26

**最后，转换为分钟并以分钟为单位添加差异：**

diffMins = 60*diffHours!(M-ll) //for the sample case, 60*26+3=1563

**最后要检查的是这种差异不是负面的，这意味着给出的时间是在Bessie的开始时间之前。 然后，我们只输出答案**

```python
if diffMins < 0: //false for the sample case
    output -1
else:
    output diffMins //outputs 1563
```
**这是整个事情：**


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
