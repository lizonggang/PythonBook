###### 读/写文件
---

# <center>第10章: 读/写文件</center>
---


### 10.1.文件流

请考虑以下示例：

```python
age = int(input())
print("You are " + str(age) + " years old.")
```

您将在屏幕上看到如下：

```
Hi, how old are you?
14
You are 14 years old.
```

print()和input()函数用于与用户交互。这样，我们在屏幕上写句子来提问或说些什么并得到来自用户的答案。我们写入屏幕的内容称为"输出"，我们从用户那里读取程序获取输入，处理它，以及打印输出。有时，从键盘上读取并写入屏幕不实用;每次程序运行时我们都必须从键盘输入。
相反，我们可以使用文件;我们可以将输入一次写入文件和程序每次都从文件中读取。而且，我们可以保存输出另一个文件供进一步使用而不是写入屏幕。

```python
fin = open("infile.txt", "r")
fout = open("outfile.txt", "w")
age = int(fin.readline())
fout.write("You are " + str(age) + "years old.\n")
fout.close()
```

```
infile.txt:                 outfile.txt
14                           You are 14 years old.
```

在第1行，我们打开输入文件，而我们在第2行打开输出文件。输入
文件在open()中用"r"值表示。同样，指示输出文件
用"w"。在第3行，我们使用readline() 来读取文件中的输入而不是
键盘。在第4行，我们使用write()而不是print()来写输出
文件而不是屏幕。请注意，我们最后使用了"\n"。在Python中，"\n"
是行尾字符，写"不按Enter键作为print()。所以我们
最后手动添加它。最后一件事就是关闭输出文件，如图第5行所示。


在运行程序之前，我们打开infile.txt 并在其中写入所需的输入。
在上面的例子中，输入是14.因为我们假设输入已经是
在我们运行程序的文件中，我们不需要通知用户输入像我们在第一个例子中所做的输入。

