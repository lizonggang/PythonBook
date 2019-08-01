# 第5章提示：练习 - 第2部分

**反向索引** 是解决其中一些练习题的好主意。 简单来说，反向索引可以描述为使用数组的索引号来存储某些值。


示例：想象一下考试。 最低分为0，最高分为10.有7名学生教师可以通过两种方式存储学生的分数：

1-）创建一个数组并存储存储分数的学生student_scores [] = {4,6,2,10,4,7,4}

2-）为存储得分频率得分的分数创建一个数组score_frequency [] = {0,0,1,0,3,0,1,1,0,0,1}


<br>

**student_scores[]** 是常规索引。 我们只存储得分.

Student_0 has a score of 4

Student_1 has a score of 6

Student_2 has a score of 2 ... etc. and finally

Student_6 has a score of 4



另一方面， **score_frequency[]**  是反向索引，它以不同的方式保存数据。

There is/are 0 student(s) who received 0 as a score

There is/are 0 student(s) who received 1 as a score

There is/are 1 student(s) who received 2 as a score

There is/are 0 student(s) who received 3 as a score

There is/are 3 student(s) who received 4 as a score

There is/are 0 student(s) who received 5 as a score

There is/are 1 student(s) who received 6 as a score

There is/are 1 student(s) who received 7 as a score

There is/are 0 student(s) who received 8 as a score

There is/are 0 student(s) who received 9 as a score

There is/are 1 student(s) who received 10 as a score



常规指数和反向指数的利弊
- 在常规索引中，您可以存储任何数字（prō）
- 在反向索引中，数据需要受到限制。 （在此示例中，最大分数 - 为10因此，数组大小必须至少为11.如果数据不受限制 - 不能使用反向索引）（contrā）
- 在常规索引中，为了对数据进行排序，您需要一种排序算法（contrā）
- 在反向索引中，数据已经排序（prō）
- 在常规索引中，您需要花费一些精力来查找数据频率（contrā）
- 在反向索引中存储频率（prō）
- 在常规索引中，您不必担心存储的数据。 （数据可以是 - 例如负面）（prō）
- 在反向索引中，您不能保留负值。 因为数组索引始终 - 从0开始并逐个增加。 （控制）{在某些情况下你可以通过将所有值移动相同的数量来克服这个问题}


现在这里有提示：

**问题1：**反向索引的简单应用。 所有数字均为正数，限制为1000.（可行）

**问题2：**所有数字均为正数，不同，限制为1000.（可行）

**问题3：**所有数字都是正数，限制是1000.（可行）这次你需要考虑数字可以重复。 它们可能并不明显。 当您打印结果时，您将有一个嵌套循环（最好是while循环），它将继续打印索引（如果该索引处的内容大于0），则减少每个打印的索引。 内容变为0后停止打印索引

**问题4：**将所有数字移动1000.（因为最小数字是-1000。如果你将每个数字移动1000，那么最小数字将存储在数组的第0个索引中。你需要创建你的 这个问题中的数组大到2001年。为什么？
**问题5：**有2组数据。 相同的反向索引数组将用于两组数据。 限制是-1000到1000.需要转移。 阵列大小约为2千。（可行的）

**问题6：**您不能使用反向索引，因为数字不受问题5的限制。因此您需要找到另一种方法。



假设有两个变量。 （我将它们称为指标1和指标2）简而言之，假设i1和i2

并且有两个阵列。 数组a []和数组b []

Array **a** has **n** numbers in it , and array **b** has **m** numbers in it.  So far so good

Now i1=0 and i2=0

In a loop of (m+n) numbers 

Compare a[i1]  versus b[i2]       If a[i1]<b[i2]  print a[i1] and increase i1 by1  else  print b[i2] and increase i2 

如果i1达到其极限（n）并且i2达到其极限（m为m），则需要小心。尽量避免“超出边界”错误。

一旦完成一个数组（我的意思是完成），您需要打印其他数组的剩余数字。 毕竟两个数组都是最初排序的。

