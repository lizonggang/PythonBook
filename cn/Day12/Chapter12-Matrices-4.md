###### 用python编程
---

### 12.2. 矩阵初始化

可以在定义数组时初始化矩阵：

```python
matrix = [[1, 2, 2, 1], [4, 5, 5, 3], [2, 3, 5, 3]]
```


### 12.3. 矩阵作为迷宫的图形

矩阵可以用于不同的目的，而不仅仅是代表等数字迷宫和图表。

*练习12.4：

您将获得一个迷宫和路径的地图。检查是否路径是退出的正确方法。你将从那开始位置(1,1)，退出位于(1，m-1)。迷宫的一个例子尺寸(7,6)的尺寸如下。启动和退出位置显示为 'S' 和 'E'。路径显示为红色到出口。

![](http://legendary.cdn.play8.io/learnpython/img/day12/d12-p2.png)


```
样本输入：                  样本输出：
7 6                         Right path!
1 1 1 1 1 1
1 0 1 0 0 0
1 0 1 0 0 1
1 0 0 1 0 1
1 1 0 0 0 1
1 0 0 1 0 1
1 1 1 1 1 1
ddrdrruulurr
```

您将首先读取迷宫的大小(n, m)。然后迷宫将作为一个矩阵大小为(n，m); 1是墙，0是空位。矩阵的大小不会超过(100,100)。路径以四个字符串组成不同的字母;'l' 的意思是'左'，'r'的意思是"右"， 'u'的意思是"向上"，而 'd'的意思是 "向下"。

