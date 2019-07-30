###### 变量 - 整数和浮点数
---

<table><tr><td bgcolor=#FFE4C4>
secondsInADay = 86400<br>
print("There are", secondsInADay, "seconds in one day.")
</td></tr></table>

将输出：
```python
There are 86400 seconds in one day.
```



在python中，表达式是在一行中还是分成多行并不重要。 例如，以下代码是相同的：
<table><tr><td bgcolor=#FFE4C4>

print("There are", <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;secondsInADay, <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"seconds in one day.")
</td></tr></table>



### 2.3变量的算术运算
假设我们有三个盒子，其中两个盒子里有一些钱。 那么我们就可以在这两个盒子里拿钱，把所有的钱都放到第三个盒子里。同样，假设我们有三个变量名为Box1，Box2和Box3，其中Box1和Box2分别包含数字11和5。 我们可以在Box1和Box2中的数字相加并将总和放到Box3中。 但是，我们不会丢失盒子中的数字; 他们也保持不变。
![blockchain](http://legendary.cdn.play8.io/learnpython/img/day1/2.3.png)


例2.3：假设您有两个三个框，Box1，Box2和Box3。 Box1和Box2分别包含11和5。 编写一个Python程序，将两个盒子中的数字相加，将其放入Box3，然后将Box3输出到屏幕。
```python
Box1 = 11
Box2 = 5
Box3 = Box1 + Box2
print(Box3)
```
输出。
```
16
```

我们可以像算术一样使用算术运算符，+ ， -， * ，/， () 等。









