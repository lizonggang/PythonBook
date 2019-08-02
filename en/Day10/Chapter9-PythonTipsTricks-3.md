###### python Tips and Tricks

```python
print(number)
```

Similarly, we can check if the calculation of the divisors is correct by outputting the values in the array as follows after line 9:

```python
for counter in range(index):
    print(divisors[counter])
```

We will immediately notice that it is wrong since the values in the divisor array are wrong. So we carefully check the divisor calculation and see the mistake in line 7.

```python
divisors[index] == divisor
```

After running in the next step, we will see the number itself as one of its divisors. Then we will check the ``for`` loop again, and will find out the range is wrong and it has to be upto ``number``：

```python
for divisor in range(2, number + 1):
```

We will check it again after correcting the mistake. Next debugging step is after line 14:

```python
print(sum)
```

We will see that the sum is not correct, and notice the mistake in the for loop:

```python
sum = divisors[counter]
```

It has to be “+=” instead of “=” Finally, the program will produce the desired output.

> [!NOTE]
>  Some of the common mistakes can be listed as follows:
> - Wrong initialization / range of the loop counter
> - Use of “==” instead of“=”
> - Simple mistakes with conditions that lead undesired output or infinite loop
> - Wrong update of the loop counter

Always remember a code might be syntax error free however; it might not work
properly to create the desired output. In other words, your code might compile but it might have some logical mistakes at the same time. In that case, it is
recommended you add ''prints" and print the values of variables inside suspicious loops and conditionals to track the changes of variables. Also, you may add some kind of notes such as ``print`` ("T``his is the 1st condition and I am here``") so that you will make sure whether or not the compiler executed that specific if condition.


#### Congratulations - end of lesson reached

Well done!

<br>

<center> - 77 - </center>

