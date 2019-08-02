###### Programming with Python
---


Example 10.1 Write a program reads a number N, and after that N numbers from a file. The program  will write the sum of these N numbers to the output file.

```
infile.txt:                 outfile.txt
5                           The sum is 16.
1 2 3 4 5 6
```

```python
fin = open("infile.txt", "r")
fout = open("outfile.txt", "w")
numbers = fin.readline().split()

sum = 0
for i in range(N):
    sum += int(numbers[i])
fout.write(str(sum)+"\n")
fout.close()
```

First we read ``N`` from the file at line 3. Then, we read all the numbers in one line and convert them to an array using ``split()``. Next, we add the numbers up in a ``for`` loop which traverses the array at lines 7-8. Finally at line 9, we write the answer to the file.

In the example above,N is given in the beginning. Suppose N is not given and we have to read the numbers till the end of the file.

```
infile.txt:                 outfile.txt
1                           The sum is 6.
2
3
4
5
6
```

We can write the program as follows:

```python
fin = open("infile.txt", "r")
fout = open("outfile.txt", "w")
N=0
numbers = [0]*100
while True:
    value = fin.readline()
    if not value:
        break
    numbers[N] = int(value)
    N += 1
sum = 0
for i in range(N):
    sum += int(numbers[i])
fout.write(str(sum) + "\n")
fout.close()
```

<br>

<center> - 80 - </center>

