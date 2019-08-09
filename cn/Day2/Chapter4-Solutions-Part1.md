
问题1：例4.1

```python
x = int(input())            # 从键盘读取x
counter = 1                 # 最初计数器为1
while counter <= 100:       # 计数器小于或等于100执行此循环
    print(x + counter)
    counter = counter + 1   # 将计数器增加1
```

问题2：例4.2

```python
number = 1
while number != 0:          # 如果 number 不等于0，执行这个循环
    number = int(input())   # 从键盘读入 number
    if number > 5:          # 如果 number 大于5
        print(number)
```

问题3：例4.2

```python
number = int(input())       # 从键盘读入 number
counter = 0
while number != 0:          # 如果 number 不等于0，执行这个循环
    counter = counter + 1
    number = int(input())
print(counter)
```

问题4：例4.3

```python
x = int(input())            # 从键盘读取x数字
number = int(input())       # 第一次读取数字
while number != 0 :         # 而数字不等于0＃执行此循环
    if number > x:          # 如果数字大于x
        print(number)
    number = int(input())
```

问题5：例4.4

```python
n = int(input())
counter = 1
while counter <= n:
       print(counter)
       counter = counter + 1
```

问题6：例4.5

```python
n = int(input())                # 从键盘输入一个数字
counter = 0                     # 循环计数器
power = 1;                      # 初始化 power 等于1
while counter < n:              # 计数器小于 n ,执行循环
       power = power * 2        # 将当前 power 乘以2
       counter = counter + 1    # 计数器加1
print(power)
```


问题7：例4.6

```python
n = int(input())
counter = 0                     # 初始化counter为0
total = 0                       # 初始化 total 为0
while counter < n:              # 重复循环n次
       number = int(input())    # 读取 number
       total = total + number   # 将数字添加到总数中
       counter = counter + 1
 print(total)                   # 在循环后输出总数
```

问题8：例4.7

```python
number = int(input())
while number <= 35 and number >= 17 :
      print(number)
```

