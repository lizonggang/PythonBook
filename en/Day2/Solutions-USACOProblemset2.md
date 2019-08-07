### Solution for "Promotion Counting"

**The first critical observation is that once some students have reached platinum they are stuck there because there is no division higher than platinum. Therefore, the number of people that were promoted to platinum is simply the number of people that are in platinum after the promotions minus those in platinum before the promotions. However, for the lower divisions this is not the case because participants may have been promoted into those divisions but then later promoted out of those divisions. So, for example, the number of people promoted from silver to gold is the number of people in gold after minus the number of people in gold before plus the number of people promoted from gold to platinum to avoid undercounting. This also works for bronze to silver.**

**Let’s observe this solution on a sample case:**
```
1 2
1 1
1 1
1 2
```

**The number of kids in platinum increased by 1 during the contest which means that there was 1 person that was promoted from gold to platinum. The number of kids in gold stayed the same, but we know that 1 kid was promoted from gold to platinum. Therefore, there must have been 1 person that was promoted from silver to gold (otherwise the number of people in gold would have decreased after the 1 student was promoted from gold to platinum). Similarly, since the number of people in silver stayed the same, there must have been 1 person promoted from bronze to silver to account for the person that left silver by being promoted to gold. Thus the solution is as follows:**
```
1
1
1
```

**Also note that the number of people in bronze is irrelevant to solving this problem.**
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

### Solution for "Bedtime Reading, I"


**We need to find the sum of every positive integer that divides I. In the sample case, we have I=12.**

**Our strategy will be to first find all the divisors, and then add them to our sum. First we read the input and initialize the answer variable, which we will call sigma.**

```
read I
sigma = 0
```

**If a number d is a divisor of I, that means I has no remainder when it is divided by d. For example, 3 is a divisor of 12 because 12%3 = 0. Thus, our test for if d is a divisor of I can be written as:**

```
if I%id = 0:
```

**Now, if it is a divisor, add it to the answer.**
```
sigma += d
```

**So all that remains to do is to find all the possible divisors, so that we can check them. Note that we are only looking for positive integer divisors, so we can start checking at 1. When do we stop checking? We know that no integer bigger than I will be a divisor of I, so we can stop there. We do this with a simple for loop:**

```
for d from 1 to I:
```

**We'll finish off by writing the answer. Putting it all together, we get the full code:**

```python
read I
sigma = 0
for d from 1 to I:
    if I % d = 0:
        sigma += d
output sigma
```

