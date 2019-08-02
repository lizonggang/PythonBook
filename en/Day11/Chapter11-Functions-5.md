###### Functions
---

Exercise 11.5: Write a program that reads two numbers at, >* and a character c from the keyboard. The program outputs two squares with the sizes x and y filled with character c.

```
input:                      output:
3 5 #                       ###
                            ###
                            ###

                            #####
                            #####
                            #####
                            #####
                            #####
```

### 11.3. Local / Global Variables

Variables defined in a function can only be used in that function. Look at the
example below:

```python
def Power(x, y):
    z = 1
    for i in range (y):
        z *= x
    return z

x =int(input())
z = 11
print(Power(10, x))
print(z)
```

In this example, variable y defined in line 1 belongs to the Power function hence
it can't be used in main. The variable x is defined in lines 1 and 7. x in line 1,
belongs to the Power whereas the other one belongs to the main code. Be careful
that in line 16, the value ofx in main code goes to the variable^ in the Power
function, x of the Power function receives the value 10 from line 9. Similarly, z
in line 8 belongs to the main code and it is not affected from z in the Power
function. Hence, line 10 will print 'll' for the value ofz since it is initialized with
'll' in line 8. We can consider x's in the main code and Power as two different
boxes with the same names in two different rooms. Same goes for z.

Exercise J!.6: What is the output of the following program if user enters 'I8cakes'和'try911' from the keyboard respectively.

```python
def NumOfDigits(s, x)
    digits = 0
    for letter in s:
        if letter >= 101 and letter <= '9';
            digits += 1
    return digits + x
x=3
s = input()
t = input()
print(NumOfDigits(t, x + x))
```

<br>

<center> - 87 - </center>