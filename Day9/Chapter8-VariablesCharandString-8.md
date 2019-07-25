###### 用Python编程
---

举个例子，

```python
x = int("12345")
```

> [!NOTE]
> 注意：int()函数的字符串参数必须是有效数字，否则它将是一个错误。


将数字转换为字符串也存在相反的功能。
例如，s = str(x)将数字x转换为字符串s。

 举个例子，

```python
s = str(12345)
```

将“12345”存储在字符串s中。

### 8.6. 字符串数组

请记住，我们声明了由整数值组成的数组：

```python
mylntArray = [0] * 10
```

声明一个包含10个整数的数组。同样，我们可以使用字符串声明数组值：

```python
myStrArray = [""] * 10
```

声明一个包含10个字符串的数组。我们可以读取和输出数组位置以同样的方式。

例8.6：读取输入中的整数n和n个单词并写入单词以相反的顺序。输入中最多有100个字符串。

```
样本输入                    样本输出
4                           About
Helloworld!                 TryIt!
Hello                       Hello
TryIt!                      HelloWrold!
About
```

解决方案：

```python
n = int(input())
words = [nn] * 100

# read n words from the input
for counter in range(n):
    words[counter 1 = input()

# write words on the screen in reverse order
for counter in range (n-1, -1, -1):
    print(words[counter])
```
