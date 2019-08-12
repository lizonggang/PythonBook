### “促销计数”的解决方案

**第一个重要的观察结果是，一旦一些学生达到铂金，他们就会被困在那里，因为没有高于铂金的分数。 因此，晋升为白金的人数仅仅是晋升后的白金人数减去促销前的白金人数。 然而，对于较低级别的部门而言，情况并非如此，因为参与者可能已晋升为这些部门，但后来又晋升为这些部门。 因此，举例来说，从白银晋升到黄金的人数是减去黄金人数之后的黄金人数加上从黄金升级到白金以避免计算不足的人数。 这也适用于青铜色到银色。**

**让我们在样品盒上观察这个解决方案：**
```
1 2
1 1
1 1
1 2
```

**在比赛期间，铂金的孩子数量增加了1，这意味着有1人从黄金晋升到白金。 黄金的孩子数量保持不变，但我们知道1个孩子从黄金晋升到白金。 因此，必须有一个人从白银晋升为黄金（否则在1名学生从黄金晋升为白金后，黄金人数会减少）。 同样地，由于白银的人数保持不变，所以必须有1人从铜牌升级到白银，以解释通过晋升为黄金而留下白银的人。 因此解决方案如下：**
```
1
1
1
```

**另请注意，青铜人数与解决此问题无关。**
```
read BronzeBefore, BronzeAfter
read SilverBefore, SilverAfter
read GoldBefore, GoldAfter
read PlatinumBefore, PlatinumAfter
goldToPlatinum = platinumAfter - platinumBefore
silverToGold = goldAfter - goldBefore + platinumAfter - platinumBefore
bronzeToSilver = silverAfter - silverBefore + goldAfter - goldBefore +
platinumAfter - platinumBefore

print bronzeToSilver
print silverToGold
print goldToPlatinum
```

---

<br>

###解决“睡前读物”


**我们需要找到除以I的每个正整数的总和。在示例中，我们有I = 12。**

**我们的策略是首先找到所有除数，然后将它们加到我们的总和中。 首先，我们读取输入并初始化应答变量，我们称之为sigma。**

```
read I
sigma = 0
```

**如果数字d是I的除数，那意味着当它除以d时我没有余数。 例如，3是12的除数，因为12％3 = 0.因此，我们对if d的除数是I的除数可以写成：**

```
if I%id = 0:
```

**现在，如果它是一个除数，请将其添加到答案中。**
```
sigma += d
```

**所以剩下要做的就是找到所有可能的除数，以便我们检查它们。 请注意，我们只查找正整数除数，因此我们可以从1开始检查。我们什么时候停止检查？ 我们知道没有比我大的整数将成为我的除数，所以我们可以止步于此。 我们通过一个简单的for循环来做到这一点：**

```
for d from 1 to I:
```

**我们将通过写答案来结束。 总而言之，我们得到完整的代码：**

```python
read I
sigma = 0
for d from 1 to I:
    if I % d = 0:
        sigma += d
output sigma
```

