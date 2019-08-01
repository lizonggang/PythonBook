# Guess My Number Game

You will make guess my number game. The game is a two player game; 

- One is "picker" the other is "guessor".
- Picker picks a integer number between 1 and 100 inclusively and the guessor guesses it.
- The goal for the guessor is to guess picker's number in the least number of guesses.
- After each guess, picker provides feedback such as "go down", "go up", or "correct"
  - "go down" means the picker's number is less than the guessor's guess
  - "go up" means the picker's number is greater than the guessor's guess
- The game finishes when guessor correctly guesses the picker's number.


## Task 1 (%40 of the total points):

- Read an integer number N. It's guaranteed that the user will enter the number between 1 and 100.
- Continuously read guesses from the user until the user enters the correct number N.
- Finally print the number of guesses.

**Sample Input and Output:**

('>' indicates the user input)

```python
>87
guess:
>34
go up
guess:
>56
go up
guess:
>78
go up
guess:
>90
go down
guess:
>83
go up
guess:
>89
go down
guess:
>88
go down
guess:
>87
correct!
8
```

<br>

## Task 2 (%60 of the total points):
If the guess is less than 1 or greater than 100 let the user know it is invalid. Number of guesses will be calculated based on only valid entries.

**Example:**

```python
>87
guess:
>34
go up
guess:
>56
go up
guess:
>104
invalid
>110
invalid
>90
go down
guess:
>-40
invalid
>0
invalid
>1
go up
guess:
>100
go down
guess:
>87
correct!
6
```

