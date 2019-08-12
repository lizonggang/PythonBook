### “偶数？奇数？”的解决方案


哦哦！ 这些数字太大而无法存储在我们的普通整数类型中。 但我们需要整数吗？ 您可能还记得，从数学课上我们可以通过查看最后一位数来确定数字是偶数还是奇数。 我们可以在这个问题中使用该策略，并处理它们给我们的整数
字符串。

** Python的注意事项：**这个问题在Python中很容易，因为我们对可以使用的整数大小没有限制。 我们可以只使用。而不是以字符串形式读取整数，然后只使用最后一位数字
模数运算符直接在数字上。

```python
read N
for i from 0 to N-l:
      read t
      if t % 2 == 0:
            print("even")
      else :
            print("odd")
```

从本质上讲，这个问题是N个不同的问题，都在一个输入中。 我们可以独立地解决彼此。 首先，我们读取案例数并迭代每个案例。

```python
read N
for i from 1 to N:
```

在Python中，您不需要做任何额外的事情。 但是在C ++和Java中，我们需要做几件事来检查最后一位数。 我们需要在C ++ / Java中将整数读作字符串。 这对每种语言都有不同的语法，如下所示。

C++|Java
-|-                        
string s;|String s = myScanner.next();
cin >> s;|                            

然后，我们必须得到最后一个数字，作为一个字符。

C++|Java
-|-                 
char lastDigit = s[s.size()-1];|char lastDigit =       
&nbsp;|s.charAt(s.length()-1);


现在，将最后一位数转换为整数。 我们可以通过减去字符“O”来做到这一点。 例如，'4' - '0'将是4.记住这个技巧 - 它经常用于编程。


C++/Java:
```
int digit = (int)(lastDigit-'0');
```

最后，我们检查数字是偶数还是奇数，并相应地输出。 我们将再次使用伪代码：

```python
if digit%2==0: //even
    output "even"
else:             //odd
    output "odd"
```

---

<br>

###“添加逗号”的解决方案

在我们完成完整的解决方案之前，让我们看一下示例案例：
``153920529``

为了找到这种特殊情况的解决方案，我们向后移动数字，每次我们看到的数字位数除以3时加上逗号，除非我们在数字的开头。 添加完所有逗号后，我们得到：
``153,920,529``

解决此问题的一种可能方法是首先将数字存储为字符串。 然后，使用for循环一次迭代字符串3个字符，向后，在每次迭代时添加逗号。 该解决方案如下所示：

```python
read m
n = length(m)
answer = ""
//adding commas by groups of 3
for i from 0 through n-4 incrementing i by 3:
    a = substring of m from n-i-3 to n
    answer = "," + a + answer


// after the last comma is added, there is a bit of the original number

II    from the beginning that needs to  be added to answer
if n mod 3=0:                                            
    b = substring of m from 0 through 3                 
else:                                                     
    b = substring of m from 0 through  n mod 3          

print b + answer
```

在这个解决方案中，在for循环中，我们通过n-4而不是n-3来避免在数字的开头放置一个逗号，其中总的位数可以被3整除。例如，我们想要 避免产生``153,920,529``而不是``153,920,529``。


---

<br>


                                                                              

###“字符串函数编码”的解决方案

 
Bessie的函数f（N，S）有两个参数：字符串S和整数N.该函数返回一个字符串，该字符串是从索引N到结尾+原始字符串的原始字符串的子字符串。 请注意，该函数使用基于0的索引。 例如f（2，“COW”）=“W”+“COW”=“WCOW”; 再次应用它：f（2，“WCOW”）=“OW”+“WCOW”=“OWWCOW”。 第三次应用该功能：f（2，“OWWCOW”）=“WCOW”+“OWWCOW”=“WCOWOWWCOW”。 这解释了第一个样本输出。
 
对于每个字符串，使用循环重复Bessie函数指定的次数。 要实现Bessie的函数，请通过将原始字符串的子字符串与原始字符串连接来创建新字符串。

```python
read Z 
for i from 1 to Z: 
    read N C curStr 
    for j from 1 to C: 
        curStr = substring of curStr from N to end (0-indexed) + curStr 
    print curStr 

```
