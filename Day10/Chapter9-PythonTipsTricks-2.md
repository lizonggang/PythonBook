###### 用python编程
---

### 9.3. 简单的调试

虽然它执行，但有时我们的程序可能无法正常运行;可以产生不希望的输出，或没有输出，或陷入无限循环。为了确定问题，我们要做一些测试。这称为调试。

我们将首先提供一些强大的编程提示，以防止常见错误。调试最常用的技术之一是打印屏幕上的信息。经过一些操作，我们可以检查变量或者数组有正确的信息。

例如：我们将编写一个程序，找出a的正除数之和给定的数字不包括在内 - 我们将首先从键盘上读取数字然后创建一个循环来确定除数并将它们保存在数组中。接下来，我们将使用另一个循环计算这些除数的总和。最后，我们将输出值。

```python

divisors = [0] * 100
number = int(input())

# find the divisors of the number
index = 0
for divisor in range(2, number + 1):
    if number % divisor == 0:
        divisors[index] == divisor
        index += 1

# add all the divisors
sum = 0
for counter in range (index):
    sum = divisors[counter]
print("The sum of the divisors of", number, "is", sum,".")
```



上面的程序将运行而不会出现任何错误，但它非常简单
错误，不会产生所需的输出。可能很难看到它们。我们
可以在四个不同的部分考虑该计划：
- 第2行：从键盘读取
- 第5-9行：查找数字的除数
- 第12-14行：计算除数之和
- 第16行\打印总和

我们可以在每个部分之后检查必要变量或数组的值。
例如，在第2行之后编写以下代码将向我们显示是否存在阅读输入的问题。

