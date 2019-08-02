## 第7章：解决方案 - 第1部分

**问题 1: 例子： 7.1**

```python
for number in range(10, 56):
    if number % 10 <= 5:
        print(number)
```

Alternative solution:

```python
# 分别生成1位和10位数
# 然后输出它们
for tens in range (1,6):
    for ones in range (6):
        print(tens, end = "")
        print(ones)
```

**问题 2: 例子： 7.1: 一个更好的例子**

```python
for number in range(10, 56):
    if number % 10 <= 5:
        print(6 - int(number / 10), end = "")
        print(number % 10)
```

Alternative solution:

```python
# 分别生成1位和10位数 然后输出它们
for tens in range(5J 0, -1):
    for ones in range(6):
        print(tens, end = "")
        print(ones)
```

**问题 3: 练习： 7.1**

```python
# 分别生成个位和十位数
# 然后输出它们
for tens in range(1 > 7):
    for ones in range (1,6,2):
        print(tens, end = "")
        print(ones)
```


**问题 4: 练习： 7.2\***

```python
# 试从10到66的所有数字
for number in range (10, 67):
    # 只打印奇数
    # 中有6个或更少的数字
    if number % 10 <= 6 and number % 2 == 1:
        print(number)
```

**问题 5: 练习： 7.3**

```python
# 分别生成个位和十位和百位数
# 然后输出它们
for hundreds in range(1 , 5):
    for tens in range(5):
        for ones in range(5):
            print(hundreds, end="")
            print(tens, end="")
            print(ones)
```

**问题 6: 练习： 7.5**

```python
n, m = input().split()
n = int (n)
m = int (m)
# 保持当前行
for row in range (1, n + 1):
    # 每行中的打印行数m次
    for col in range(m):
        print(row,end="")
    print()
```

**问题 7: 练习： 7.7**

```python
n = int (input())
# 保持当前行
for row in range (1,n+l):
    # 保持当前列
    # 输出每个位置的列号
    for col in ranged row+1):
        print(col, end:"")
    print()
```

**问题 8: 练习： 7.9**

```python
n = int (input())
numbers = input().split()
for i in range(n):
    numbers[i] = int (numbers[i])
    stars = numbers[i]
    # 输出一行中的星星
    for j in range(stars):
        print('*',end="")
    print() # 输出回车
```

**问题 9: 练习： 7.10**

```python
n = int (input())
numbers = input().split() # 将数字保存到数组中
for i in range(n):
    numbers[i] = int (numbers[i])
# 计算数组中每个数字从1到1000
for i in range(1,1001):
    # 计算数组中的数字i
    cnt = 0
    for j in range(n):
        if numbers[j]==i :
            cnt+=l
    # 如果不止一个，输出它
    if cnt > 1:
        print(i)
```

