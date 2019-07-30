
另一方面，我们可以使用变量调用函数。例如，以下程序将 $10^z$ 的值写入从中读取z的屏幕
键盘。

```python
def Power(x, y)：
    prod = 1
    for i in range(y):
        prod *= x
    return prod

z = int(input())
pow =Power(10, z)
print(pow)
```

在上面的程序中，实例化后输出。

```python
pow = Power(10, z)
print(pow)
```

我们可以直接输出，

```python
print(Power(10, z))
```

没有定义变量pow。

我们也可以用表达式调用函数。例如，以下内容程序将值 10<sup>z * t + 2</sup> 输出屏幕，其中z和t从中读取键盘。


```python
def Power(x, y):
    prod = 1
    for i in range(y):
        prod *= x
    return prod

z = int(input())
t = int(input())
print(Power(10, z * t + 2))
```

在函数'return'命令，立即返回指定的值，并且函数中的其余代码不执行。例如，下面的Power功能如果y(指数)的值是负数，则立即返回0。

```python
def Power (x, y):
    if y < Ot
        return 0

    prod = 1
    for i in range(y):
        prod *= x
    return prod
```
