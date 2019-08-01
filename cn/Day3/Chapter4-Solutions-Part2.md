**问题1：例4.8**

```python
number = int(input())
if number % 7 == 3:
    print(number)
while number != 0:
    number = int (input())
    if number % 7 == 3 :
        print(number)
```

<br>

**问题2：例4.9**

```python
total = 0
number = int(input())
while number != 0 :
    total = total + number * number
    number = int (input())
print(total)
```

<br>

**问题3：例4.10**

```python
n = int(input())
print(n)
while n > 1 :
    if n % 2 == 0 :
        n = n / 2
    else :
        n = n * 3 + 1
    print(int(n))
```

<br>

**问题4：例4.11\***

```python
 number = 1
 counter = 0
 total = 0
 while number != 0 :
    number = int (input())
    if counter < 5 :        # 如果是小于5其中的一个
            total = total + number
    counter = counter + 1
 print(total)
```
<br>

**问题5：例4.12\*\***

```python
number = 1
counter = 0
total = 0
while number != 0:
    last = number       # 在读取之前保存最后一个数字
    number = int(input())
    if counter < 5: # 如果前5个数字之一
        total = total + number
    counter = counter + 1
print(total + last)
```

<br>

**问题6：例4.13**

```python
counter = 10
while counter <= 55:
# 如果一个数字取模小于6 输出数字
    if counter % 10 < 6:
        print(counter)
    counter = counter + 1
```

或者，我们可以使用以下想法：


```python
# 分别保留1位和10位数字
tens =1
ones = 0
# 输出第一个十位数，然后输出个位数
while tens < 6 :
    print(str(tens)+str(ones))
    ones = ones +1
    # 只要一个数字大于5
    # 增加十位数并重置一位数
    if ones > 5 :
        ones =0
        tens = tens + 1
```

<br>

**问题7：例4.14**

```python
counter = 50
while counter >= 10:
    print (counter)
    counter = counter + 1
# #if个数字取模大于5跳到下一个数字
    if counter % 10 > 5:
        counter = counter - 16
```

或者，我们可以使用以下想法：


```python
# 分别保留个位和十位数字
tens = 5
ones = 0
while tens > 0 :
# 先输出是十位数，然后是个位数
    print(str(tens) + str(ones))
    ones = ones + 1
    # 只要个数字大于5
    # 减少十位数并重置一位数
    if ones > 5 :
        ones =0
        tens = tens - 1
```
<br>

**问题8：例4.15\***

```python
counter = 10
while counter < = 6 6:
    # 如果一个数字小于7
    # 并且它是奇数，输出数字
    if counter % 10 < 7 and counter % 2 == 1 :
        print(counter)
    counter = counter + 1
```

或者，我们可以使用以下想法：

```python
# 分别保留个位和十位数字
tens =1
ones = 1
while (tens < 7):
    # 输出第一个十位数，然后输出个位数
    print(str(tens)+str(ones))
    ones = ones + 2
    # 只要个位数字大于6
    # 增加十位数并重置个位数
    if ones > 6:
        ones = 1
        tens = tens + 1
```
<br>

**问题9：例4.16\***

```python
for counter in range (100, 445):
    # 如果个位数和十位数小于5
    # 输出数字
    if counter % 10 < 5 and counter % 100 < 50 :
        print(counter)
```

或者，我们可以使用以下想法：

```python
# 分别保留个位数和十位数
hundreds=l
tens =0
ones =0
while hundreds < 5 :
    # 输出第一个百位，然后是十位和个位数
    print(str(hundreds)+str(tens)+str(ones))
    ones = ones + 1
    # 只要个位数字大于4
    # 增加十位数并重置个位数
    if ones > 4 :
        ones = 0
        tens = tens + 1
    # 只要十位数大于4
    # 增加数百位并重置十位数
    if tens > 4 :
        tens = 0
        hundreds = hundreds + 1
```
<br>

**问题10：例4.17\*\***
```python
# 分别保留个位数和十位数
hundreds = l
tens = 0
ones = 0
while hundreds < 5 :
    # 输出第一个百位，然后是十位和个位数
    print(str(hundreds)+str(tens)+str(ones))
    ones = ones + 1
    # 只要个位数字大于4
    # 增加十位数并重置个位数
    if ones > 4 :
        ones = 0
        tens = tens + 1
    # 如果十位数字大于4
    # 百位数自增
    if tens > 4:
        tens = 0
        hundreds = hundreds + 1
```




