## 猜猜我的号码游戏
你会猜猜我的数字游戏。 这场比赛是一场双人比赛;

- 一个是“挑选者”，另一个是“猜测者”。
- Picker选择1到100之间的整数，猜测者猜测它。
- 猜测者的目标是以最少的猜测猜测选择器的数量。
- 每次猜测后，选择器都会提供反馈，例如“下降”，“上升”或“正确”
    - “下降”意味着选择器的数量小于猜测者的猜测
    - “上升”意味着选择器的数量大于猜测者的猜测
- 当猜测者正确猜出选择器的号码时，游戏结束。


### 任务1（总分数的40%）：
- 读取整数N.保证用户输入1到100之间的数字。
- 连续读取用户的猜测，直到用户输入正确的数字N.
- 最后打印猜测数量。
请注意，输入和输出格式必须与以下示例完全相同。

**样本输入和输出：**

（'>'表示用户输入）

```python
>87
guess:
>34
go up
guess:
>56
go up
guess:
>78
go up
guess:
>90
go down
guess:
>83
go up
guess:
>89
go down
guess:
>88
go down
guess:
>87
correct!
8
```

<br>

### 任务2（总分的60％）：
如果猜测小于1或大于100，则让用户知道它无效。 猜测次数将仅根据有效条目计算。<br>
**例子：**

```python
>87
guess:
>34
go up
guess:
>56
go up
guess:
>104
invalid
>110
invalid
>90
go down
guess:
>-40
invalid
>0
invalid
>1
go up
guess:
>100
go down
guess:
>87
correct!
6
```

