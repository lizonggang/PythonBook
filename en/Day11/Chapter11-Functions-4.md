###### 用python编程

练习11.4：编写一个程序，从键盘上读取三个字符串检查这些字符串中的元音数量是否相等。

```
输入:                       输出:
ThBeE GOOD VoWeLs          Same number of vowels.
ThBeE equal VoWeLs         Not same number of vowels.
```

我们可以在函数内部调用函数。功能的顺序无关紧要。
例如，


```python
def PowerOflO(k):
    return Power(10, k|

def Power (x, y):
    prod = 1
    for i in range(y):
        prod *= x
    return prod

z = int(input())
print(PowerOflO(z))
```

在上面的代码中，PowerOflO 函数调用Power，因此调用Powr函数低于它。

> [!NOTE]
> 备注：正如您所注意到的，当我们拥有时，功能尤其有用多次做一个过程。他们还组织了一个混> 乱的代码，使它更多可以理解的。

<br>

### 11.2. 没有返回值的函数

有时我们不需要函数的返回值。

例11.2: 编写一个读取两个字符串并写入数字的程序在屏幕上这些字符串中的数字。

```python
def NumOfDigits(s):
    digits = 0
    for letter in s:
        if letter >= 101 and letter <= '9':
            digits += 1
    print(digits)

s1 = input()
s2 = input()
NumOfDigits(s1)
NumOfDigits(s2)
```
