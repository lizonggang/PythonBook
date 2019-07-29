###### 矩阵
---

你会输出'Right path!'如果路径通向出口的出口位置，否则输出 'Wrong path!'在屏幕上。

### 12.4. 字符矩阵
例12.3：在练习4中，迷宫以整数矩阵给出。
例如，我们可以更直观地在字符矩阵中表示它;

```
样本输入：                  样本输出：
7 6                         Right path!
######
#.#...
#.#..#
#..#.#
##...#
#..#.#
######
ddrdrruulurr
```

在此表示中，'#'对应于墙，'.'对应于空位置。我们不需要在角色之间留出空间。我们可以阅读输入
几乎相同的方式：

```python
n, m = input().split()
n = int(n)
m = int(m)
maze = [[]]*n # create an mepty maze with n rows.

# read the maze from the input
fro row in range(m):
    maze[row] = list(input()) # read the row and convert to a array
path = input()
```


我们也可以使用矩阵来操纵形状。以下练习演示了如何使用矩阵来操纵形状。

练习12.5：编写一个从键盘读取数字n =< 20的程序并在屏幕上打印星号螺旋，如下所示:

```
样本 n = 5                      n = 8
*****                           ********
*                               *
* ***                           * ******
*   *                           * *    *
*****                           * *  * *
                                * **** *
                                *      *
                                ********
```

<br>

**祝贺 - 达到了训练的结束**
