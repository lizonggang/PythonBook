###### Variables — Char and String
---

The above code adds one more ‘*’ in the front and ‘!’ at the end of the string each time.
To check whether two strings are equal or not equal, we use ‘==’ or1 ‘!=’ operators
as in integer variables.

Example 8.3: Write a program that reads two numbers and an arithmetic operator (+, —, *, /) from the keyboard. The program applies the operation to the numbers and prints the result on the screen:

```
Sample input:        Sample output:
5                    105
21
*
```

解决方案：

```python
numl = int(input())
num2 = int(input())
op = input()
if op =="+"：
    result = numl + num2
if op =="-"：
    result = numl  -  num2
if op =="*"：
    result = numl * num2
if op =="/"：
    result = numl / num2
print(result)
```

We can also use ‘<’, '<=’, ‘>=’, and ‘>’ operators to compare the alphabetical order of the strings.

```python
if string1 < string2：
    print("string1 is before string2")
else:
    print("string1 is not before string2")
```

The code fragment above prints ‘``string1 is before string2``' if ``string1`` is
alphabetically comes before ``string2``. Suppose ``string1`` is ‘``try it``’ and ``string2``
is ‘``trial``’ then the program prints ‘``string1 is not before String2``’.

> [!NOTE]
> Be careful that capital letters come before lower-case letters in computers. 
> For instance, if ``string1`` is ‘``Zinc``’ and ``string2`` is ‘``about``’ then the program prints ‘``string1 is before string2``’,since ‘Z’ is before ‘a’.


<br>

<center> - 63 - </center>
