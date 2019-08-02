## Chapter 11: Solutions

This page contains the solutions except the optional ones:

**Question 1: Example 11.1**

```python
def NumLetters(s):
    count =0
    for letter in s:
        if (letter >= 'A' and letter <= 'Z') or (letter >= 'a' and letter <= 'z'):
            count += 1
    return count
```

<br>

**Question 2: Exercise 11.1**

```python
def UpperCase(s):
    s = s.upper()
    return s
```

<br>

**Question 3: Exercise 11.2**

```python
def SameWords (sl,s2):
    si = sl.upper()
    s2 = s2.upper()
    if sl==s2:
        return 1
    else:
        return 0
```

<br>

**Question 4: Exercise 11.3**

```python
def Reverse(s):
    return s[::-1]
```

<br>

**Question 5: Exercise 11.4**

```python
# function returns number of vowels
def NumV〇Mels(s):
    count =0
    s = s.upper()
    # check if vowel
    for i in s :
        if i == 'A' or i == 'E' or i == 'I' or i == '0* or i == 'U* :
            count+=l
    return count
a,b,c=input().split()
if NumVowels(a) == NumVowels(b) and NumVowels(a) == NumVowels(c):
    print("Same number of vowels.")
else :
    print("Not same number of vowels.")
```

<br>

**Question 6: Example 11.2**

```python
def NumOfDigits(s):
    digits =0
    for letter in s:
        if letter >= '0' and letter <= *9':
            digits += 1
    return digits
sl,s2 = input().split()
print (NumOfDigits(sl) + Num0fDigits(s2))
```

<br>

**Question 7: Exercise 11.5**

```python
# prints a square with the given size and character
def PrintSquare(a,ch):
    for i in range (a):
    # print one line
    for j in range(a):
        print(ch, end="")
    print()
x,y,ch = input().split()
x = int(x)
y = int(y)
PrintSquare(x, ch)
print()
PrintSquare(y, ch)
```

