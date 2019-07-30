## 蟾蜍和青蛙

写下面的蟾蜍和青蛙游戏。

蟾蜍和青蛙是一个单人游戏。给定一块大小为N（其中N为奇数）的板，板的左侧充满了蟾蜍，右侧是青蛙，中间的正方形是空的。这是N = 7的初始板配置：

```TTT-FFF```

'T'：蟾蜍，'F'：青蛙，'-'：空的

蟾蜍可向右滑动或向右跳过一个方格。同样，青蛙可向左滑动或向左跳过一个方格。游戏的目的是将蟾蜍移动到右侧，将青蛙移动到棋盘的左侧，移动次数最少。最终配置应如下：

```FFF-TTT```

##### 游戏设计：

1. 玩家将输入电路板尺寸N.N是奇数（3 <= N <= 21）。然后你将设置相对于N的板。
2. 在每个回合中，打印当前板和屏幕上的移动次数。
3. 然后程序等待播放器输入，一个介于1到N之间的数字。该数字表示在该正方形中移动元素。
- 示例：3将位置3处的蟾蜍移动到位置4。
- 示例：6将青蛙在位置6移动到位置4。

4. 如果提供的移动无效，请继续询问玩家移动。否则采取行动。

5. 每当所有青蛙都在左侧并且所有蟾蜍在右侧并且空方块在中间时，游戏结束。

N = 5的样本输入和输出：
（'>'表示用户输入）

```
>5

TT-FF
>4

TTF-F
Number of moves:
1

>2

T-FTF
Number of moves:
2

>1

-TFTF
Number of moves:
3

>3

FT-TF
Number of moves:
4

>3
Invalid entry!

>5

FTFT-
Number of moves:
5

>4

FTF-T
Number of moves:
6

>2

F-FTT
Number of moves:
7

>3

FF-TT
Number of moves:
8

You win!
```

#### 任务1（总分数的40%）：

电路板尺寸N始终为7。

#### 任务2（总分数的40%）：
电路板尺寸N可以改变（N是奇数）
#### 任务3（总分数的20%）：
除了任务2，添加撤消移动选项; '0'表示撤消。 玩家应该能够撤消直到游戏开始。

输入和输出样本
（'>'表示用户输入）

```
>15

TTTTTTT-FFFFFFF
>7

TTTTTT-TFFFFFFF
Number of moves:
1

:  :  :
:  :  :

TTTTFT-TFTFFFFF
Number of moves:
7

>9

TTTTFTFT-TFFFFF
Number of moves:
8

>0

TTTTFT-TFTFFFFF
Number of moves:
7

:  :  :
:  :  :

FFFFFFFT-TTTTTT
Number of moves:
62

>8

FFFFFFF-TTTTTTT
Number of moves:
63

You win!
```
