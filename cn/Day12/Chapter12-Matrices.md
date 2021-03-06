###### 矩阵
---

# <center>第12章: 矩阵</center>
---


## 12.1. 介绍

当我们去邮局时，我们看到邮箱排成行和列。每个邮箱都有邮件，并带有一个号码。邮箱也可以在不使用这些数字的情况下描述。如果我们引用一行和一行列它将对应一个邮箱。如果我们要求我们的朋友找到邮箱在第3行和5列，他或她将很容易找到它。就像邮件一样邮局中的盒子，矩阵由盒子组成行和列号。

![](http://legendary.cdn.play8.io/learnpython/img/day12/d12-p1.png)

上面的矩阵A有3行4列，所以它有12个带数字的方框在他们中。在上面的矩阵中，引用位置是第1行第2列。

> [!NOTE]
> 我注意到，就像在数组中一样，索引从0开始。

我们可以按如下方式定义和初始化矩阵：

```python
myMatrix = [0] * n
for i in range (n):
    myMatrix[i] = [0] * m
```

定义一个名为'myMatrix'的矩阵，包含3行和4列。它类似于阵列;另外矩阵有二维，因此我们需要再添加一个定义时的括号。上面的代码用零初始化矩阵。

我们可以以与我们相同的方式读取和写入矩阵位置阵列。例如，

```python
print(myMatrix[1][2])
```

输出位置(1, 2) - 第1行，第2列的值 - 而

```python
myMatrix [l] [2] = 100
```

将值 "100" 放在同一位置。


