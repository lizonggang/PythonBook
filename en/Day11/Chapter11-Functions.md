###### Functions
---

# <center>Chapter 11: Functions</center>
---


Consider a cheesecake factory. Cheese, milk, flour, sugar etc... are supplied to
the factory; factory bakes mixing them and produces cheesecake. **Functions** are like factories; they get ``input``, makes some ``operations``, and produce ``output``.

![blockchain](http://legendary.cdn.play8.io/learnpython/img/day11/d11-p1.png)

For instance, suppose we have a function called power. It receives two values ``x`` and ``y`` then returns the valued x<sup>y</sup>. We can call the function with the values 10 and 3, and put the return value of function in a variable ``pow`` as follows:


```python
pow = Power(10, 3)
```

Here, Power function will return 10<sup>3</sup> = 1000 and this value is put in the variable pow. We can write the entire program including the ``Power`` function as follows:

```python
def Power(x, y):
    prod = 1
    por i in range(y):
        prod *= x
    return prod

pow = Power(10, 3)
print(pow)
```

The function has to be defined above the code it's called. In this code, Power
function is defined between lines 1 and 5. Input and output types, and the name
of the function are defined in line 1: it receives two values, x and y. We write the operations in the body of the function which is indented; lines 2 to 5. It returns a value as indicated in line 5.

<br>

<center> - 83 - </center>
