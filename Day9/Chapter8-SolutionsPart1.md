**问题1: 练习8.1**

```python
name = input()
for counter in range(5):
    print("Your name is " + name + ".")
```
<br>

**问题2: 练习 8.1**

```python
name = input()
n = int(input())
for counter in range(n):
    print(name)
    # slide the name with one blank each time
    name = " " + name
```

<br>

**问题3: 例子8.2**

```python
name = input()
n = int(input())
name = + " " + name + " "
for counter in range(n):
    name = "*" + name + "!"
    print(name)
```

<br>

**问题4: 例子8.3**

```python
numl = int(input())
num2 = int(input())
op = input()
if op == "+"：
    result = numl + num2
if op == "-"：
    result = numl - num2
if op == "*"：
    result = numl * num2
if op == "/"：
    result = int(numl / num2)
print(result)
```

<br>

**问题5:**

```python
s = input()
# if the s1ze of the string is even
if len(s) % 2 == 0:
    print("No middle character!")
else:
    middle = int(len(s)/2)
    print(s[middle])
```

<br>

**问题6:**

```python
n = int(input())
words = [""] * 100
# read n words from the input
for counter in range(n):
    words[counten] = input()
# write words on the screen in reverse order
for counter in range(n-l, -1, -1):
    print(words[counter])
```

<br>

**问题7:**

```python
wordl = input()
word2 = input()
word3 = input()
if wordl < word2 and word2 < word3:
    print(wordl + "\n" + word2 + "\n" + word3)
if wordl < word3 and word3 < word2:
    print(wordl + "\n" + word3 + "\n" + word2)
if word2 < wordl and wordl < word3:
    print(word2 + "\n" + wordl + "\n" + word3)
if word2 < word3 and word3 < wordl:
    print(word2 + "\n" + word3 + "\n" + wordl)
if word3 < wordl and wordl < word2:
    print(word3 + "\n" + wordl + "\n" + word2)
if word3 < word2 and word2 < wordl:
    print(word3 + "\n" + word2 + "\n" + wordl)
```

<br>

**问题8:**

```python
# 问题1:
"""
    str = input()
    rev = ""
    for ch in str :
        rev = ch + rev
    print(rev)
"""
############################
# 问题2:
# write string in backward order
str = input()
for counter in range(len(str)-l,-l,-l):
    print(str[counter], end = ""）
############################
# 问题3:
"""
    str = input()
    print(str[::-1])
"""
```

<br>

**问题9:**

```python
str = input()
n = int(input())
rev = ""
for ch in str:
    rev = ch + rev
for i in range(n):
    print(rev)
```

<br>

**问题10:**

```python
str = input()
a,b,n = input().split()
a = int(a)
b = int(b)
n = int(n)
sub = ""
#get the substring starting from a and length b
for counter in range(b):
    sub += str[a + counter]
for i in range(n):
    print(sub)
```

**另一个方法:**

```python
str = input()
a,b,n = input().split()
a = int(a)
b = int(b)
n = int(n)
# str[a:a+b] is the substring of s from index a to index a+b (excluding a+b).
for i in range(n):
    print(str[a:a+b])
```

<br>

**问题11:**

```python
s1 = input()
s2,a,n = input().split()
a = int(a)
n = int(n)
# str[a:a+b] is the substring of s from index a to index a+b (excluding a+b).
s1 = sl[0:a] + s2 + sl[a:len(sl)]
for i in range(n):
    print(s1)
```

<br>

**问题12:**

```python
s = input()
a,b,n = input().split()
a = int(a)
b = int(b)
n = int(n)
# str[a:a+b] is the substring of s from index a to index a+b (excluding a+b).
s = s[0:a] + s[a + b : len(s)]
for i in range(n):
    print(s)
```

<br>
        
**问题13:**

```python
s1 = input()
s2,a,b,n = input().split()
a = int(a)
b = int(b)
n = int(n)
# str[a:a+b] is the substring of s from index a to index a+b (excluding a+b).
s1 = sl[0:a] + s2 + sl[a+b : len(sl)]
for i in range(n):
    print(s1)
```

<br>

**问题14:**

```python
s1 = input()
s2 = input()
found = sl.find(s2)
if found == -1 :
        print("not found!")
else :
        print(found)
```

另一个方法:

```python
s1 = input()
s2 = input()
found = -1
if len(sl) >= len(s2):
    # search for s2 in s1
    for counter in range(len(sl)-len(s2)+1):
        # check if s2 is a substring of s1,
        # starting from the counter's pos1tion
            if (found == -1 and s1[counter:counter+len(s2)] == s2) :
                found = counter
if found == -1:
    print("not found!")
else:
    print(found)
```

<br>

**问题15： 练习 8.10**

```python
n = int(input())
# read n words from the input file
words = [ "" ] * n
for counter in range(n):
    words[counter] = input()
# read the string to be deleted
d = input()
# search the substring in each word and if found just delete the first occurance
for counter in range(n):
    search = words[counter].find(d)
    if (search != -1 ) :
        words[counter] = words[counter][0:search] + words[counter][search+ len(d): len(words[counter])]
# write output file
for counter in range(n):
    print(words[counter])
```
