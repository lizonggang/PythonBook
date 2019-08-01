###### Nested Conditions
---

# <center>Chapter 6: Nested Conditions</center>

Example 6.1 Every morning at 10 am, Lucy looks at the thermometer and the humidity meter and decides what to eat or drink according to the temperature and the humidity levels. The following table shows what Lucy eats or drinks in what conditions- For example, if the temperature is 45°F and the humidity is 53% then Lucy eats cake. 

&nbsp;|Temperature < 60°F |Temperature > 60°F
-|-|-
Humidity < 40%|Lucy drinks coffee |Lucy drinks iced tea
Humidity >= 40%|Lucy eats cake|ucy eats ice cream

Write a program that reads two numbers, the temperature and the humidity accordingly, from the input and writes what Lucy does to the output.

Sample input:|Sample output:
-|-
45 53|Lucy eats cake


```python
temperature, humidity = input().split()
temperature = int(temperature)

if temperature < 60 and humidity < 40:
        print("Lucy drinks coffee ")
if temperature < 60 and humidity >= 40:
        print("Lucy eats cake")
if temperature >= 60 and humidity < 40:
        print("Lucy drinks iced tea")
if tempecatuce >= 60 and humidity >= 40:
        print("ucy eats ice cream")
```


The first two ifs have a shared condition which the temperature is less than 60°F.
Also, the last two ifs have another shared condition. We can put ifs into two groups by their first conditions as in the figure below. If we check the first
condition we reduce the conditions to two out of four. And then we can check the
other condition separately and decide which action Lucy will take.

<br>

<center> - 49 - </center>

