### Solution for "Even? Odd?"


Uh oh! These numbers are much too big to store in our normal integer type. But do we need the whole number? You might recall from math class that we can determine whether a number is even or odd just by looking at the last digit. We can use that strategy in this problem, and process the integers they give us as
strings.

**Note for Python:** This problem is quite easy in Python, since we have no restriction on the size of integers that we can use. Instead of reading the integers in as a string and then using only the last digit, we can just use the
modulo operator directly on the number.

```python
read N
for i from 0 to N-l:
      read t
      if t % 2 == 0:
            print("even")
      else :
            print("odd")
```

Essentially, this problem is N different problems, all in one input. We can solve each independently of the other. First, we read the number of cases and iterate through each.

```python
read N
for i from 1 to N:
```

In Python, you don’t need to do anything extra. But in C++ and Java, we need to do a couple things to check the last digit. We need to read the integer as a string in C++/Java. This has different syntax for each language, shown below.

C++|Java
-|-                        
string s;|String s = myScanner.next();
cin >> s;|                            

Then, we have to get the last digit, as a character.

C++|Java
-|-                 
char lastDigit = s[s.size()-1];|char lastDigit =       
&nbsp;|s.charAt(s.length()-1);


Now, convert the last digit to an integer. We can do this by subtracting the character 'O'. For example, '4'-'0' would be 4. Keep this trick in mind - it is often used in programming.


C++/Java:
```
int digit = (int)(lastDigit-'0');
```

Finally, we check if the digit is even or odd, and output accordingly. We will use pseudo-code again:

```python
if digit%2==0: //even
    output "even"
else:             //odd
    output "odd"
```

---

<br>

### Solution for "Adding Commas"

Before we go through the full solutions, let’s take a look at the sample case:
``153920529``

To find the solution for this particular case, we move backward through the number adding a comma each time the number of digits we have seen is divisible by 3 unless we are at the beginning of the number. After all the commas have been added, we get:
``153,920,529``

One possible way to solve this problem is to first store the number as a string. Then, use a for-loop to iterate through the string 3 characters at a time, backward, adding commas at each iteration. This solution is demonstrated below:

```python
read m
n = length(m)
answer = ""
//adding commas by groups of 3
for i from 0 through n-4 incrementing i by 3:
    a = substring of m from n-i-3 to n
    answer = "," + a + answer


// after the last comma is added, there is a bit of the original number

II    from the beginning that needs to  be added to answer
if n mod 3=0:                                            
    b = substring of m from 0 through 3                 
else:                                                     
    b = substring of m from 0 through  n mod 3          

print b + answer
```

In this solution, within the for-loop, we make i go through n-4 instead of n-3 to avoid placing a comma at the beginning of numbers in which the total number of digits is divisible by 3. For example, we want to avoid producing, ``153,920,529`` instead of ``153,920,529``.


---

<br>


                                                                              

### Solution for "String Function Encoding"

 
Bessie's function f(N, S) has two arguments: a string S and an integer N. The function is returns a string which  is a substring of the original string from index N to the end + the original string. Note that the function uses  0-based indexing. For example f(2, "COW") = "W" + "COW" = "WCOW"; applying it again: f(2, "WCOW") =  "OW" + "WCOW" = "OWWCOW". Applying the function for the third time: f(2, "OWWCOW") = "WCOW" +  "OWWCOW" = "WCOWOWWCOW". This explains the first sample output.  
 
For each string, repeat Bessie’s function the specified amount of times using a loop. To implement Bessie’s function, create a new string by concatenating a substring of the original string with the original string. 

```python
read Z 
for i from 1 to Z: 
    read N C curStr 
    for j from 1 to C: 
        curStr = substring of curStr from N to end (0-indexed) + curStr 
    print curStr 

```
