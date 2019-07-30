###### 变量 - 字符和字符串
---

在上面的代码中，我们写了字符串变量的名称然后是一个点和'len()'获得字符串的大小。上面的代码片段将在屏幕上写入"12"(包括空格和感叹号)。

例8.5：编写一个输出字符串中间字符的程序。如果它没有，在屏幕上输出'No middle character!'。

```
样本输入:           样本输出:
Trial               i
```

```
样本输入:           样本输出:
Helloworld          No middle character!
```

解决方案：

```python
s = input() 
# if the size of the string is
if len(s) % 2 == 0:
    print("No middle character!"|
else:
    middle = int(len(s)/2)
    print(s[middle])
```


练习8.3：编写程序从键盘读取一个字符串并写入在屏幕上反转它。

```
样本输入:           样本输出:
Trial               lairT
```

练习8.4：编写程序从键盘读取字符串和整数n并在屏幕上反复写入n次。

```
样本输入:           样本输出:
5                   lairT
                    lairT
                    lairT
                    lairT
                    lairT
```
