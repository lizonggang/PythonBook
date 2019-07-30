## 盒装游戏中的便士
箱子里的便士是一个双人棋盘游戏。 该板是一系列N盒。 最初，每个盒子都有一些便士。 玩家轮流。 在每个回合中，当前玩家选择最左边或最右边的框。 当没有剩余的盒子时游戏结束。 在游戏结束时，拥有最多便士的玩家赢得比赛。 如果两个玩家拥有相同数量的便士，那么游戏将被束缚。 一个示例游戏如下：

```
Board (N = 8)        Player turn  Player move  Player 1 score  Player 2 score
-----------------    -----------  -----------  --------------  --------------
8 12 2 4 6 3 7 10        1           Right          10              0
8 12 2 4 6 3 7           2           Right          10              7
8 12 2 4 6 3             1           Left           18              7
 12 2 4 6 3              2           Left           18             19
    2 4 6 3              1           Left           20             19
      4 6 3              2           Left           20             23
        6 3              1           Left           26             23
          3              2           Right          26             26
```

- 游戏是平局！

## 任务1（总积分的60%）：
在盒子游戏中写一个两个玩家的便士。

游戏设计：
老板最初输入板N的大小（1 <= N <= 20）并且N个整数每个数大于0。
玩家1开始游戏。
在每个回合中，依次输出棋盘，玩家和他们的分数。
程序要求玩家进入移动。 玩家将输入1表示左侧或2表示右侧。 否则程序将告知移动无效并要求同一玩家再次移动。
如果有胜利者或者是平局，则程序应输出游戏结果并停止。
样本输入和输出：
（'>'表示用户输入）

```
Enter the number of boxes:
>5
Enter pennies in each box:
>1 5 8 3 17

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>1

Boxes:
5 8 3 17
Player 1 score:1
Player 2 score:0
Enter player 2 move (1 for leftmost,2 for rightmost):
>2

Boxes:
5 8 3
Player 1 score:1
Player 2 score:17
Enter player 1 move (1 for leftmost,2 for rightmost):
>7
Invalid move!

Enter player 1 move (1 for leftmost,2 for rightmost):
>7
Invalid move!

Enter player 1 move (1 for leftmost,2 for rightmost):
>8
Invalid move!

Enter player 1 move (1 for leftmost,2 for rightmost):
>1

Boxes:
8 3
Player 1 score:6
Player 2 score:17
Enter player 2 move (1 for leftmost,2 for rightmost):
>2

Boxes:
8
Player 1 score:6
Player 2 score:20
Enter player 1 move (1 for leftmost,2 for rightmost):
>1
Player 1 score:14
Player 2 score:20
Player 2 won!
```

任务2（总分数的40%）：
除了任务1，改进你的程序，以便它允许玩家撤消他们的动作。 玩家将输入1表示左侧，2表示右侧，3表示撤消。 否则程序将告知移动无效并要求同一玩家再次移动。

如果玩家输入3，则需要返回之前的状态。 您需要取消最后一步，更新分数并相应地更新转弯。 如果没有撤消动作，换句话说，如果你到达游戏的开头，当用户输入3时就不会有任何变化。

样本输入和输出：
（'>'表示用户输入）

```
Enter the number of boxes:
>5
Enter pennies in each box:
>1 5 8 3 17

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>1

Boxes:
5 8 3 17
Player 1 score:1
Player 2 score:0
Enter player 2 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>5
Invalid move!

Enter player 1 move (1 for leftmost,2 for rightmost):
>6
Invalid move!

Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>1

Boxes:
5 8 3 17
Player 1 score:1
Player 2 score:0
Enter player 2 move (1 for leftmost,2 for rightmost):
>1

Boxes:
8 3 17
Player 1 score:1
Player 2 score:5
Enter player 1 move (1 for leftmost,2 for rightmost):
>2

Boxes:
8 3
Player 1 score:18
Player 2 score:5
Enter player 2 move (1 for leftmost,2 for rightmost):
>1

Boxes:
3
Player 1 score:18
Player 2 score:13
Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
8 3
Player 1 score:18
Player 2 score:5
Enter player 2 move (1 for leftmost,2 for rightmost):
>3

Boxes:
8 3 17
Player 1 score:1
Player 2 score:5
Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
5 8 3 17
Player 1 score:1
Player 2 score:0
Enter player 2 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>3

Boxes:
1 5 8 3 17
Player 1 score:0
Player 2 score:0
Enter player 1 move (1 for leftmost,2 for rightmost):
>1

Boxes:
5 8 3 17
Player 1 score:1
Player 2 score:0
Enter player 2 move (1 for leftmost,2 for rightmost):
>1

Boxes:
8 3 17
Player 1 score:1
Player 2 score:5
Enter player 1 move (1 for leftmost,2 for rightmost):
>2

Boxes:
8 3
Player 1 score:18
Player 2 score:5
Enter player 2 move (1 for leftmost,2 for rightmost):
>2

Boxes:
8
Player 1 score:18
Player 2 score:8
Enter player 1 move (1 for leftmost,2 for rightmost):
>2
Player 1 score:26
Player 2 score:8
Player 1 won!
```


