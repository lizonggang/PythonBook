###### 函数
---

练习11.5：编写一个程序，读取两个数字，> *和一个字符c
键盘。程序输出两个大小为x和y的正方形
人物角色

```
输入:                       输出:
3 5 #                       ###
                            ###
                            ###

                            #####
                            #####
                            #####
                            #####
                            #####
```

### 11.3. 本地/全局变量

函数中定义的变量只能在该函数中使用。看以下示例：

```python
def Power(x, y):
    z = 1
    for i in range (y):
        z *= x
    return z

x =int(input())
z = 11
print(Power(10, x))
print(z)
```

在此示例中，第1行中定义的变量y因此属于Power函数它不能在主函数中使用。变量x在第1行和第7行中定义。在第1行中定义x属于Power，而另一个属于主要代码。小心在第16行中，主代码中的x值变为Power中的变量函数，Power函数的x从第9行接收值10.类似地，z第8行属于主代码，它不受电源中z的影响功能。因此，第10行将为z的值输出'11'，因为它已初始化为第8行中的'11'。我们可以将主代码中的x和Power视为两个不同的两个不同房间的名字相同的盒子。 z同样如此。

练习11.6：如果用户输入，以下程序的输出是什么分别来自键盘的'I8cakes'和'try911'。

```python
def NumOfDigits(s, x)
    digits = 0
    for letter in s:
        if letter >= 101 and letter <= '9';
            digits += 1
    return digits + x
x=3
s = input()
t = input()
print(NumOfDigits(t, x + x))
```
