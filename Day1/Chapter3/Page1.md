# <center>第3章: 条件</center>
---

###　3.1. if 语句

假设凯蒂说 “如果下雨，我会用我的雨伞”。
同样，我们可以在Python中使用条件语句。
例如，我们可以设置如下条件：
&nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; 如果x大于5，则写'x大于5'
例3.1：编写一个从键盘读取数字并写入的程序
如果给定的数字大于5，则输出'x大于5'。
```python
x = int(input())
if x > 5:
    print("x is greater than 5")
```
<table><tr><td bgcolor=#87CEFA>注意：以print开头的行是缩进的（通常有4个空格或制表符）。<br>
如果没有缩进，那将是一个错误。
</td></tr></table>


### 3.2. if - else

假设泰勒说 “如果下雨，我会用我的雨伞，否则我会戴上太阳镜”。

同样，在我们程序的条件语句中，我们可以告诉计算机
如果条件是假的，该怎么办。

例如，
&nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; 如果x大于5，则写 'x大于5'，否则写 'x不大于5'。


例3.2：编写一个从键盘读取数字并写入的程序
如果给定的数字大于5，则输出 'x大于5'。否则，输出 'x不大于5'。

```python
x =  int(input())
if x > 5:             # if x is greater than 5
    print  ("x is greater than 5")

else:                 # otherwise
    print  ("x is not greater than 5")
```


