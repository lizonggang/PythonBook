**问题1：例4.20\*\***

```python
x = int(input())
if (x == 0):
    print(0)
# 打印出数字0
while (x > 0):
    # 在屏幕上写一些数字
    print(x % 10 , end = "")
    # 获得一个新数字x
    x = int(x / 10)
```
<br>

**问题2：例4.21\*\***

```python
n = int(input())
m = int(input())
row = 1
col = 1
while row <= n:
# 在屏幕上输出列号
print(row, end="")
# 增加列
col = col + 1
# 如果大于m
if col > m :
    col = 1;            # 重置列 col 等于1
    row = row + 1       # 增加行
    print()             # 转到下一行
```
<br>

**问题3：例4.22\*\***

```python
n = int(input())
row = 1
col = 1
while row <= n :
# 在屏幕上输出列号
print(col, end=" •’）
# 增加列
col = col + 1
# 如果大于row
if col > row :
    col = 1             # 重置列 col 等于1
    row = row + 1       # 增加行
    print ()            # 转到下一行
```
<br>

**问题4：例4.23\*\*\***

```python
n = int(input())
row = 1
col = 1
while row <= n :
    if col == 1 :
        m = int(input())
    if col != 1 :
        print( e n d = •_，.)
# 增加列
col = col + 1
# 如果完成列
if col > m + 1 :
    col = 1           # 重置列 col 等于1
    row = row +       # 重置列 col 等于1
    print()           # 转到下一行
```

<br>

**问题5：例4.24\*\*\***

```python
n = int(input())
m = int(input())
row = 1
col = 1
while row <= n :
print(col + row - 1, end = " " )
# 增加列
col = col + 1
# 如果完成列
if col > m :
    col =1              # 重置列 col 等于1
    row = row + 1       # 重置列 col 等于1
    print()             # 转到下一行
```
<br>

**问题6：例4.25\*\*\***

```python
""" a是从2到n的数字
    b用于检查“a”是否为素数
    b是从“2”到2的平方根的数字
    如果“a”为素数，则prime为1，否则为0
    最初“a”被认为是素数 """

n = int(input())
a = 2
b = 2
prime = 1

while a < n:
    # 每当b到达a的平方根
    # 和a是素数，输出a
    if b*b > a and prime == 1:
        print(a, end = " ")

    # 每当b超过a的平方根时
    if b * b > a :
        b = 2               # 重置 b
        a = a + 1           # 开始检查下一个号码
        prime = 1           # 将prime重置为1
    # 如果a可以被b除掉
    if a % b == 0 :
        prime = 0;          # a不是素数
```

