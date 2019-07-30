###### 用Python编程
---


练习8.5：写一个程序读取一个字符串s和三个整数a，b和n键盘，并写入从第a的位置开始的s子串继续b个字符，在屏幕上n次。

```
样本输入                    样本输出
Helloworld!                 oworl
4                           oworl
5                           oworl
5                           oworl
                            oworl
```



在上面的例子中，从第4位置开始的子字符串是'oworl'。
我们可以获得类似于数组的字符串的一部分。我们可以编写简化代码
在上一个练习中如下：

```python
s = input()
a = int(input())
b = int(input())
n = int(input())
substring = s[a:a+bj
for counter in range(n):
    print(substring)
```

s[a:a+b]是从索引a到索引 a + b（不包括a + b）的s的字符串。


练习8.6：写一个程序从键盘读取两个字符串s1，s2和两个整数a，n。在s2位置插入s1，然后将新字符串写入n次。

```python
样本输入                    样本输出
Helloworld!                 HelloNewworld!
New 5 3                     HelloNewworld!
                            HelloNewworld!
```

> [!TIP]
> 您可以使用子字符串的想法。

Exerdse8.7：写一个程序读取来自键盘的一个字符串s和三个整数a， b，n。从位置a开始删除s中的b个字符，然后写入新字符串n次在屏幕上。

```python
样本输入                    样本输出
Helloworld!                 Helld!
2 5 3                     Helld!
                            Helld!
```

> [!TIP]
> 您可以使用子字符串的想法。

