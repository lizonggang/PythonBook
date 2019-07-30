###### 用python编程
---

> [!NOTE]
> 函数的名称区分大小写，因为它在变量中。


 示例ll.l：编写一个返回给定字符串中字母数的函数。

```python
def NumLetters(s)：
    count = 0
    for letter in s:
        if (letter >= 'A' and letter <= 'Z') or \
           (letter >= 'a' and letter <= 'z'):
            count += 1
    return count
```


此代码检查for循环中字符串s中的所有字母。如果是当前的字符在'A'和'Z'(大写)或'a'和'z'(小写)之间增量计数。请注意，我们使用 '\' 来包装长行。

练习11.1：编写一个名为Uppercase的函数，将所有字母转换为给定字符串中的大写。例如，

```python
print(UpperCase("i8-iocakes!"))
```

将会在屏幕输出 "I8-10CAKES!"。

练习11.2：编写一个名为SameWords的函数，检查是否有两个无论案例差异如何，单词都是相同的。如果字符串相等，返回1，否则返回0。
例如，将会输出 "0" ，

```python
print(SameWords("Trivial", "Trival"))
```

将会输出 "1" 在屏幕上。

```python
print(SameWords("tRiViAl", "TrIvIaL"))
```


练习11.3：编写一个名为Reverse的函数来反转给定的字符串。
例如，

```python
print(Reverse("!esreveR"))
```

将会输出 "Reverse!" 在屏幕上。

### 11.1. 如何调用函数

我们可以用值调用函数。例如，第14行的功能Power使用两个值10和3调用第一个示例：

```python
pow =Power(10, 3)
```


