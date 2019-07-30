###### 用Python编程
---


练习8.2：根据字母顺序对给定的三个字符串进行排序。

```
样本输入            样本输出
hello               Try
about               about
Try                 hello
```

### 8.3. 字符串作为字符数组

实际上，我们可以将字符串视为一个字符数组。也就是说，我们可以取到字符串的特定字符，类似于数组，如下所示：

```python
print(name[3])
```

上面的代码将在屏幕上打印字符串名称的第4个位置的字符。注意字符串的第一个字符位于0位置与数组相同。

但是，以下代码会产生错误：

```python
name[3] = 'z'
```

要更改字符串中的字符，我们不能如上所述。我们将重新审视如何更改字符串。

我们可以使用list()函数将字符串转换为字符数组。例如：

```python
s = "testing"
chararray = list(s)
```

chararray 将是 ['t', 'e', 's', 't, 'i ', 'n', 'g']。

同样，我们也可以使用join()函数将字符数组转换为字符串！）

```python
s = "".join(chararray)
```

这里的值告诉join() 如何合并数组的元素。 例如：

```python
s = "-".join(chararray)
```

在这种情况下，s变为“t-e-s-t-i-n-g”。

### 8.4. 字符串函数

字符串具有不同的有用功能。其中一个是len()函数给出了字符串中的长度。请记住，我们使用len()来获得大小,一个阵列也是。它可以使用如下：

```python
s = "Hello world!"
theLength = len(s)
print(theLength)
```

