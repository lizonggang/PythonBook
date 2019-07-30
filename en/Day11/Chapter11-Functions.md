###### 函数
---

# <center>第11章: 函数</center>
---


考虑一下芝士蛋糕工厂。提供奶酪，牛奶，面粉，糖等...工厂烘烤混合它们并且生产乳酪蛋糕。函数是像工厂一样;他们得到输入，做一些操作，并产生输出。

![blockchain](http://legendary.cdn.play8.io/learnpython/img/day11/d11-p1.png)

例如，假设我们有一个叫做power的函数。它接收两个值x和y,然后输出 $x^y$ 。我们可以使用值10和3调用函数，并将函数的返回值放在变量pow中，如下所示：

```python
pow = Power(10, 3)
```

这里，Power函数将返回 $10^3$ = 1000，并将此值放入pow变量中。我们可以编写包括Power函数在内的整个程序，如下所示：

```python
def Power(x, y):
    prod = 1
    por i in range(y):
        prod *= x
    return prod

pow = Power(10, 3)
print(pow)
```

该函数必须在其调用的代码之上定义。在这段代码中，Power函数在第1行和第5行之间定义。输入和输出类型，以及名称函数的定义在第1行中：它接收两个值x和y。我们写的在缩进的函数体中的操作;第2到第5行。它返回一个值如第5行所示。

