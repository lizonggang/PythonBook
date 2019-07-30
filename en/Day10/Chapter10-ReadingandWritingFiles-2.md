###### 用python编程
---


例子10.1 写一个程序读取数字N，N从文件获取。 程序将这些数字和和写入文件。

```
infile.txt:                 outfile.txt
5                           The sum is 16.
1 2 3 4 5 6
```

```python
fin = open("infile.txt", "r")
fout = open("outfile.txt", "w")
numbers = fin.readline().split()

sum = 0
for i in range(N):
    sum += int(numbers[i])
fout.write(str(sum)+"\n")
fout.close()
```

首先，我们从第3行的文件中读取N。然后，我们读取一行中的所有数字
并使用split()将它们转换为数组。 接下来，我们添加数字在第7-8行遍历数组的循环。 最后在第9行，我们写出答案在文件中。

在例子中，N在开头给出。 假设没有给出N，我们必须读取数字直到文件末尾。

```
infile.txt:                 outfile.txt
1                           The sum is 6.
2
3
4
5
6
```

我们写一个程序像这样：

```python
fin = open("infile.txt", "r")
fout = open("outfile.txt", "w")
N=0
numbers = [0]*100
while True:
    value = fin.readline()
    if not value:
        break
    numbers[N] = int(value)
    N += 1
sum = 0
for i in range(N):
    sum += int(numbers[i])
fout.write(str(sum) + "\n")
fout.close()
```

