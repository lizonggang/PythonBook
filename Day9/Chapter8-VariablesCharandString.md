###### 变量 - 字符和字符串
---
# <center>第8章：变量 - 字符和字符串</center>
  
### 8.1. 介绍

字符串变量可以包含任何字符，如字母和数字。例如，你可以把'John'放在一个字符串变量中，但不能放在整数变量中。字符串赋值与整数变量相同：

```python
myVariable = "John"
```

把'约翰'放在我的变量中。

> [NOTE]
> 我们可以在John之前和之后使用单引号（'）或双引号（"）。

例8.1：编写一个程序，从键盘上读取你的名字并打印出来。如果名字是'John'那么它在屏幕上5次为'你的名字是约翰'。

```
样本输入                        样本输出      
 John                        你的名字是约翰。
                             你的名字是约翰。
                             你的名字是约翰。
                             你的名字是约翰。
                             你的名字是约翰。
```

解决方案：

```python
name = input()
for counter in range(5):
    print("Your name is " + name + ".")
```

在字符串中，'+表示连接它们。

例如，

```python
firstname = "John"
lastname = "Doe"
fullname = firstname + " " + lastname
print(fullname)
```

输出变成

```John Doe
```

请注意，我们在firstname和lastname之间添加了一个空格。
