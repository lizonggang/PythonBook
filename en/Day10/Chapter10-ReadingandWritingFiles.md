###### Reading / Writing Files
---

# <center>Chapter 10: Reading / Writing Files</center>
---


### 10.1. File Streams

Consider the following example:

```python
age = int(input())
print("You are " + str(age) + " years old.")
```

You will see on the screen as follows:

```
Hi, how old are you?
14
You are 14 years old.
```

``print()`` and ``input()`` flinctions are used to interact with the user. This way, we write sentences to the screen to ask questions or to say something and get answers from the user. What we write to the screen is called '``output``' and what we are reading from the user is '``input``' Computer programs get the input, process it, and print the output. Sometimes, reading from the keyboard and writing to the screen is not practical; every time the program runs we have to enter from keyboard. Instead, we can use files; we can write our input once into the files and the program reads from the file each time. Moreover, we can save the output in another file for further use instead of writing to screen.

```python
fin = open("infile.txt", "r")
fout = open("outfile.txt", "w")
age = int(fin.readline())
fout.write("You are " + str(age) + "years old.\n")
fout.close()
```

```
infile.txt:                 outfile.txt
14                           You are 14 years old.
```

At line 1, we open our input file whereas we open the output files at line 2. Input file is indicated with the “``r``” value in ``open()``. Similarly, output file is indicated with “``w``”. At line 3, we use ``readline()`` to read the input from the file instead of the keyboard. At line 4, we use ``write()`` instead of ``print()`` to write the output to the file instead of the screen. Note that we used “``\n``” at the end. In Python, “``\n``” is the end-of-line character, write " doesn’t press enter as ``print()`` does. So we added it manually at the end. The last thing is to close the output file as shown in
line 5.

Before running the program we open ``infile.txt ``and write the required input in it. In the example above, the input is 14. Since we assume that the input is already in the file when we run the program, we do not need to inform the user to enter the input as we did in the first example.

<br>

<center> - 79 - </center>
