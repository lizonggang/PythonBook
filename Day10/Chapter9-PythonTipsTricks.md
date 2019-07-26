# <center>第9章: Python技巧</center>
---

### 9.1. 表达式和算术运算

在Java中，我们可以使用 '\'终止一长行。例如，将长行分成多行以下代码相同：

```python
print("There are "+ secondsInADay + " seconds in one day.")
```


```python
print("There are "+ secondsInADay + str(secondsInADay) \
      + " seconds in one day.")
```

有一些快捷操作代替了一些算术运算。他们如下表所示：

运算符|例子|等效表达式
-|-|-
+=|number += 10|number = number + 10
-=|number -= 10|number = number - 10
*=|number *= 10|number = number * 10
/=|number /= 10|number = number / 10

> [!INFO]
> 小心不要将变量或数字除以零否则程序将失败。

<br>

### 9.2. 循环

有时我们需要根据中间的条件退出循环操作。那时，我们使用 'break' 命令如下：

```python
number = int(input())
for counter in range(20):
    isEven = number % 2
    if isEven == 0:
        square = number * number
        print(square)
    if number % 11 == 0：
        break
    number += 1
```

在这里，如果数字可以被11整除，我们就会停止循环。

