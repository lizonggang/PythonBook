###### 条件语句
---

练习3.2：填写___程序代码，以便程序读取两个键盘上的数字，找到这两个数字中的较大者.
```python
numberl = int(input())
number2 = int(input())

if ____:
    print(number2)
else:
    print(number1)
```

练习3.3：从键盘上读取三个正数，然后编写一个程序输出这个数，如果它除6余数是3。

样本输入：
```python
11
9
15
```

样本输出：
```python
9
15
```


### 3.4. 逻辑运算符

假设丹尼说 “如果下雨而且我在外面，我会用我的雨伞”。
考虑以下条件声明：
           如果 x大于5 且 小于10，则输出 'x小于4'。

例3.3：编写一个从键盘读取数字并写入的程序如果给定的数字 大于5且小于10，输出'x小于4'。

```python
x = int(input ())         # read x from keyboard
if x > 5 and x < 10:      # if x is greater than 5 and less than 10
    print("x is less than 4")
```

考虑以下条件声明：
          如果x大于5或小于10，则写 'x小于4'。

假设彼得说 “如果下雨或者我在外面，我会用我的伞，否则我会戴上我的墨镜”。

