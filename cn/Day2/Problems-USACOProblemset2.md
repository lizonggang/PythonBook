**问题 1**

```
促销计数
==================

Bessie the cow 正在帮助Farmer John参加美国牛奥林匹克运动会（USACO），一个在线竞赛，参与者回答挑战问题证明他们对牛琐事的掌握。

为了回应更广泛的参与者背景，Farmer 约翰最近将比赛扩大到包括四个部门难度：青铜，银，金和铂金。全新参与者从青铜师开始，任何时候他们都得分完美的比赛他们被提升到更高的难度。参与者甚至可以晋升在同一场赛中多次。农夫约翰跟踪一个所有参赛者及其当前部门的名单，所以他可以随时在适当的水平开始每个人一个比赛。

在发布他最近的比赛结果时，Farmer约翰想要包括参与人数的信息从铜到银，从银到金，从黄金到白金。然而，他忽略了计算促销活动的时间在比赛期间发生。贝茜，她是聪明的牛然而，实现了Farmer John可以推断出的数量促销活动仅来自参与者的数量比赛前后的每个级别。请帮她表演这个计算！

问题名称：推广

输入格式：

输入由四行组成，每行包含两个整数范围0..1,000,000。第一行指定青铜的数量参赛者在比赛前后注册。第二line指定之前和之后的白银参与者数量比赛。第三行指定黄金数量比赛前后的参赛者。最后一行指定比赛前后的白金参与者人数。

输出格式：

请输出三行，每行包含一个整数。该第一行应包含参与者的数量从青铜器升为银牌。第二行应该包含从白银晋升为黄金的参与者人数。该最后一行应该包含参与者的数量从黄金升级到铂金。

样品输入：

1 2
1 1
1 1
1 2

样本输出：

1
1
1

在这个例子中，每个部门登记了1名参与者在比赛之前。比赛结束时，有2名参赛者以青铜和白金登记。这可能是一种方式发生的事情是在比赛期间加入了2名新参与者;一被推广到铂金，另一个留在青铜。
```


<br>

**问题 2**

```
我睡前读书，
==================

农夫约翰正在为他做夜间睡前阅读工作。 “哦，这让我很头疼，”贝茜呻吟道。

“但这只是简单的数论，”FJ回答道。 “我们过去吧它再次。 数字的sigma函数只是它的总和除数的数量。 所以，对于像12这样的数字，除数是1,2,3,4,6和12.总结它们我们得到28.”

“这里的所有都是它的？” 贝茜问道。

“是的。” FJ回答道。 “也许有人会写一个程序来计算整数I的西格玛函数（1 <= I <= 1,000,000）。”

问题名称：br1

输入格式：

*第1行：单个整数，I

样品输入：

12

输出格式：

*第1行：我所有除数的总和。

样本输出：

28
```