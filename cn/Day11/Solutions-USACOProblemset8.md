###“清道夫狩猎”解决方案
 
在样本输入中，分别为P和Q以及24和2。
P有8个因子：1,2,3,4,6,8,12,24
Q有2个因素：1,2
有2 * 8 = 16种可能的配对（按排序顺序）：

```
       1 1 
       1 2 
       2 1 
       2 2 
       3 1 
       3 2 
       4 1 
       4 2 
       6 1 
       6 2 
       8 1 
       8 2 
       12 1 
       12 2 
       24 1 
       24 2 
```

 
读入输入（P和Q位置）。 首先找到因子P和Q.这可以通过检查所有数字<= N来完成。在获得P和Q的因子后，找到所有对（i，j），使得i是P的因子，j是a Q的因素。请注意，此方法可确保根据问题的规范对输出进行排序。


```python
read P, Q 

array p_factors[] 
for i from 1 to P:  
    if P % i == 0 
        add i to p_factors 

array q_factors[] 
for j from 1 to Q: 
    if Q % j == 0 
        add j to q_factors         
for i in p_factors 
    for j in q_factors 
        print i, j 
```

还有另一个实现不涉及使用数组来存储P和Q的因子：

```python
read P, Q 
for i from 1 to P: 
    // if i is a factor of P 
    if P % i == 0: 
        for j from 1 to Q: 
            // if j is a factor of Q 
            if Q % j == 0: 
                print i, j 
```
 
---


<br>


                                                                              

### “幽闭恐惧症奶牛”的解决方案

 
目标是找到最近的一对奶牛。 距离定义为sqrt（xdifference ^ 2 + ydifference ^ 2）。 在样本测试数据中，最接近的一对奶牛是指数为7和9的奶牛，从问题陈述中给出的图表的快速目视检查可以看出这一点：

```
10 | . . . . . . . 3 . . . . . 
 9 | . 1 . . 2 . . . . . . . . 
 8 | . . . . . . . . . . . . . 
 7 | . . . . . . . . . . 4 . . 
 6 | . . . . . . 9 . . . . . . 
 5 | . 8 . . . . . . . . . . . 
 4 | . . . . . 7 . . . . . . . 
 3 | . . . . . . . . . 5 . . . 
 2 | . . . . . . . . . . . . . 
 1 | . . . . 6 . . . . . . . . 
 0 --------------------------- 
                       1 1 1 1 
   0 1 2 3 4 5 6 7 8 9 0 1 2 3 
```

使用嵌套for循环检查所有奶牛对; 每次找到较小的距离时更新存储的值。 确定具有最小距离的一对奶牛后，输出答案。
 
另外，请注意，乘法过程可能会溢出整数（使用long long或C ++中的某些内容）。 作为另一个实现提示，我们不需要平方根函数，因为我们不需要实际距离，但我们只是比较它们。 因此，比较两个数字的平方根与没有平方根的比较相同。

```python
read N 
array xcord[], ycord[] 
for i from 1 to N: 
    read xcord[i], ycord[i] 

// check the distance between all pairs 
minDist = very large number 
a = -1, b = -1 
for i from 1 to N: 
    for j from (i + 1) to N: 
        curDist = (xcord[i] - xcord[j])^2 + (ycord[i] - ycord[j])^2 
        if(curDist < minDist): 
            minDist = curDist 
            a = i, b = j 
print a, b 

```

