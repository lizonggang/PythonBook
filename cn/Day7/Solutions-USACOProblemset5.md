### “数学实践”的解决方案

在这个问题中，给出2个整数A，B作为输入。 目标是找到最小的整数E，使得2 A ^ E> A和2 ^ E = B的第一个数字。

在示例中，A = 1且B = 6.如问题陈述所示，可以生成如下表：

```
E       2^E         First digit of 2^E
---     ---         ------------------
2       4           4                 
3       8           8                 
4       16          1                 
5       32          3                 
6       64          6                 
```


当E = 6时; 2 ^ E = 64.这是E的最小值，使得2 ^ E大于A（64> 1）并且64的第一个数字等于B（6），因此答案是E.


这可以通过枚举E的所有可能值来完成，因为E在1..62的范围内。 为了检查第一个数字是否为B，一种方法是将数字转换为字符串，然后取第一个字符，并将字符转换回整数。


Python|C++|Java
-|-|-
ord(str(X)[0]) - ord('0')|to_string(X)[0] - '0'|("" + X).charAt(0) - '0'



另一种方法是除以10的幂次除法，直到找到第一个非零答案。

```python
function firstDigitof(X)
    num = 10AY where 10AY is very large
    while int(X / num) == 0:
        num = num / 10
    return int(X / num)
```


如果没有满足上述条件的答案，则输出0.注意2 ^ e可能会溢出整数类型（在C ++中使用long long或在其他语言中使用类似的东西）

```c++
read A, B

for e in 1 . . 62 :                               
    if 2 ^ e > A and firstDigitof(2 ^ e) == B:
        output e                              
        end the program                       
output 0                                         
```


还有另一个解决方案可以更容易地计算第一个数字 - 而不使用firstDigitOf函数中的循环。 在外环内，跟踪小于或等于2 ^ e的最大功率10。 存储该信息后，计算第一个数字只需要一个整数除法运算。 请参阅下面的实现。

```python
read A, B                                 
pow10 = 1                                 
for e in 1..62:                           
    if 2 ^ e > pow10 * 10:                   
        pow10 *= 10        
    if 2 ^ e > A and int(2 ^ e / pow10) == B:       
        output e                                  
        end the program                           
output 0
```

---
<br>

###解决方案“为什么母牛过马路？”


我们知道，当我们在某个时间在道路的一个特定侧面观察他并且在一段时间之后在道路的另一侧观察他时，一头母牛已经过马路了。 因此，我们必须跟踪10头奶牛的位置，并在我们发现奶牛越过马路时增加适当的计数器。

我们来看一个示例案例：
```
8
3 1
3 0
6 0
2 1
4 1
3 0
4 0
3 1
```

在这种情况下，关于10头奶牛有8个观察结果。 我们在第1侧看到母牛3，然后在0侧看到母牛3，然后再看到0侧，最后是第1侧。通过这些观察，我们可以确定母牛3至少两次切换侧面。 我们只观察过牛6和2一次，所以我们无法确定它们是否会切换侧面。 对于母牛4，我们在第1侧观察他，然后在第0侧观察他，所以我们知道他至少切换了一次。 因此，总的来说，我们可以确认的开关数量是3。

```python
read n
answer = 0
declare array[] of size 10 and initialize all with -1

for i from 0 to n:
    read cowName,sideOfRoad
    if (array[cowname] is not 0) and (array[cowname] is not sideOfRoad):
        answer = answer + 1

    array[cowName] = sideOfRoad

print answer
```


