## 第五章：参考答案-第2部分

**问题1：练习 5.6\*\***

```python
n = int(input()) # read n。 n是数字的数量
numbers = input().split() # 这里我们创建一个数组，数组的名字是numbers
# 我们需要将数组项转换为整数
for i in range (len(numbers)):
    numbers[i] = int (numbers[i])
# 现在我们将创建另一个名为freq的数组。
# freq [x]将保持x在数字数组中出现的次数
freq = [0] * 1001 # 数组的最大数量可以是1000.因为1000是包含的 inclusive
for i in range ( n ) :
    freq[numbers[i]] = freq[numbers[i]] +1
for i in range (1001):
    if freq[i] > 1 :
        print (i)
```

<br>

**问题2：练习 5.7\*\***

```python
n = int(input()) # read n。 n是数字的数量
numbers = input().split() # 这里我们创建一个数组，数组的名字是numbers # 我们需要将数组项转换为整数
# 我们需要将数组项转换为整数
for i in range (len(numbers)):
    numbers[i] = int (numbers[i])
# 现在我们将创建另一个名为freq的数组。
# freq [x]将保持x在数字数组中出现的次数
freq = [0] * 1001 # 数组的最大数量可以是1000.因为1000是包含的 inclusive
for i in range ( n ) :
    freq[numbers[i]] = freq[numbers[i]] + 1
for i in range (1001):
    if freq[i] > 0 :
        print (i)
```

<br>

**问题3：练习 5.8\*\*\***

```python
n = int(input()) # read n。 n是数字的数量
numbers = input().split() # 这里我们创建一个数组，数组的名字是numbers # 我们需要将数组项转换为整数
# 我们需要将数组项转换为整数
for i in range (len(numbers)):
    numbers[i] = int (numbers[i])
# 现在我们将创建另一个名为freq的数组。
# freq [x]将保持x在数字数组中出现的次数
freq = [0] * 1001 # 数组的最大数量可以是1000.因为1000是包含的 inclusive
for i in range ( n ) :
    freq[numbers[i]] = freq[numbers[i]] + 1
i=0
while i<1001 :
    if freq[i] > 0 : # 只要频率> 0，则打印索引
        print (i)
        freq[i] = freq[i] - 1 # 每次打印后降低频率
    else :
        i = i + 1 # 如果频率为0则转到下一个
```

<br>

**问题4：练习 5.9\*\***

```python
n = int(input()) # read n。 n是第一个数组的数量。
arrl = input().split() # 这里我们创建一个数组，数组的名字是 arrl
# 我们需要将数组项转换为整数
for i in range (len(anrl)):
    arrl[i] = int (arrl[i])
m = int(input()) # read m。 m是第二个数组的数量
arr2 = input().split() # 这里我们创建一个数组，数组的名字是 arr2
# 我们需要将数组项转换为整数
for i in range (len(arr2)):
    arr2[i] = int (arr2[ij)
# 现在我们将创建1个freq数组，以保持x在arrl和arr2组合中出现的次数
freq = [0] * 2001 # 数组的最大值可以是1000.因为1000是包含的
# 但是，由于我们在这里有负数，我们需要将所有数字移动1000
for i in range ( n ) :
    freq[arrl[i]+1000] = freq[arrl[i]+1000] + 1
for i in range ( m ) :
    freq[arr2[i]+1000] = freq[arr2[i]+1000] + 1
i=0
while i<2001 : # 范围介于0到2000之间
    if freq[i] > 0 : # checking freq
        print (i-1000 , end = " ") # shift回来！
        f「eq[i] = f「eq[i] - 1
    else :
        i=i+1
```

<br>

**问题5：练习 5.10\*\*\***

```python
n = int(input()) # read n。 n是第一个数组的数量
arrl = input().split() # 这里我们创建一个数组，数组的名字是 arrl
# 我们需要将数组项转换为整数
for i in range (len(arrl)):
    a「rl[i] = int (a「rl[i])
m = int(input()) # read m。 m是第二个数组的数量
arr2 = input().split() # 这里我们创建一个数组，数组的名字是 arr2
# 我们需要将数组项转换为整数
for i in range (len(arr2)):
    arr2[i] = int (arr2[ij)
# 现在我们将创建1个频率，以保持x出现在arrl和arr2 combinei中的次数
freq = [0] * 2001 # 数组的最大值可以是1000.因为1000是包含的
# 但是，由于我们在这里有负数，我们需要将所有数字移动1000
for i in range ( n ) :
    freq[arrl[i]+1000] = freq[arrl[i]+1000] + 1
for i in range ( m ) :
    freq[arr2[i]+1000] = freq[arr2[i]+1000] + 1
i=0
while i<2001 : # 范围介于0到2000之间
    if freq[i] > 0 : # 检查 freq
        print (i-1000 , end = " ") # shift回来！
        freq[i] = freq[i] - 1
    else :
        i=i+1
```

<br>

**问题6：练习 5.110\*\*\***

```python
n = int(input()) # read n。 n是第一个数组的数量
arrl = input().split() # 这里我们创建一个数组，数组的名字是 arrl
# 我们需要将数组项转换为整数
for i in range (len(anrl)):
    arrl[i] = int (arrl[i])
m = int(input()) # read m。 m是第二个数组的数量
arr2 = input().split() # 这里我们创建一个数组，数组的名字是 arr2
# 我们需要将数组项转换为整数
for i in range (len(arr2)):
    arr2[i] = int (arr2[ij)
# 为每个列表创建一个位置标记
posl = 0
pos2 = 0
while posl < n and pos2 < m :
    # 比较当前位置的数字
    # 输出较小的一个并跳到下一个数字
    if arrl[posl] < anr2[pos2]:
        print (arrl[posl], end = " " )
        posl+= 1
    else :
        print (arr2[pos2], end = M ")
        pos2+= 1
# 如果有的话，写下第一个列表中的剩余数字
while posl < n :
    print(arrl[posl], end = M ")
    posl+= 1
# 如果有，写下第二个列表中的剩余数字
while pos2 < m :
    print(arr2[pos2], end = M ")
    pos2+= 1
```
