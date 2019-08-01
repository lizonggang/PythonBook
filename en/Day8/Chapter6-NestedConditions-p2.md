###### Programming with Python
---

![](http://legendary.cdn.play8.io/learnpython/img/day8/p1.png)

The following code shows how we can compare two conditions one after the
other. This is called “nested ``if``s”. In the first ‘``if`` block’， we only consider the conditions that satisfies‘temperature < 60’.

```python
if temperature < 60:
    if humidity < 40:
        print("Lucy drinks coffee")
    else:
        print("Lucy eats cake")
```

Note that the ``else`` corresponds to 'temperature < 60 adn humidity >= 40'.

> [!NOTE]
> In the code above, we may not use parenthesis since the inner ``if`` block is only one statement.

Example 6.2：Write the same program in the previous exercise by using nested ``if``s.

Solution:

```python
temperature, humidity = input().split()
temperature = int(temperature)
humidity = int(humidity)

if temperature < 60:
    if humidity < 40:
        print("Lucy drinks coffee")
    else:
        print("Lucy eats cake")
else:
if humidity < 40:
        print("Lucy drinks iced tea")
    else:
        print("Lucy eats ice cream")
```

<br>

<center> - 50 - </center>

