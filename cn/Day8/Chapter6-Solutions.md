## 第6章：参考答案

**问题1: 练习6.1**

```python
temperature, humidity = input().split()
temperature = int(temperature)
humidity = int(humidity)
if temperature < 60 and humidity < 40:
    print("露西喝咖啡")
elif temperature < 60 and humidity >= 40:
    print("露西吃蛋糕")
elif temperature >= 60 and humidity < 40:
    print("露西喝冰茶")
else :
    print("露西吃冰淇淋")
```

<br>

**问题2: 练习6.2**

```python
temperature, humidity = input().split()
temperature = int(temperature)
humidity = int(humidity)
if temperature < 60: # 由于t < 60，则有两种情况
    if humidity < 40: # t < 60 且 h < 40
        print("露西喝咖啡")
    else: # case2：t < 60 且 h > = 40
        print("露西吃蛋糕")
else: # 有两种情况，t >= 60
    if humidity < 40: # t >= 60 且 h < 40
        print("露西喝冰茶")
    else: #case2: t >= 60 且 h >= 40
        print("露西吃冰淇淋")
```

<br>

**问题3: 练习6.1**

```python
# 读取温度和湿度
t, h = input().split()
t = int (t)
h = int (h)
# h < 4 0的两个情况
if h < 40 :
    # h < 40 且 t < 60
    if t < 60 :
        print ("露西喝咖啡")
    # h < 40 且 t >= 60
    else :
        print ("露西喝冰茶")
else :
    # h >= 40 且 t < 60
    if t < 60 :
        print ("露西吃蛋糕")
    # h >= 40 且 t >= 60
    else :
        print ("露西吃蛋糕")
```

<br>

**问题4: 练习6.2**

```python
# 读取温度和湿度
t , h = input().split()
t = int (t)
h = int (h)
if t < 60 and h < 40 :
    print ("露西喝咖啡")
elif t < 60 and h < 60 :
    print ("露西打网球")
elif t < 60 and h >= 60 :
    print ("露西吃蛋糕")
elif t >= 60 and h < 40 :
    print ("露西喝冰茶")
elif t >= 60 and h < 60 :
    print ("露西打高尔夫")
else :
    print ("露西吃冰淇淋")
```

<br>

**问题5: 练习6.3**

```python
# 读取温度和湿度
t , h = input().split()
t = int (t)
h = int (h)
# t < 60 的两个情况
if t < 60 :
    # t < 60 并且 h < 40
    if h < 40 :
        print ( "露西喝咖啡")
    # t < 60 并且 40 <= h < 60
    elif h < 60 :
        print ( "露西打网球")
    # t < 60 并且 h >= 60
    else :
        print ( "露西吃蛋糕")
else :
# t >= 60 并且 h < 40
    if h < 40 :
        print ( "露西喝冰茶")
    # t >= 60 并且 40 <= h < 60
    elif h < 60 :
        print ( "露西打高尔夫")
    # t >= 60 并且 h >= 40
    else :
        print ( "露西吃蛋糕")
```

<br>

**问题6: 练习6.4**

```python
# 读取天数
d = int (input())
for i in range(d):
    # 读取温度和湿度
    t , h = input().split()
    t = int (t)
    h = int (h)
    if h>=40 and h < 60 :
        # 输出当天
        print ("Day",st「（i+l)+”："，end = " ")
        # t < 60 并且 40 <= h < 60
        if t < 60 :
            print ("露西打网球")
        # t >= 60 并且 40 <= h < 60
        else :
            print ("露西打高尔夫")
```

<br>

**问题7: 练习6.6**

```python
a, b, c = input().split()
a = int(a)
b = int(b)
c = int(c)
# 可能的b c情况
if a < b and b < c :
    print (str(a)+"\n"+str(b)+"\n"+str(c))
elif a < c and c < b :
    print (str(a)+"\n"+str(c)+"\n"+str(c))
elif b < a and a < c :
    print (str(b)+"\n"+str(a)+"\n"+str(c))
elif b < c and c < a :
    print (str(b)+"\n"+str(c)+"\n"+str(a))
elif c < a and a < b :
    print (str(c)+"\n"+str(a)+"\n"+str(b))
else :
    print (str(c)+"\n"+str(b)+"\n"+str(a))
# \n is for new line
```


替代方案：

```python
a,b,c = input().split()
a = int(a)
b = int(b)
c = int(c)
# 初始化顺序 a < b < c
mi = a # 使用“min”作为变量名
med = b
ma = c # 使用“max”作为变量名
# 如果 a > c  min和max
# a和c是有序的
if a > c :
    ma = a
    mi = c
# initial order: min < b < max
# 如果b是最小的（b <min <max）
# 更新最小值和中间值
if b < mi :
    med = mi
    mi = b
# 如果b是最大的（min <max <b）
# 更新最大值
elif b > ma :
    med = ma
    ma = b
print (mi)
print (med)
print (ma)
```

<br>

**问题8: 练习6.7\***

```python
a, b, c = input().split()
a = int(a)
b = int(b)
c = int(c)
# 可能的 a b c 排序
if a < b :
    # 的可能排序
    # a<b<c, a<c<b, c<a<b
    if b < c :
        print (str(a)+"\n"+str(b)+"\n"+str(c))
    elif a < c :
        print (str(a)+"\n"+str(c)+"\n"+str(b))
    else :
        print (str(c)+"\n"+str(a)+"\n"+str(b))
else :
    #b <a的3个可能的排序
    # b<a<c, b<c<aJc<b<a
    if a < c :
        print (str(b)+"\n"+str(a)+"\n"+str(c))
    elif b < c :
        print (str(b)+"\n"+str(c)+"\n"+str(a))
    else :
        print (str(c)+"\n"+str(b)+"\n"+str(a))
#\n 是换行符
```