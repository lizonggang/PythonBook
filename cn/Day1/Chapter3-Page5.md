###### 条件语句
---

<table><tr><td bgcolor=#87CEFA>if-eise语句的一般形式是：<br>
<br>
if 条件表达式:<br>
&nbsp;&nbsp;&nbsp;&nbsp;(表达式)<br>
&nbsp;&nbsp;&nbsp;&nbsp;...<br>
else:<br>
&nbsp;&nbsp;&nbsp;&nbsp;(表达式)<br>
&nbsp;&nbsp;&nbsp;&nbsp;...
</td></tr></table>



### 3.5. if - else if - else

在if语句中，我们可以有一系列条件延续 'else if'。
例3.6：假设输入一个得分，我们会输出 'not good'，'fair'，'good'，或者屏幕上的 'awesome';

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•得分<50，
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•50 <得分<70，
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•70 <得分<90，
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;•得分> 90。

```python
i£ score < 50:
    print ("not good")
elif score >= 50 and score < 70:
    print("fair")
elif score >= 70 and score < 90:
    print("good")
else:
    print("awesome")
```

> [!NOTE] 
> 注意：不要忘记if，elif和else行末尾的冒号(:)。


