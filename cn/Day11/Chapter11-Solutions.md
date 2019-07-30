此页面包含除可选解决方案之外的解决方案：

**问题1: 例子11.1**

```python
def NumLetters(s):
    count =0
    for letter in s:
        if (letter >= 'A' and letter <= 'Z') or (letter >= 'a' and letter <= 'z'):
            count += 1
    return count
```

<br>

**问题2: 练习11.1**

```python
def UpperCase(s):
    s = s.upper()
    return s
```

<br>

**问题3: 练习11.2**

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

**问题4: 练习11.3**

```python
def Reverse(s):
    return s[::-1]
```

<br>

**问题5: 练习11.4**

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

**问题6: 例子11.2**

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

**问题7: 练习11.5**

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

