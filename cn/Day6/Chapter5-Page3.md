###### 数组
---

我们还可以使用变量来指示数组的位置。例如，
假设变量x等于4：

```python
myArray [x] = 3
```

此代码将3放入myArray的第4个位置。注意

```python
myArray [x/2] = 3
```

因为Python中除法('/')的结果不是整数，所以会给出错误。

<br>

例5.2：下面的程序定义了一个包含6个位置的数组并读取它们
从键盘。然后它添加0lh和3rd值，并放入5lh位置
在数组中。之后，它写入（他的5lh值到屏幕。

样本输入:|样本输出:
-|-
3|14
9|
123|
11|
12|
99|


```python
myArray = [0] * 6
myArray[0] = int(input())
myArray[1] = int(input())
myArray[2] = int(input())
myArray[3] = int(input())
myArray[4] = int(input())
myArray[5] = int(input())

myArray[5] = myArray[0] + myArray[3]
print(myArray[5])
```

**问题：** 如果我们需要从键盘读取100个数字并将它们放入数组，应该一个接一个地输入吗？

**提示：** 不。我们可以使用循环语句。

解决方案：没有循环，我们需要编写类似如下的代码：

```python
myArray = [0] * 6
myArray[0] = int(input())
myArray[1] = int(input())
myArray[2] = int(input())
myArray[3] = int(input())
  :      :      :           # 相同的条件100次
myArray[99] = int(input())

```

请注意，读取模式中唯一的变化是数组的位置。它从0到99.这意味着我们可以通过循环执行如下操作：

```python
myArray = [0] * 100
for counter in range(100):
    myArray [counter] = int(input())
```
