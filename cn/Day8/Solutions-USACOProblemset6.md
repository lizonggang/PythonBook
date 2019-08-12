###“完美广场”的解决方案


在样本输入中，（a，b）有2个解，使得a ^ 2  -  b ^ 2 = 15：
(4, 1): 16-1 = 15
(8, 7): 64-49 = 15

读入输入，这是两个方格（N）的差异。 检查a和b的所有可能组合，使aA2-bA2 = N.如果找到满意的对，则将计数增加1.最后，打印总对数。

```python
read N
answer = 0
for b from 1 to 500:
    for a from b + 1 to 500
        if a * a - b * b == N
            answer = answer + 1

output answer
```

不是使用嵌套循环来检查a和b的所有组合，而是可以使用一个循环来枚举a的值并构造b的可能值。

```python
read N
answer = 0
for a from 1 to 500
    if isPerfectSquare(a * a - N)
        answer = answer + 1

output answer
```

例如，当a = 4时，可以通过检查b是否是整数来计算b的可能值，b = sqrt（a A 2 -N）= sqrt（16-15）。 值1是完美的正方形，因此可以获得b并且答案递增1。

我们用不同的方式检查一个数字是否是一个完美的正方形。 完美数字的根必须是整数。 一个简单的实现如下：

```python
function isPerfectSquare(X):
    Y = int(sqrt(X))
    if Y ^ 2 == X:
        return true
    else
        return false
```

**解决这个问题的另一种解决方案是优雅地找到N的除数。** 由于N = aA2-bA2，因此可以将其重写为N =（a + b）*（a-b）。 对于每对除数，使得p * q = N且p> = q，求解
系统（a + b = p，a  -  b = q） - >（a =（p + q）/ 2）。 如果a是整数（p + q可被2整除）则存在满足问题陈述中所述条件的对（a，b）。

在样本情况下，N = 15.一个可能的因子分解是p = 5和q = 3; 在这种情况下，a可以求解为（3 + 5）/ 2 = 4; 然后，这是1.这与上述解决方案一致。

```python
read N
answer = 0
for i from 1 to sqrt(N):
    // if i and (N/i) is the divisor pair and
    //if (i + N / i) is divisible by 2
    // Note that always i <= (N / i)
    if N % i == 0 and (i + N / i) % 2 == 0:
        answer = answer + 1
```

---

<br>



### “车轮旋转”解决方案

在样品测试盒中，皮带轮1通过直带连接到皮带轮2，因此皮带轮2的方向与皮带轮1的方向相同（顺时针方向）。 皮带轮3通过直带连接到皮带轮2，因此它也是顺时针方向。 皮带轮4通过交叉皮带连接到皮带轮3，因此它与皮带轮3的方向相反，这使其逆时针（1）。

**一个简单的想法如下：**将带信息存储在数组中。 从第一个滑轮开始，使用嵌套环找到驱动下一个滑轮的皮带。 然后确定下一个滑轮的方向。 重复，直到确定最后一个滑轮的方向。

```python
read N
numCross = 0
for i from 1 to N-l:
    read s[i] d[i] c[i]

eDir = 0
for i from 1 to N-l:
    for j from 1 to N-l:
        if s[j] == i:
            if c[j] == 1:
                if eDir = 1:
                    eDir = 0
                else :
                    eDir = 1
print eDir
```

**替代解决方案：**

在之前的解决方案中，我们不需要搜索滑轮，因为它从1到N.我们只需要将滑轮方向信息存储在从1到N的滑轮阵列中。然后我们可以确定滑轮的旋转方向。 每个滑轮从一开始。

```python
read N
numCross = 0
for i from 1 to N-l:
    read s d c
    type[s] = c

eDir = 0
for i from 1 to N-l:
    if type[i] == 1:
        if eDir = 0:
            eDir = 1
        else:
            eDir = 0
print eDir
```

**替代解决方案：**

这是一个很好的观察：实际上滑轮的顺序无关紧要。

如果两个皮带轮通过直带连接，则从动皮带轮的旋转方向与驱动皮带轮相同。 但是，如果两个滑轮通过交叉皮带连接，则驱动的旋转方向
滑轮与驱动滑轮相反。 因此，我们可以计算交叉滑轮的数量来计算方向翻转的次数。 如果数量是偶数，则最终滑轮的方向将与第一滑轮的方向相同。 如果数字是奇数，则最终滑轮的方向将与最后一个滑轮的方向相反。 请注意，滑轮的顺序无关紧要。
```python
read N
numCross = 0
for i from 1 to N-l:
    read s d c
    if c == 1:
        numCross += 1

if numCross is divisible by 2:
    print 0
else :
    print 1
```
