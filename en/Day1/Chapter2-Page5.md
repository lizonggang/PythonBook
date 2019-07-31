###### Variables - Integer and Flag
---

### 2.4. Reading Numbers from Keyboard

In Python, we can read numbers from keyboard and put the number we read into
the variable boxes using ‘``input()``’.

Example 2.6: The following Python program puts two numbers read from
keyboard into ``box1`` and ``box2``. Then it puts the half of the sum of ``box1`` and ``box2``
into ``box3`` and it writes ``box3`` to the screen.

``python
box1 = int(input())
box2 = int(input())
box3 = (box1 + box2) / 2
print(box3)
``

In this code above, ``input()`` read one line of keyboard input and ``int()`` converts it
to an integer.

> [!NOTE]
> Be careful to enter each integer in one line-not both oftheminone line.
Otherwise the code will give error.



Exercise 2.4: Write a program that reads two numbers from the keyboard and put
them into ``box1`` and ``box2``. Then it puts the multiplication of ``box1`` and ``box2`` into ``box3`` and it writes ``box3`` to the screen.

We can also ask our question when reading input from keyboard as follows:

``python
age = int(input("please enter your age: "))
print("you will be", age + 40, "years old after 40 years")
``

For instance, if the user enters 14 from the keyboard, the output will be as
follows (red is the user input):

please enter your age: <font color=red>14</font> <br>
you will be 54 years old after 40 years

<br>

<center> - 17 - </center>

