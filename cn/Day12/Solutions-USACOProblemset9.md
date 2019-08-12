###“作物圈”的解决方案
 
首先，我们需要读取所有输入并将其存储在数组中。

```python
read N 
array X[401], Y[401], R[401] 
for i from 1 to N: 
    read X[i], Y[i], R[i] 
```

问题告诉我们，我们需要为每头奶牛计算一些东西，这意味着我们将遍历它们并开始计算：

```python
for cow1 from 1 to N: 
    count = 0 
```

然后，我们需要计算重叠的奶牛数量。 我们将它转移到辅助函数，所以现在我们只说两条母牛i和j重叠，如果重叠（i，j）为真。 我们需要遍历所有的奶牛以检查它们是否重叠，然后如果它们那么添加到计数中。 请记住，牛不能与自身重叠！

```python
for cow2 from 1 to N: 
    if cow == cow2:                         // a cow can't overlap with itself 
        continue 
    if overlap(cow, cow2): 
        count += 1 
```

我们通过输出与之重叠的奶牛数来完成循环。 这是main函数的代码：

```python
read N 
array X[401], Y[401], R[401] 
for i from 1 to N: 
    read X[i], Y[i], R[i] 

for cow1 from 1 to N: 
    count = 0 
    for cow2 from 1 to N: 
        if cow1 == cow2:                  // a cow can't overlap with itself 
            continue 
        if overlap(cow, cow2): 
            count += 1 
    output count 
```
 
现在我们只需编写重叠函数。 我们将需要每头牛的X，Y和R，但只要我们确保全局声明这些数组，我们就可以从我们的函数中访问它们。
 
两头奶牛什么时候重叠？ 截止时应该是它们刚刚接触时，意味着它们的半径之和等于它们之间的距离，我们可以使用毕达哥拉斯定理来计算它们。 如果它们的半径之和更小，则它们不重叠; 否则，他们这样做。
 
我们也想避免毕达哥拉斯定理的平方根，所以我们将比较平方距离与半径平方和。 这是最终的重叠功能

```python
function overlap(i, j): 
    // Pythagorean Theorem 
    distSquared = (X[i]-X[j])^2 + (Y[i]-Y[j])^2 
    sumOfR = R[i] + R[j] 
    sumOfRSquared = sumOfR * sumOfR 
    if sumOfRSquared > distSquared: 
        return true 

    return false 
```

请注意，我们返回false而没有else子句。 这是因为如果if语句运行，它下面的代码永远不会，所以else子句不是必需的。 通常，这是更好的做法，因为它确保函数将返回一些东西。

---

<br>


                                                                              

###“牛骨头”解决方案
 
在样本输入中，有3个骰子，3个，2个和3个边，所有可能的结果如下所示：

```
1 1 1 -> 3  1 2 1 -> 4  2 1 1 -> 4  2 2 1 -> 5  3 1 1 -> 5  3 2 1 -> 6 
1 1 2 -> 4  1 2 2 -> 5  2 1 2 -> 5  2 2 2 -> 6  3 1 2 -> 6  3 2 2 -> 7 
1 1 3 -> 5  1 2 3 -> 6  2 1 3 -> 6  2 2 3 -> 7  3 1 3 -> 7  3 2 3 -> 8 
```

下表显示了可能的总和是它们的出现次数

sums|3|4|5|6|7|8 
-|-|-|-|-|-|-
occurrence|1|3|5|5|3|1 
 
5和6都出现最频繁 -  5次。 由于问题是要求最小的整数和，在这种情况下，当出现平局时，选择5作为答案。
 
为了确定最常出现的总和，我们考虑骰子可以着陆的每个等概率案例。 为此，我们循环第一个骰子的可能值，第二个骰子的值和第三个骰子的值。 在三个循环中，我们计算总和并记下它在数组中的出现。 然后，我们扫描数组，查找出现次数最多的总和。

```python
read S1 S2 S3 

for i from 1 to S1: 
    for j from 1 to S2: 
        for k from 1 to S3: 
            cSum = i + j + k 
            count[cSum] += 1 

mostFrequent = 0 

for i from 1 to S1 + S2 + S3: 
    if count[i] > count[mostFrequent]  
        mostFrequent = i 

print mostFrequent 
```

**替代解决方案：**或者，我们可以首先循环总和。 然后我们可以遍历骰子的组合并计算该总和中有多少结果。 我们会跟踪哪个总和最有可能加起来这个数字。
 

```python                                                                 
read S1 S2 S3 

mFSum = 0           // sum of maximum frequency 
mFFreq = 0          // maximum frequency 

// loop through all possible sums 
for cSum from 3 to S1 + S2 + S3: 
    cFreq = 0 
    // check all possible rolls 
    for i from 1 to S1: 
        for j from 1 to S2: 
            for k from 1 to S3: 
                if i + j + k == cSum: 
                    cFreq += 1 
    // update the maximum frequency 
    if cFreq > mFFreq 
        mFSum = cSum 
        mFFreq = cFreq 

print mFSum 
```

