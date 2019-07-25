###### 变量 - 字符和字符串
---

上面的代码在前面添加了一个或多个'*'， 在每个字符串的末尾加上 '!'。
要检查两个字符串是否相等，我们使用 '==' 或 '!='运算符与整数变量一样。

例8.3：编写一个程序，读取符键盘上的两个数字的和一个算术运算(+， - ，*，/)。该程序将操作应用于运算并在屏幕上打印结果：

```
样本输入        样本输出
5               105
21
*
```

解决方案：

```python
numl = int(input())
num2 = int(input())
op = input()
if op =="+"：
    result = numl + num2
if op =="-"：
    result = numl  -  num2
if op =="*"：
    result = numl * num2
if op =="/"：
    result = numl / num2
print(result)
```
我们还可以使用'<'，'<='，'>='和运算符来比较字母顺序字符串。

```python
if string1 < string2：
    print("string1在string2之前")
else:
    print("string1不在string2之前")
```

则上面的代码片段打印'string1在string2'之前按字母顺序排在string2之前。假设string1是'try it'和string2 is'trial'then程序打印string1不在String2'之前。

> [!NOTE]
> 大写字母在计算机中的小写字母之前。
例如，如果string1为'zinc'且string2为'about'，则打印该程序
'string1 is before string2'，因为 'Z'是在'a'前。

