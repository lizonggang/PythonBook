## 第五章: 参考答案-第一部分

**问题1：练习 5.1**

```python
myArray = [0] * 21
counter = 0
number = int(input())
while number != 0 :             # 存储数组中的数字
    myArray[counter] = number
    counter = counter + 1
    number = int(input())
middle = int(counter / 2)       # 数组的中间位置，必须是int
print(myArray[middle])          # 在中间输出数字
```

**问题2：练习 5.2**

```python
myArray = [0] * 20
n = int(input)  # 从键盘读取n
# 从键盘读取n个数字
for counter in range(n) :
    number = int(input())
    myArray[counter] = number
 # 以相反顺序输出数字
 for counter in range(n - 1, -1 , -1) :
    print(myArray[counter])
```

一种替代方式：

```python
myArray = [0] * 20
n = int(input)# 从键盘读取n
# 从键盘读取n个数字并反向存储它们
for counter in range(n - 1, -1 , -1) :
    number = int(input)
    myArray[counter] = number
 # 输出数字
 for counter in range(n):
    print(myArray[counter])
```

**问题 3:**

```python
myArray = [0] * 20
n = int(input) # 从键盘读取n
# 从键盘读取n个数字
for counter in range(n):
    myArray [counter] = int(input)
# 从键盘上读取a和b
a = int(input)
b = int(input)
for counter in range(n);
    #输出数组中的位置，如果它可被a或b整除
    if myArray[counter] % a == 0 or myArray[counter] % b == 0 :
        print(myArray[counter])
```


**问题4：练习 5.5\*\***

```python
arr = [0] * 20
    # 读n然后将n个数字放入数组中
n = int(input)
for i in range(n) :
    arr[i] = int(input())
# 检查位置0和n-1,1和n-2的数字，
# 直到数组的中间
symmetric = 1
left = 0
right = n-1
while left<right :
    if arr[left] != a r r [ r i g h t ] :
        symmetric =0
    left = left + 1
    right = right - 1
# 如果数组不对称，先输出“not”
if symmetric == 0 :
    print("not", end = •_ •，）
print("symmetric")
```


一种替代方式：

```python
arr = [0] * 20
rev = [0] * 20
    # 读n然后将n个数字放入数组中
n = int(input)
for i in range(n):
    arr[i] = int(input)
    # 以相反的顺序保存数字
    rev[n-i-l]=arr[i]
# 检查数组是否与其反向相同
symmetric = 1
for i in range(n):
    if arr[i] != rev[i]:
        symmetric =0
# 如果数组不对称，先输出“not”
if symmetric == 0:
    print("not", end=" ")
print("symmetric")
```

**问题 5:**

```python
arr = [0] + 20000
n = int(input)
# 将数字读入数组
for i in range(n):
    arr[i] = int(input)
k = int(input)
pos = -1 # 数组中k的位置
# 检查k是否在数组中
for i in range(n):
    if arr[i] == k :
        pos = i
        break
        # 首次出现时必须使用#break命令
print(pos)
```


**问题 6:**

```python
arr = [0] * 200
n = int(input)
# 将数字读入数组
for i in range(n):
    arr[i] = int(input)
    if arr[i] == 0 :              # 输出0是第一个
        print(0, end=" ")

# 输出除0之外的数组
for i in range(n):
    if arr[i] != 0 :
        print(arr[i], end=" ")
```


**问题 7:**

```python
arr = [0] * 200
n = int(input())
# 将数字读入数组
for i in range(n) :
    arr[i] = int(input())
    if arr[i] < 0 :   # 首先输出负数
        print( arr[i] , end=" ")

# 输出除负数之外的数组
for i in range(n):
    if arr[i] >= 0 :
        print( arr[i] , end=" ")
```
