## Tic-Tac-Toe游戏
写一个双人tic-tac-toe游戏。

Tic-tac-toe是一款双人棋盘游戏。 棋盘是3 x 3.第一个玩家将'X'放在棋盘上，第二个玩家放'O'。 无论是横向，纵向还是对角地放置三个相同标记的人都会赢得比赛。 如果在9个动作结束时棋盘已满，并且没有获胜者，那就是平局。

#### 游戏设计：
1. 棋盘最初充满破折号（-）。 第一个玩家以'X'开头。
2. 在每个回合中依次输出棋盘和玩家
3. 程序要求玩家进入移动。 玩家将输入两个整数; 行和列。 行和列都必须介于1和3之间。 否则程序将告知移动无效并要求同一玩家再次移动。 如果任何用户选择了也是无效移动的占用方块。样本tic-tac-toe板：

样本tic-tac-toe棋盘：

```
O-O
XXO
--X
```

'X'是第一个玩家，'O'是第二个玩家。 '-'代表空方块。



#### 任务1（总分数的40%）：
设计游戏并检查抽奖。 在此任务中，测试数据将始终以平局结束。 您无需检查获胜者或领带。 您可以通过"Tie!" 消息完成游戏。

##### 样本输入和输出：
（'>'表示用户输入）


```
---
---
---

Player 1, please enter your move (row, col):
>1 1

X--
---
---

Player 2, please enter your move (row, col):
>2 2

X--
-O-
---

Player 1, please enter your move (row, col):
>3 4

Invalid move!

Player 1, please enter your move (row, col):
>0 2

Invalid move!

Player 1, please enter your move (row, col):
>3 2

X--
-O-
-X-

Player 2, please enter your move (row, col):
>1 2

XO-
-O-
-X-

Player 1, please enter your move (row, col):
>1 3

XOX
-O-
-X-

Player 2, please enter your move (row, col):
>2 1

XOX
OO-
-X-

Player 1, please enter your move (row, col):
>2 3

XOX
OOX
-X-

Player 2, please enter your move (row, col):
>3 3

XOX
OOX
-XO

Player 1, please enter your move (row, col):
>3 1

XOX
OOX
XXO

Tie!
```

#### 任务2（总分的60%）：
设计游戏并检查抽奖和胜利。 只要有胜利者就完成游戏。

##### 样本输入和输出：
（'>'表示用户输入）

```
---
---
---

Player 1, please enter your move (row, col):
>1 1

X--
---
---

Player 2, please enter your move (row, col):
>3 4

Invalid move!

Player 2, please enter your move (row, col):
>5 6

Invalid move!

Player 2, please enter your move (row, col):
>3 1

X--
---
O--

Player 1, please enter your move (row, col):
>2 2

X--
-X-
O--

Player 2, please enter your move (row, col):
>3 2

X--
-X-
OO-

Player 1, please enter your move (row, col):
>3 3

X--
-X-
OOX

1. player won!
```

