**问题1: 练习8.11**

```python
n = int(input())
spend = input().split()
for counter in range( n ) :
    spend[counter] = int(spend[counter])
m, shoptype = input().split()
m = int(m)
# determine the bonus points per dollar
bonus = 1
if shoptype == "bakery":
    bonus = 5
elif shoptype == "produce":
    bonus = 2
# calculate the total bonus points
points =0
for counter in range(n):
    if spend[counter]>m :
        points = points + bonus*spend[counter]
print(points)

```

<br>

**问题2: 练习8.12\***

```python
s = input()
cnt = 0
# gc over the entire string
for ch in s:
    # if the current character is an uppercase or lowercase letter
    if (ch>='A' and ch<='Z') or (ch>='a' and ch<='z')：
        cnt+=1
print(cnt)
```

<br>

**问题3: 练习8.13\***

```python
s = input()
print(s.upper())
```

问题4: 练习8.14**

```python
   s1, s2 = input().split()
   # convert s1 to uppercast
   s1 = s1.upper()
   # convert s2 to uppercast
   s2 = s2.upper()
   if s1==s2:
        print("same")
   else :
        print("not same")
```

<br>

**问题5: 练习8.15\***

```python
s = input()
cnt = 0
# go over the entire string
for ch in s:
    # if the current character is a digit
    if ch>='0' and ch<='9':
        cnt+=1
print(cnt)
```

<br>

**问题6: Example 8.17\***

```python
s1,s2 = input().split()
vowels="aeiouAEIOU"
cntl = 0
cnt2 = 0
# count the vowels in first string
for ch in s1:
    if vowels.find(ch)!=-1:
        cnt1+=1
    # count the vowels in second string
for ch in s2:
    if vowels.find(ch)!=-1:
        cnt2+=1

if cntl==cnt2:
    print("Same number of vowels.")
else:
    print("Not same number of vowels.")
```

<br>

**问题7: 练习8.19\***

```python
n,c = input().split()
n = int(n)
row = ""
# generate one row in a string
for i in range(n):
    row+=c
# output the row n times
for i in range(n):
    print(row)
```

<br>

**问题8: 练习8.20\***

```python
n, c = input().split()
n = int(n)
row = ""
# generate the top and bottom rows
topbottom = ""
for i in range(n):
    topbottom+=c
# generate the blanks in the middle rows in a string
middle = ""
for i in range(n-2):
    middle+=' '
print(topbottom)
# output the middle rows n-2 times
for i in range(n-2):
    print(c+middle+c)
print(topbottom)
```

<br>

**问题9: 练习8.21\*\***

```python
n,m = input().split()
n = int(n)
m = int(m)
maze = [""] * n
for i in range(n):
    # store maze in a string array
    maze[i] = input()
path = input()
# (r,c) is the location in the maze
# valid: stores the validity of the path
r=l
c=l
valid=l
# walk through the path
for ch in path:
    # update the location in the maze
    if ch == 'u':
        r-=1
    if ch == 'd':
        r+=1
    if ch == 'l' :
        c-=1
    if ch == 'r' :
        c+=1
    # check if reached the exit
    if r==1 and c==m-1 :
        # if still remaining path
        if ch!=path[len(path)-1]:
            valid=0
        break
    # it's invalid path if hits to wall
    if maze[r][c]=='#':
        valid=0
        break
# the path has to finish at (1,m-1) without hitting any walls
if valid==0 or r!=1 or c!=m-1 :
    print("Wrong path!")
else :
    print("Right path!")
```