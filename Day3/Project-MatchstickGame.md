# 火柴游戏

（火柴棍游戏 - 人类 vs 人类）

写下面的火柴棍游戏。

火柴棍是一款双人游戏。最初桌上有N个比赛。在每个回合中，当前玩家从表中选择1,2或3个匹配。选择桌上最后一场比赛的玩家赢得比赛。

游戏进行如下：

1. 老板输入匹配数，N在哪里（1 <= N <= 100）
2. 老板输入整数D.如果D为1，则需要在屏幕上绘制带有字符|的匹配项（bar）和*（asteriks） - 请参阅 下面的示例。如果为0，则不会在屏幕上绘制它们。
3. 节目要求当前玩家选择1,2或3场比赛。
4. 玩家输入一个号码。玩家选择的匹配数将从表中删除。
5. 另一位玩家转弯并继续比赛，直到桌上没有剩余比赛为止。
6. 无论谁挑选桌上的最后一根火柴，都会赢得比赛。

## 任务1（总分数的40%）：
- 读取整数N.
- 读取D的值。对于任务1，保证该值为0，因此您无需在此任务中在屏幕上绘制匹配项。
- 连续读取每个玩家的值，并在屏幕上显示当前玩家和剩余匹配数。保证不会有无效输入。例如，球员不会输入5来挑选5场比赛。
- 当屏幕上没有更多匹配时完成游戏。在屏幕上显示获胜者。
请注意，输入和输出格式必须与以下示例完全相同。

样本输入和输出：
（'>'表示用户输入）

```python
Enter the number of matches:
>9
Enter draw value 1 for draw, 0 for not draw:
>0
Number of remaining matches: 9
Player 1: How many matches do you want to pick? (1,2 or 3)
>2
Number of remaining matches: 7
Player 2: How many matches do you want to pick? (1,2 or 3)
>3
Number of remaining matches: 4
Player 1: How many matches do you want to pick? (1,2 or 3)
>3
Number of remaining matches: 1
Player 2: How many matches do you want to pick? (1,2 or 3)
>1
Player 2 won the game!
```

## 任务2（总分数的40％）：
除了任务1之外，这次不保证玩家将输入有效的条目。 您需要检查播放器输入的有效性。 通常记住，移动可以是1或2或3.同时请记住，如果只剩下2个匹配且玩家输入3，则表示无效移动。<br>
**例子：**


```python
>7
Enter draw value 1 for draw, 0 for not draw:
>0
Number of remaining matches: 7
Player 1: How many matches do you want to pick? (1,2 or 3)
>1
Number of remaining matches: 6
Player 2: How many matches do you want to pick? (1,2 or 3)
>4
Invalid move!
You can pick 1, 2 or 3 matches.
Number of remaining matches: 6
Player 2: How many matches do you want to pick? (1,2 or 3)
>0
Invalid move!
You can pick 1, 2 or 3 matches.
Number of remaining matches: 6
Player 2: How many matches do you want to pick? (1,2 or 3)
>3
Number of remaining matches: 3
Player 1: How many matches do you want to pick? (1,2 or 3)
>1
Number of remaining matches: 2
Player 2: How many matches do you want to pick? (1,2 or 3)
>3
Invalid move!
You can pick 1, 2 or 3 matches.
Number of remaining matches: 2
Player 2: How many matches do you want to pick? (1,2 or 3)
>1
Number of remaining matches: 1
Player 1: How many matches do you want to pick? (1,2 or 3)
2
Invalid move!
You can pick 1, 2 or 3 matches.
Number of remaining matches: 1
Player 1: How many matches do you want to pick? (1,2 or 3)
1
Player 1 won the game!
```

## 任务3（总分数的20％）：
除了任务2，您还需要在屏幕上绘制火柴。<br>
**例子：**

```python
Enter the number of matches:
>6
Enter draw value 1 for draw, 0 for not draw:
>1
Number of remaining matches: 6
* * * * * *
| | | | | |
| | | | | |
| | | | | |
| | | | | |
Player 1: How many matches do you want to pick? (1,2 or 3)
>4
Invalid move!
You can pick 1, 2 or 3 matches.
Number of remaining matches: 6
* * * * * *
| | | | | |
| | | | | |
| | | | | |
| | | | | |
Player 1: How many matches do you want to pick? (1,2 or 3)
>2
Number of remaining matches: 4
* * * *
| | | |
| | | |
| | | |
| | | |
Player 2: How many matches do you want to pick? (1,2 or 3)
>3
Number of remaining matches: 1
*
|
|
|
|
Player 1: How many matches do you want to pick? (1,2 or 3)
>1
Player 1 won the game!
```


---

# 火柴游戏

写下与人类玩家一起玩的火柴棍游戏。电脑将是第一个播放器。

火柴棍是一款双人游戏。最初桌上有N个比赛。在每个回合中，当前玩家从表中选择1,2,3，...... M匹配。选择桌上最后一场比赛的玩家赢得比赛。

游戏进行如下：

1. 老板输入匹配数N（1 <= N <= 100）。
2. 老板也进入M;玩家可以选择的最大匹配数（M <= N）。
3. 程序要求当前玩家选择数字匹配（1,2,3 ...... M）。
4. 玩家输入一个号码。玩家选择的匹配数将从表中删除。
5. 另一位玩家转弯并继续比赛，直到桌上没有剩余比赛为止。
6. 无论谁挑选桌上的最后一根火柴，都会赢得比赛。

## 任务1（总积分的%60）：
- 读取整数N.
- 读取整数M.保证M对于此任务始终为3。
- 连续读取每个玩家的值并在屏幕上显示当前玩家和剩余的匹配数量。
- 不保证玩家将输入有效的条目。您需要检查玩家输入的有效性。通常记住，如果M = 3，移动可以是1或2或3。另外请记住，如果只剩下2场比赛且玩家输入3，则表示无效动作。
- 当屏幕上没有更多匹配时完成游戏。在屏幕上显示获胜者
请注意，输入和输出格式必须与以下示例完全相同。

**样本输入和输出：**
（'>'表示用户输入）


```python
Enter the number of matches:
>10
Enter the maximum amount that a player can pick:
>3
Number of remaining matches: 10
Player 1: How many matches do you want to pick? (1..3)
2
Number of remaining matches: 8
Player 2: How many matches do you want to pick? (1..3)
>5
Invalid move!
You can pick 1..3 matches.
Number of remaining matches: 8
Player 2: How many matches do you want to pick? (1..3)
>0
Invalid move!
You can pick 1..3 matches.
Number of remaining matches: 8
Player 2: How many matches do you want to pick? (1..3)
>2
Number of remaining matches: 6
Player 1: How many matches do you want to pick? (1..3)
2
Number of remaining matches: 4
Player 2: How many matches do you want to pick? (1..3)
>3
Number of remaining matches: 1
Player 1: How many matches do you want to pick? (1..3)
1
Player 1 won the game!
```



