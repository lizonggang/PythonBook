###### 用python编程
---

练习8.1：编写一个程序，从中读取您的姓名和编号n键盘并在屏幕上打印您的名字n次，每次移动一个空格。

```
样本输入        样本输出
Jane            Jane
4                Jane
                  Jane
                   Jane
```

### 8.2. 字符串操作

我们也可以将数字放在字符串中。但是，它们不是价值观，你不能对它们进行算术运算.

```python
numberl ="21"
number2 ="34"
sum = int(number1 + number2)
print(sum)
```
这个打印2134因为当添加字符串时，它们组合成一个大字符串。

我们可以用上面提到的字符串做一些操作。我们已经看过，如何在字符串中分配值，例如：

```
name ="Jane"
```

我们还可以使用加法(+)和(+=)运算符来连接字符串：

```
name ="Jane"
string ="Hello" + name
```
字符串string里将包含"Hello Jane"。

例8.2：编写一个程序，从中读取名称和数字n键盘并在屏幕上打印名称n次，如下所示：

```
样本输入        样本输出
Jane            *Jane !
4               **Jane !!
                ***Jane !!!
                ****Jane !!!!
```

解决方法：

```python
name = input()
n = int(input())
name = " " + name + " "
for counter in range(n):
    name = "*" + name + "!"
    print(name)
```
