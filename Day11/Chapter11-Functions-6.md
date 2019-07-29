###### 用python编程
---

主代码中定义的变量可从所有函数访问。对于
例如，

```python
def Power (x, y):
        global prod
        prod = 1
        for i in range (y):
            prod *= x

x = int(input())
Power(10, x)
print(prod)
```

prod在第2行中使用关键字 "global" 定义。这次，prod是一样的主代码和Power函数使用的代码。这些类型的变量被称为全局变量而其他变量是本地变量。请注意，如果我们不使用在第2行的定义中，Python会认为prod只属于Power函数并将在第9行给出错误。

> [!NOTE]
> 避免使用与本地变量相同的名称定义全局变量。这使代码更加混乱。

练习11.7：如果用户输入，以下程序的输出是什么分别来自键盘的'I8cakes'和'try911'。

```python
global y
y = 0

def NumOfDigits(s, x):
    digits = 0

    for letter in s:
        if letter >= 101 and letter <= 191:
            digits += 1
    return digits + x

x = 3
s = input()
t = input()
print(NumOfDigits(t, 19))
y = x * 2
```

> [!NOTE]
> 备注：最好尽可能多地定义局部变量。我们大多数当我们需要在许多函数中使用相同的变量时，定义全局变量。

<br>

**祝贺 - 达到了教训的结束** <br>
**做得好！**

