###### 变量 - 整数和浮点数
---

### 2.4. 从键盘读取数字
在Python中，我们可以从键盘读取数字，并使用 'input()' 将我们读取的数字放入变量框中。

例2.6：以下Python程序将从键盘读取的两个数字放入box1和box2。 然后它将box1和box2之和的一半放入box3，然后将box3写入屏幕。
```python
box1 = int(input())
box2 = int(input())
box3 = (box1 + box2) / 2
print(box3)
```

在上面的代码中，input() 读取一行键盘输入，in() 将其转换为整数。

> [!NOTE]
> 注意：注意要在行首输入每个整数 - 不要在一行中输入它们。否则代码将给出错误。


练习2.4：编写一个程序，从键盘读取两个数字，并将它们放入box1和box2。 然后它将box1和box2的乘法放入box3，并将box3写入屏幕。

我们也可以在从键盘读取输入时询问我们的问题，如下所示：

```python
age = int(input("please enter your age: "))
print("you will be", age + 40, "years old after 40 years")
```

例如，如果用户从键盘输入14，则输出如下（红色是用户输入）：

please enter your age: <font color=red>14</font> <br>
you will be 54 years old after 40 years

