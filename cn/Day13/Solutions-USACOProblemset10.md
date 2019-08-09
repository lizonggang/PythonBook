###“奶牛计数”的解决方案

在介绍解决方案之前，我将介绍问题中的示例案例：
10 1
 
在这种情况下，我们必须打印前10个不包含1的数字中最大的数字。为此，我们遍历正整数，用1跳过整数并总共输入10个数字。 最后，我们打印出这10个数字中最大的一个并得到：
22

现在，我们必须将这个解决方案概括为跳过数字``L``的``N``数字。首先，我们创建一个方法来识别给定数字，``a``是否包含数字``L``。 这个名为``seen``的方法使用mod 10检查数字的最后一位是否为“L`”，然后使用整数除法删除最后一位数。 这样，它可以检查数字中的任何数字是否为“L”。

```python
seen(a, L): 
    while a > 0: 
        if a % 10 == L: 
            return true 
        a = a/10 
    return false
```

实现此方法的另一种方法是使用字符串并遍历字符串并检查它是否包含字符“L`”：

```python
seen(a, L): 
    a = string of a 
    L = character of L 
    for i from 0 through n-1 
        if a[i] = L: 
            return true 
    return false 
```

接下来，我们构建实际打印答案的主要方法。 main方法总共跳过``n``整数，同时跳过包含``L``的整数。 最大的整数存储在``counter``中，并且在找到总共不包含`````的``n``整数后打印出来。
       ​                    
```python
counter = 1 
read n, L 
for i from 1 through n: 
    while seen(counter, L): 
        counter = counter + 1 
 
    counter = counter + 1  
 
print counter         
```

---

<br>

 

### “开关灯”解决方案
 
我们需要保持所有灯的状态并实现所请求的操作。 我们将使用false来表示关闭的灯光，并使用true来表示正在亮起的灯光。 首先，让我们为它设置一个布尔数组
点亮并读取灯的数量和操作。

```python
read N, M 
array lights[501] 

//set the lights to all be off 
for i from 1 to N: 
    lights_i = false 
```

现在我们需要读取输入并进行处理。

```python
for i from 1 to M: 
    read instruction, s, e 
```

在第一种情况下，我们需要切换每个灯，所以我们应该遍历它们：

```python
if instruction == 0: 
    for light from s to e: 
```

要切换灯光，我们需要将其设置为已经处于相反的状态，这可以通过二进制NOT（！）操作来完成。

```python
lights_light = not lights_light 
```

在另一种情况下，我们再次需要迭代，这次保持所有灯的计数。 然后我们需要输出我们的计数。

```python
if instruction == 1: 
    count = 0 
    for light from s to e: 
        if(lights_light)           // this will be true if the light is on 
            count = count + 1 
    output count 
```

我们将这些全部放在一起以获得最终解决方案：

```python
read N, M 
array lights[501] 


for i from 1 to N: 
    lights_i = false 

for i from 1 to M: 
    read instruction, s, e 
    if instruction == 0: 
        for light from s to e: 
            lights_light = not lights_light 
    if instruction == 1: 
        count = 0 
        for light from s to e: 
            if(lights_light) 
                count = count + 1 
        output count 
```



