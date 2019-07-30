###### 变量 - 字符和字符串

字符串数组中字符串的特定位置可以如下所示：

```python
print(myStrings[5][3])
```

在屏幕上的myStrings数组中打印字符串5的位置3处的字符。

```python
print(myStrings[5][3:8])
```

打印从位置3开始并且长度为6的字符串5的子字符串myStrings数组在屏幕上。


练习10：写一个程序读取一个整数n，然后是n个单词和一个字符串输入。 从包含s的任何单词中删除。 在屏幕上写下新单词。输入中最多有100个字符串。

```
样本输入                    样本输出
4                           Helloworld! 
Helloworld!                 wer
lower                       trial
trial                       Hel
Hello
lo
```

字符串 'lo' 从'Helloworld!'，'lower'和'Hello'中删除。
