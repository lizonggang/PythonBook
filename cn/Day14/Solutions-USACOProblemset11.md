###“机器人犁”解决方案
 
在样本输入中，来自（1,1） - （2,4）和（1,3） - （5,4）的所有正方形都已被耕作。 在第一条指令中，犁了8个方格。 在第二条指令中，犁了10个方格。 然而，耕地的总数是14，因为区域（1,1） - （2,4）和（1,3） - （5,4）具有重叠区域（1,3） - （2,4） ）4号的实际平方数是14。
 
模拟问题。 跟踪犁过的和不犁的东西（所有方块最初都是未开槽的）。 然后，最后，循环遍历矩阵并计算犁过的方块。 我们使用1索引来对应问题陈述。
 
最初，将矩阵的所有条目设置为false，以指示土地未开挖。

```python
read X, Y, I 
array plowed[241][241] 
for x from 1 to X: 
    for y from 1 to Y: 
        plowed[x][y] = false 
```

迭代所有耕作指令并将正方形标记为真

```python
for i from 1 to I: 
    read Xll, Yll, Xur, Yur 
    for x from Xll to Xur: 
        for y from Yll to Yur: 
            plowed[x][y] = true 
```

处理完所有耕作指令后，计算已标记为真的正方形数（耕）

```python
count := 0 
for x from 1 to X: 
    for y from 1 to Y: 
        if plowed[x][y]: 
            count += 1 
output count 
```

---

<br>


###“Parkside三角”的解决方案

 
我们来看一个示例案例：
``5 3``
 
在这种情况下，我们必须从数字3开始，并创建5个级别，其中数字按递增顺序mod 9.增加的数字首先垂直放置然后水平放置，如下所示：

```
3 4 6 9 4 
  5 7 1 5 
    8 2 6 
      3 7 
        8 
```

在我们的解决方案中，我们必须模拟此过程并创建一个如下所示的数组：

```
3 4 6 9 4 
0 5 7 1 5 
0 0 8 2 6 
0 0 0 3 7 
0 0 0 0 8 
```

然后，我们打印数组，同时用空格替换所有0。 要创建此数组，我们在第一列中放置1个数字，然后在第二列中放置两个数字，在第n列中放置n个数字。 我们放下的每个数字都比前一个数字大一个，除了我们采用每个数字mod 9（9本身除外）因为我们只想要数字1-9。
 
```python
read n,s 
array[n][n] 
for i from 0 through n-1: 
    for j from 0 through i: 
        array[j][i] = s 
        s = (s+1) mod 9 
        if array[j][i]= 0: 
            array[j][i] = 9 

for i from 0 through n-1: 
    for j from 0 through n-1: 
        if array[i][j] > 0: 
            print array[i][j], " " 
        else:  
            print "  " 
    print to new line 
```

