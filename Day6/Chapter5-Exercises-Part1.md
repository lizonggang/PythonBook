**问题1**
编写一个程序，从输入中读取数字，并在中间输出数字。 当用户输入0时程序停止。保证用户输入奇数个数字，最多有21个数字（包括0）。<br>
**例子:**

输入|结果
-|-
3|11
9|
123|
11|
12|
99|
0|


**问题2**
编写一个程序，从输入中读取N个N个数字，其中N <= 20。 然后它以相反的顺序将这些数字写入屏幕。<br>

**例子:**

输入|结果
-|-
6|99
3|12
9|11
123|123
11|9
12|3
99|


**问题3**
从输入读取N个N个数字（N <= 20）并将它们放入数组中。 然后读取A和B，并在数组中写入可以按相同顺序被A或B整除的数字。<br>
**例子:**

输入|结果
-|-
7|15
15|21
19|6
7|18
21|
6|
37|
18|
3|
5|


**问题4**
给定N，则N个数（N <= 20）发现数字序列是否对称。 如果数字序列是对称的，则写入“对称”，否则在屏幕上写“不对称”。<br>
**例子:**

输入|结果
-|-
8|不对称
15|
19|
7|
21|
6|
37|
18|
1|
7|对称
15|
19|
7|
21|
7|
19|
15|


**问题5**
找到第一次出现的数字K的索引，如果找不到返回-1。 您将获得一个N个数字列表（1 <= N <= 20000）。

例如，假设您被赋予以下数组作为输入。

```python
2 3 4 4 9 11 12

```

搜索4应返回2，搜索9应返回4，并且搜索10应该返回-1。

输入格式：

*第1行：整数N.

*第2行：N个整数排序。

*第3行：整数K.

样本输入：

```
7
2 3 4 4 9 11 12
9
```

输出格式：

*第1行：提供的数组中第一次出现K的索引，如果没有找到返回-1。

样本输出：

4

输出详情：

9的索引是4。

<br>

**问题6**
从输入读取N个N个数字（N <= 200）并将它们放入数组中。 然后再次写出数字，但所有0都移到前面。
<br>

**例子:**

输入|结果
-|-
8|0 0 82 82 9 42 100 23
82|
82|
9|
42|
0|
100|
23|
0|

<br>

**问题7**
从输入读取N个N个数字（N <= 200）并将它们放入数组中。 然后再次写出数字，但所有负数都以相同的顺序移到前面。
<br>

**例子:**
输入|结果
-|-
5|-32 -11 48 26 47
48|
26|
47|
-32|
-11|