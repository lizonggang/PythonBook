###### 循环
---

### 4.2. for循环

除了while循环，我们还有另一种循环类型; for循环。让我们输出包括1到30之间的偶数。我们使用while循环写程序如下：

```python
counter = 1                         # 从1开始
while counter <= 30：               # 循环直到30
    if counter % 2 == 0：           # 如果当前数字是偶数
        print(counter * counter)    # 输出它的平方
    counter = counter + 1           # 自增加
```


另一种循环类型是for循环。

```python
for循环的一般形式是：
    for counter in range(x, y):
        (表达式)
        (表达式)
        :  :  :        
```

counter循环开始等于x并在counter小于y时重复执行表达式。
上面的代码可以使用for循环编写如下：

```python
for counter in range(1, 31)：       # 从1开始，小于31结束
    if counter % 2 == 0:            # 如果当前数字是偶数
        print(counter * counter)    # 输出它的平方
```

请注意，循环计数器在每次运行表达式结束时更新循环。

如您所见，有时使用for循环更实际，因为它有一个循环计数器，它在每个回合结束时更新循环计数器。

我们可以以不同的方式使用range()。例如，

```python
for counter in range(31)：          # 从0开始，小于31结束
    if counter % 2 == 0：           # 如果当前数字是偶数
        print(counter * counter)    # 输出它的平方
```


当我们在range()中只有一个值时，计数器从0开始。

```python
for counter in range(8, 31, 2)：    # 从8开始，小于31结束，每次增加计数器2
    if counter % 2 == 0：           # 如果当前数字是偶数
        print(counter * counter)    # 输出它的平方
```

当我们在range()中有第三个值时，循环counter将递增通过第三个参数。

我们也可以使用range()中的变量代替数值。

