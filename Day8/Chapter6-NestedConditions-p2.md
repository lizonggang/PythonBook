###### 用python编程
---

![](http://legendary.cdn.play8.io/learnpython/img/day8/p1.png)

以下代码显示了我们如何比较两个条件其他。 这称为“嵌套if”。 在第一个'if 块'中，我们只考虑满足'temperature < 60'的条件。

```python
if temperature < 60:
    if humidity < 40:
        print("露西喝咖啡")
    else:
        print("露西吃蛋糕")
```

请注意，else对应于 'temperature < 60 adn humidity >= 40'。

> [!NOTE]
> 在上面的代码中，我们可能不使用括号，因为内部if块只是一个语句。

例子 6.2：使用嵌套在上一个练习中编写相同的程序。

方法：

```python
temperature, humidity = input().split()
temperature = int(temperature)
humidity = int(humidity)

if temperature < 60:
    if humidity < 40:
        print("露西喝咖啡")
    else:
        print("露西吃蛋糕")
else:
if humidity < 40:
        print("露西喝冰茶")
    else:
        print("露西吃冰淇淋")
```



