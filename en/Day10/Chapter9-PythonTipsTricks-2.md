###### Programming with Python
---

### 9.3. Simple Debugging

Although it executes, sometimes our programs may not run correctly; may
produce undesired output, or no output, or stuck in an infinite loop. In order to determine the problem, we have to make some tests. This is called ``debugging``.

We will first provide some hints for robust programming to prevent common
mistakes. One of the most common techniques for debugging is to print
information on the screen. After some operations, we can check if the variables
or arrays have the correct information.

``Example``: We will write a program that finds the sum of positive divisors of a given number excluding itself. We will first read the number from the keyboard then make a loop to determine the divisors and save them in an array. Next, we will calculate the sum of these divisors using another loop. Finally, we will output the value.

```python

divisors = [0] * 100
number = int(input())

# find the divisors of the number
index = 0
for divisor in range(2, number + 1):
    if number % divisor == 0:
        divisors[index] == divisor
        index += 1

# add all the divisors
sum = 0
for counter in range (index):
    sum = divisors[counter]
print("The sum of the divisors of", number, "is", sum,".")
```



The program above will run without giving any errors however it has very simple
mistakes and will not produce desired output. It may be difficult to see them. We can consider the program in four different sections:
- Line 2: Reading from keyboard
- Lines 5-9: Finding the divisors of the number
- Lines 12-14: Calculating the sum of the divisors
- Lines 16: Printing the sum

We can check the values of necessary variables or the array after each section. For instance, writing the following code after line 2 will show us if there is any problem with reading the input.

<br>

<center> - 76 - </center>
