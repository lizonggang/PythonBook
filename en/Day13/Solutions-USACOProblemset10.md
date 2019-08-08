### Solution for "Cow Counting"

Before presenting the solution, I will go through the sample case in the problem: 
10 1 
 
In this case, we must print the largest of the first 10 numbers not containing a 1. To do this, we loop through the positive integers, skipping integers with a 1 and going through 10 numbers in total. Finally, we print the largest of those 10 numbers and get: 
22 

Now, we must generalize this solution to ``N`` numbers skipping the digit ``L`` First, we create a method that identifies if a given number, ``a​``, contains the digit ``L​``. The method, called ``​seen​``, uses mod 10 to check if the last digit of the number is ``L​`` and then uses integer division to remove the last digit. This way, it can check if any of the digits in the number is ``L​``.  

```python
seen(a, L): 
    while a > 0: 
        if a % 10 == L: 
            return true 
        a = a/10 
    return false
```

Another way to implement this method is to use strings and iterate through the string and check if it contains the character ``L``: 

```python
seen(a, L): 
    a = string of a 
    L = character of L 
    for i from 0 through n-1 
        if a[i] = L: 
            return true 
    return false 
```

Next, we build the main method that actually prints the answer. The main method goes through a total of ``​n`` integers while skipping integers that contain ``L​``. The largest integer is stored in  ``counter​`` and printed out after a total of ``n​`` integers not containing ​``L​`` have been found.  
       ​                    
```python
counter = 1 
read n, L 
for i from 1 through n: 
    while seen(counter, L): 
        counter = counter + 1 
 
    counter = counter + 1  
 
print counter         
```

---

<br>

 

### Solution for "Switching Lights"
 
We need to keep the states of all the lights and implement the requested operations. We'll use false to  represent a light being off and true to represent the light being on. First, let's set up a boolean array for the 
lights and read the number of lights and operations. 

```python
read N, M 
array lights[501] 

//set the lights to all be off 
for i from 1 to N: 
    lights_i = false 
```

Now we need to read the input, and process it. 

```python
for i from 1 to M: 
    read instruction, s, e 
```

In the first case, we need to switch every light, so we should iterate through them: 

```python
if instruction == 0: 
    for light from s to e: 
```

To toggle a light, we need to set it to the opposite state it is already at, which can be accomplished with the binary NOT (!) operation. 

```python
lights_light = not lights_light 
```

In the other case, we again need to iterate through, this time keeping a count of all the lights that are on. We then need to output our count. 

```python
if instruction == 1: 
    count = 0 
    for light from s to e: 
        if(lights_light)           // this will be true if the light is on 
            count = count + 1 
    output count 
```

We put this all together to get our final solution: 

```python
read N, M 
array lights[501] 


for i from 1 to N: 
    lights_i = false 

for i from 1 to M: 
    read instruction, s, e 
    if instruction == 0: 
        for light from s to e: 
            lights_light = not lights_light 
    if instruction == 1: 
        count = 0 
        for light from s to e: 
            if(lights_light) 
                count = count + 1 
        output count 
```



