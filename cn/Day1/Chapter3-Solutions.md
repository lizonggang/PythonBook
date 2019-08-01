##### 问题1：练习3.1
```python
x = int(input()) #  从键盘读出一个数
if x > 5:   # 如果 x大于5 成立
    print('x大于5')
```

##### 问题2：练习3.2
```python
x = int(input())
if x > 5:
    print('x大于5')
else:
    print('x不大于5')
```
##### 问题3：练习3.3
```python
x = int(input())
y = int(input())
if x > y:
    print(x)
else:
    print(y)
```
##### 问题4：练习3.4
```python
number = int(input())
if number % 6 == 3:
    print(number)
number = int(input())
if number % 6 == 3:
    print(number)
number = int(input())
if number % 6 == 3:
    print(number)
```
##### 问题5：练习3.5
```python
x = int(input())
if x > 5 and x < 10:
    print('x小于4')
```
##### 问题6：练习3.6
```python
x = int(input())
if x > 5 or x < 10:
    print('x小于4')
else:
    print('x大于15')
```
##### 问题7：练习3.7
```python
x = int(input())
if x > 10 and x != 15:
    print('我喜欢它')
else:
    print('我不喜欢它')
```
##### 问题8：练习3.8
```python
score =- int(input())
if score < 50:
    print('not good')
elif score >= 50 and score < 70:
    print('fair')
elif score >= 70 and score < 90:
    print('good')
else:
    print('awesome')
```
##### 问题9：练习3.9
```python
x = int(input())
if x % 2 == 0:
    print('这是一个偶数')
else:
    print('这是一个奇数')
```
##### 问题10：练习3.10
```python
a = int(input())
b = int(input())
c = int(input())
if a <= b and a <= c:
    print(a)
elif b <= a and b <= c:
    print(b)
elif c <= a and c <= b:
    print(c)
```
##### 问题11：练习3.11
```python
x = int(input())
y = int(input())
if x % y == 0:
    print('可整除')
else:
    print('不可整除')
```
##### 问题12：练习3.12
```python
a = int(input())
b = int(input())
c = int(input())
if a + b == c or a + c == b or b + c == a:
    print('二个数和')
if a * b == c or a * c == b or b * c == a:
    print('两个数乘积')
```
##### 问题13：练习3.13

```python
a = int(input())
b = int(input())
c = int(input())
if a <= b and b <= c:
    print(str(a) + '\n' + str(b) + '\n' + str(c))
elif a <= c and c <= b:
    print(str(a) + '\n' + str(c) + '\n' + str(b))
elif b <= a and a <= c:
    print(str(b) + '\n' + str(a) + '\n' + str(c))
elif b <= c and c <= a:
    print(str(b) + '\n' + str(c) + '\n' + str(a))
elif c <= a and a <= b:
    print(str(c) + '\n' + str(a) + '\n' + str(b))
else:
    print(str(c) + '\n' + str(b) + '\n' + str(a))

# 在上面的例子中，我们可以使用18个打印语句(每种情况下有3个)
# 但是我们使用str()函数将整数转换为字符串。 字符串就像单词。
# 您可以将单词与+运算符组合使用。
# 还要记住'\n'表示换行
```
##### 问题14：练习3.14
```python
t = int(input())
h = int(input())
if t < 60 adn h < 40:
    print('露西喝咖啡')
elif t >= 60 and h < 40:
    print('露西喝冰茶')
else:
    print('露西吃冰淇淋')
```
##### 问题15：练习3.15
```python
t = int(input())
h = int(input())
if t < 60 and h < 40:
    print('露西喝咖啡')
elif t < 60 and h < 60:
    print('露西打网球')
elif t < 60 and h >= 60:
    print('露西吃蛋糕')
elif t >= 60 and h < 40:
    print('露西喝冰茶')
elif t >= 60 and h < 60:
    print('露西打高尔夫球')
else:
    print('露西吃冰淇淋')
```

