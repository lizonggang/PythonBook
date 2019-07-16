###### 循环
---

# <center>第4章: 循环</center>
---


### 4.1 while循环

练习4.1：编写一个程序，输出你的名字10次。

**问题：** 如果要求我们写100次会怎么样？我们应该写的同一行100次？

<table><tr><td bgcolor=#87CEFA>
while循环的一般格式是：

while 条件:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(表达式)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(表达式)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;...

while循环在满足条件时重复括号之间的表达式。
</td></tr></table>


例4.1：编写一个程序，输出从x + 1到x + 100的数字，从键盘输入x的值。

```python
x = int(input())            # 从键盘读取x
counter = 1                 # 设置默认计数器的值为1
while counter <= 100:       # 在计数器小于或等于100执行此循环   
    print(x + counter)
    counter = counter + 1   # 将计数器增加1

```

> [!NOTE]
> 注意：请注意第一步和最后一步。在上面的例子中，最初计数器是1.在最后一步，将x + 100写入屏幕后，计数器变为101并且违反了条件。

<br>
下表显示了计数器counter在每一步的输出和值。假设用户从键盘输入6。

步输|输出|计数器
-|-|-
Initial||1
1|7|2
2|8|3
:|:|:
:|:|:
99|105|100
100|106|101

