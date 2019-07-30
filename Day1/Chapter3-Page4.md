###### 用python编程
---

考虑以下条件语句：

        如果x大于5或小于10，则输出'x小于4'，否则输出'x大于15'。

例3.4：编输出一个从键盘读取数字并输出入的程序如果给定的数字大于5或小于10，则输出'x小于4'。否则输出 'x大于15'.
```python
x = int(input())  # read x from keyboard

if x > 5 or x < ID:  # if x is greater than 5 or less than 10
    print("x is less than 4")
else:
    print("x is greater than 15")
```

练习3.4：编输出一个程序，从键盘读取数字并输出如果给定的数字大于10且不等于15，输出 'I like it'。否则输出 'I didn't like it'。


练习3.5：在以下程序中，在屏幕上看到 “x is greater 15” 用户必须输入的号码是什么？
```python
x = int(input())
if x == 5 or x < 10:
    print("x is less than 4")
else:
    print("x is greater than 15")
```

如果条件为**真**或**假**，则还可以有多个表达式。

例3.5：假设给定一个数字x，如果x小于10，我们将输出'small'和 x乘以2的结果。否则，在屏幕上输出'large' 和x除以2的结果。
```python
if x < 10:
    print("small")
    x = x * 2
else:
    print ("large")
    x = x / 2
```
在这里，我们以缩进的形式编输出表达式块，如前所述。

