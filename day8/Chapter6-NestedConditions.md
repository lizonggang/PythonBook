###### 嵌套条件
---

# <center>第6章: 嵌套条件</center>

例6.1 \每天早上10点，露西看着温度计和温度计

湿度计根据温度和温度决定吃什么或喝什么

湿度水平。下表显示了露西吃什么或喝什么

条件 - 例如，如果温度为45°F，则湿度为53％

露西吃蛋糕。

&nbsp;|温度 < 60°F |温度 > 60°F
-|-|-
湿度 < 40%|露西喝咖啡|露西喝冰茶
湿度 >= 40%|露西吃蛋糕|露西吃冰淇淋

编写一个程序，读取两个数字，温度和湿度，根据输入输出露西所做的事情到输出。

样本输入|样本输出
-|-
45 53|露西吃蛋糕


```python
temperature, humidity = input().split()
temperature = int(temperature)

if temperature < 60 and humidity < 40:
        print("露西喝咖啡")
if temperature < 60 and humidity >= 40:
        print("露西吃蛋糕")
if temperature >= 60 and humidity < 40:
        print("露西喝冰茶")
if tempecatuce >= 60 and humidity >= 40:
        print("露西吃冰淇淋")
```


前两个if具有共用条件，温度低于60°F。此外，最后两个if有另一个共享条件。我们可以把if分成两部分按照下图中的第一个条件分组。如果我们检查第一个条件我们将条件减少到四分之二。然后我们可以检查一下其他条件分开，并决定露西将采取的行动。


