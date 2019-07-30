###### 用python编程
---

以下代码也执行相同的操作。这个时间计数器从零开始。一旦循环开始，计数器counter就会递增1.因此，第一步 x + 1 输出在屏幕上。条件是计数器 counter < 100，因为循环当计数器达到100时必须结束。

```python
x = int(input())            # 从键盘选取x
counter = 0                 # 最初计数器为0
while counter < 100:        # 当counter小于100
    counter = counter + 1
    print(x + counter)
```

例4.2：写一个程序，则读取和输出，如果它大于5。

样本输入:|样本输出:
-|-
11|11
8|8
2|7
2|
4|
7|
5|
0|
<br>
解决方案：

```python
number = 1
while number != 0:              # number不等于1时，运行此循环
    number = int(input())       # 从键盘读取数字
        if number > 5:          # 如果数字大于5
            print(number)
```

<br>
练习4.2：编写一个程序，输出 **输入数字的次数**。当输入0时，程序将停止。

样本输入:|样本输出:
-|-
11|7
8|
2|
2|
4|
7|
5|
0|
