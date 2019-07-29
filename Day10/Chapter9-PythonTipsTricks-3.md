###### python技巧

```python
print(number)
```

同样，我们可以通过输出检查除数的计算是否正确第9行后数组中的值如下：

```python
for counter in range(index):
    print(divisors[counter])
```

我们会立即注意到，因为除数数组中的值是错误的。所以我们仔细检查除数计算并查看错误
第7行。

```python
divisors[index] == divisor
```

在下一步运行后，我们将看到数字本身就是其除数之一。然后我们将再次检查for循环，并找出范围是错误的它必须是最多的number：

```python
for divisor in range(2, number + 1):
```

纠正错误后我们会再次检查。接下来是调试步骤第14行：

```python
print(sum)
```

我们将看到总和不正确，并注意for循环中的错误：

```python
sum = divisors[counter]
```

它必须是 "+=" 代替"="最后，程序将产生所需的输出。

> [!INFO]
> 一些常见错误可以列举如下：
> - 循环计数器的初始化/范围错误
> - 使用“==”而不是“=”
> - 具有导致不希望的输出或无限循环的条件的简单错误
> - 错误更新循环计数器

永远记住代码可能没有语法错误;它可能不起作用适当地创建所需的输出。换句话说，您的代码可能会编译但是它可能同时存在一些逻辑错误。在那种情况下，它是建议你添加''print'并在可疑内打印变量的值循环和条件来跟踪变量的变化。此外，您可以添加一些注释像 print("This is the 1st condition and I am here")这样你就可以确定编译器是否执行了那个特定的if条件。


**祝贺 - 达到了教训的结束** <br>
**做得好！**
