###### 用python编程
---

例如，在python中，'Mybox = 4' 并不意味着 'Mybox 和 4 相等'; 这意味着'将4放入Mybox'。
我们也可以将十进制数放入变量中。例如，
```python
Mybox = 4.78
```

将4.78放入Mybox。如果我们想将小数作为整数，我们按如下方式进行：
```python
number = 4.78
Mybox = int(number)
```
这里，int() 只是通过取数字的整数部分来转换十进制数。Mybox中的值变为4。

### 2.2. 将变量中的数字写入屏幕
示例2.2：考虑以下示例。
```python
nicebox = 10
```

**问题：** 当您运行该程序时，您在屏幕上看不到任何内容。为什么？

假设我们想把'nicebox'中的钱写到屏幕上。
打开一个新文件，编写下面的代码，将其命名为nicebox2.py，将其保存到桌面并运行它。

```python
nicebox = 10
print(nicebox)
```

**问题：** 运行程序时，您在屏幕上看到了什么？



练习2.1：运行下面的程序后，您会在屏幕上看到什么？
```python
nicebox = 10.3
nicebox = 7.51
print(nicebox)
```
练习2.2：运行下面的程序后，您会在屏幕上看到什么？
```python
nicebox = 123
anotherbox = 21.186
print(nicebox)
print(anotherbox)
```

我们可以用print输出多个表达式。例如，


