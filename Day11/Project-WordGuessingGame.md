## 猜字游戏
写一个单词猜词游戏。

#### 游戏设计：
1. 最初老板输入了一个秘密词。
2. 秘密字将被屏幕上的星号（*）掩盖 - 每个字母一个星号。
3. 最初玩家有5条命。
4. 在每个回合中，玩家输入一个字母。 如果秘密词不包含该字母，则该玩家将失去一条生命。
5. 在每个步骤中，您需要打印使用过的字母并取消屏蔽玩家在密码中找到的字母。
6. 当生命为0（玩家输了）或玩家找到整个秘密词（玩家获胜）时完成程序。

### 任务1（总分数的40%）：
设计游戏并检查抽奖。 在此任务中，测试数据将始终以平局结束。 您无需检查获胜者或领带。 您可以通过“领带！”消息完成游戏。

##### 样本输入和输出：
（'>'表示用户输入）

```
>computer

********
Enter a lower case letter:
>q
Life left:4
So far you have used these letters:q

********
Enter a lower case letter:
>e

******e*
Life left:4
So far you have used these letters:qe

******e*
Enter a lower case letter:
>c

c*****e*
Life left:4
So far you have used these letters:qec

c*****e*
Enter a lower case letter:
>r

c*****er
Life left:4
So far you have used these letters:qecr

c*****er
Enter a lower case letter:
>t

c****ter
Life left:4
So far you have used these letters:qecrt

c****ter
Enter a lower case letter:
>y
Life left:3
So far you have used these letters:qecrty

c****ter
Enter a lower case letter:
>u

c***uter
Life left:3
So far you have used these letters:qecrtyu

c***uter
Enter a lower case letter:
>i
Life left:2
So far you have used these letters:qecrtyui

c***uter
Enter a lower case letter:
>o

co**uter
Life left:2
So far you have used these letters:qecrtyuio

co**uter
Enter a lower case letter:
>p

co*puter
Life left:2
So far you have used these letters:qecrtyuiop

co*puter
Enter a lower case letter:
>a
Life left:1
So far you have used these letters:qecrtyuiopa

co*puter
Enter a lower case letter:
>s
Life left:0
So far you have used these letters:qecrtyuiopas
You lost!
```

### 任务2（总分的60%）：
除了任务1之外，这次玩家将输入一个小写字母，但不保证玩家每次都会输入一个不同的字母。 如果玩家输入用过的信件，您需要警告玩家。

样本输入和输出：
（'>'表示用户输入）

```
>alphabet

********
Enter a lower case letter:
>a

a***a***
Life left:5
So far you have used these letters:a

a***a***
Enter a lower case letter:
>t

a***a**t
Life left:5
So far you have used these letters:at

a***a**t
Enter a lower case letter:
>a
You have used this letter before. Please enter again:
>t
You have used this letter before. Please enter again:
>e

a***a*et
Life left:5
So far you have used these letters:ate

a***a*et
Enter a lower case letter:
>l

al**a*et
Life left:5
So far you have used these letters:atel

al**a*et
Enter a lower case letter:
>p

alp*a*et
Life left:5
So far you have used these letters:atelp

alp*a*et
Enter a lower case letter:
>h

alpha*et
Life left:5
So far you have used these letters:atelph

alpha*et
Enter a lower case letter:
>g
Life left:4
So far you have used these letters:atelphg

alpha*et
Enter a lower case letter:
>b

alphabet
Life left:4
So far you have used these letters:atelphgb
You won!
```

