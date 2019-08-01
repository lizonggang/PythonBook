## Chapter 6: Solutions
This page contains the solutions except the optional ones:

**Question 1: Example 6.1**

```python
temperature, humidity = input().split()
temperature = int(temperature)
humidity = int(humidity)
if temperature < 60 and humidity < 40:
    print("Lucy drinks coffee")
elif temperature < 60 and humidity >= 40:
    print("Lucy eats cake")
elif temperature >= 60 and humidity < 40:
    print("Lucy drinks iced tea")
else:
    print("Lucy eats ice cream")
```

<br>

**Question 2: Example 6.2**

```python
temperature, humidity = input().split()
temperature = int(temperature)
humidity = int(humidity)
if temperature < 60: # there are two cases for t<60
    if humidity < 40: # easel: t<60 and h<40
        print("Lucy drinks coffee")
    else: # case2: t<60 and h>=40
        print("Lucy eats cake")
else: # similarlay there are two cases for t>=60
    if humidity < 40: # t >= 60 and h < 40
        print("Lucy drinks iced tea")
    else: #case2: t >= 60 and h >= 40
        print("Lucy eats ice cream")
```

<br>

**Question 3: Example 6.1**

```python
# read temperature and humidity
t, h = input().split()
t = int (t)
h = int (h)
# two cases for h < 40
if h < 40 :
    # h < 40 and t < 60
    if t < 60 :
        print ("Lucy drinks coffee")
    # h < 40 and t >= 60
    else:
        print ("Lucy drinks iced tea")
else:
    # h >= 40 and t < 60
    if t < 60 :
        print ("Lucy eats cake")
    # h >= 40 and t >= 60
    else:
        print ("Lucy eats cake")
```

<br>

**Question 4: Example 6.2**

```python
# read temperature and humidity
t , h = input().split()
t = int (t)
h = int (h)
if t < 60 and h < 40 :
    print ("Lucy drinks coffee")
elif t < 60 and h < 60 :
    print ("Lucy plays tennis")
elif t < 60 and h >= 60 :
    print ("Lucy eats cake")
elif t >= 60 and h < 40 :
    print ("Lucy drinks iced tea")
elif t >= 60 and h < 60 :
    print ("Lucy plays golf")
else:
    print ("Lucy eats ice cream")
```

<br>

**Question 5: Example 6.3**

```python
# read temperature and humidity
t , h = input().split()
t = int (t)
h = int (h)
# two cases for t < 60
if t < 60 :
    # t < 60 and h < 40
    if h < 40 :
        print ( "Lucy drinks coffee")
    # t < 60 and 40 <= h < 60
    elif h < 60 :
        print ( "Lucy plays tennis")
    # t < 60 and h >= 60
    else:
        print ( "Lucy eats cake")
else:
# t >= 60 and h < 40
    if h < 40 :
        print ( "Lucy drinks iced tea")
    # t >= 60 and 40 <= h < 60
    elif h < 60 :
        print ( "Lucy plays golf")
    # t >= 60 and h >= 40
    else:
        print ( "Lucy eats cake")
```

<br>

**Question 6: Example 6.4**

```python
# read number of days
d = int (input())
for i in range(d):
    # read temperature and humidity
    t , h = input().split()
    t = int (t)
    h = int (h)
    if h>=40 and h < 60 :
        # output the day
        print ("Day",st「（i+l)+”："，end = " ")
        # t < 60 and 40 <= h < 60
        if t < 60 :
            print ("Lucy plays tennis")
        # t >= 60 and 40 <= h < 60
        else:
            print ("Lucy plays golf")
```

<br>

**Question 7: Example 6.6**

```python
a, b, c = input().split()
a = int(a)
b = int(b)
c = int(c)
# possible cases for a b c ordering
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
else:
    print (str(c)+"\n"+str(b)+"\n"+str(a))
# \n is for new line
```


Alternative solution:

```python
a,b,c = input().split()
a = int(a)
b = int(b)
c = int(c)
# initial order a < b < c
mi = a # avoid using "min" as variable name
med = b
ma = c # avoid using "max" as variable name
# swap min and max
# a and c are ordered
if a > c :
    ma = a
    mi = c
# initial order: min < b < max
# if b is the smallest (b < min < max)
# update min and med
if b < mi :
    med = mi
    mi = b
# if b is the largest (min < max < b)
# update med and max
elif b > ma :
    med = ma
    ma = b
print (mi)
print (med)
print (ma)
```

<br>

**Question 8: Example 6.7\***

```python
a, b, c = input().split()
a = int(a)
b = int(b)
c = int(c)
# 6 possible cases for a b c ordering
if a < b :
    # 3 possible orderings for a < b:
    # a<b<c, a<c<b, c<a<b
    if b < c :
        print (str(a)+"\n"+str(b)+"\n"+str(c))
    elif a < c :
        print (str(a)+"\n"+str(c)+"\n"+str(b))
    else:
        print (str(c)+"\n"+str(a)+"\n"+str(b))
else:
    # 3 possible orderings for b < a
    # b<a<c, b<c<aJc<b<a
    if a < c :
        print (str(b)+"\n"+str(a)+"\n"+str(c))
    elif b < c :
        print (str(b)+"\n"+str(c)+"\n"+str(a))
    else:
        print (str(c)+"\n"+str(b)+"\n"+str(a))
#\n is for new line
```

