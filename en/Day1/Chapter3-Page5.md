###### Conditionals
---

<table><tr><td bgcolor=#87CEFA>General form of if-eise statement is:<br>
<br>
if condition:<br>
&nbsp;&nbsp;&nbsp;&nbsp;(expression)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:<br>
else:<br>
&nbsp;&nbsp;&nbsp;&nbsp;(expression)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:
</td></tr></table>



### 3.5. If - else if- else

In if statement, we can have a chain of conditions continuing with ‘else if’. 

Example 3.6: Suppose that given a score, we will write ‘not good’, ‘fair’, ‘good’ or ‘awesome’ on the screen with respect to the conditions;

- score <50，
- 50=< score <70，
- 70=< score <90，
- score >=90.

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
> Don’t forget the colons``(:)`` at the end of ``if``， ``elif`` and ``else`` lines.


<br>

<center> - 25 - </center>
