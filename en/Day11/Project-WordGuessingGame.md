## Word Guessing Game

Write a one player word guessing game.

#### Game design:
1. Initially the boss enters a secret word.
2. The secret word will be masked by asterisks (*) on screen -- one asterisk for each letter.
3. Initially the player has 5 lives.
4. In each turn, the player enters a letter. If the secret word doesn’t contain the letter, the player will lose one life.
5. In each step you need to print the used letters and unmask the letters the player found in the secret word.
6. Finish the program when the life is 0 (player loses) or player finds the entire secret word (player wins).

### Task 1 (%40 of the total points):
Design the game and check for draw. In this task,  the test data will always end with a tie. You don’t need to check for the winner or tie. You can finish the game with a message “Tie!”.

**Sample Input and Output:**
('>' indicates the user input)

```
>computer

********
Enter a lower case letter:
>q
Life left:4
So far you have used these letters:q

********
Enter a lower case letter:
>e

******e*
Life left:4
So far you have used these letters:qe

******e*
Enter a lower case letter:
>c

c*****e*
Life left:4
So far you have used these letters:qec

c*****e*
Enter a lower case letter:
>r

c*****er
Life left:4
So far you have used these letters:qecr

c*****er
Enter a lower case letter:
>t

c****ter
Life left:4
So far you have used these letters:qecrt

c****ter
Enter a lower case letter:
>y
Life left:3
So far you have used these letters:qecrty

c****ter
Enter a lower case letter:
>u

c***uter
Life left:3
So far you have used these letters:qecrtyu

c***uter
Enter a lower case letter:
>i
Life left:2
So far you have used these letters:qecrtyui

c***uter
Enter a lower case letter:
>o

co**uter
Life left:2
So far you have used these letters:qecrtyuio

co**uter
Enter a lower case letter:
>p

co*puter
Life left:2
So far you have used these letters:qecrtyuiop

co*puter
Enter a lower case letter:
>a
Life left:1
So far you have used these letters:qecrtyuiopa

co*puter
Enter a lower case letter:
>s
Life left:0
So far you have used these letters:qecrtyuiopas
You lost!
```

### ask 2 (%60 of the total points):
In addition to Task 1, this time the player will enter a lowercase letter however it is not guaranteed that the player will enter a distinct letter each time. You need to warn the player if the player enters a used letter.

**Sample Input and Output:**
('>' indicates the user input)

```
>alphabet

********
Enter a lower case letter:
>a

a***a***
Life left:5
So far you have used these letters:a

a***a***
Enter a lower case letter:
>t

a***a**t
Life left:5
So far you have used these letters:at

a***a**t
Enter a lower case letter:
>a
You have used this letter before. Please enter again:
>t
You have used this letter before. Please enter again:
>e

a***a*et
Life left:5
So far you have used these letters:ate

a***a*et
Enter a lower case letter:
>l

al**a*et
Life left:5
So far you have used these letters:atel

al**a*et
Enter a lower case letter:
>p

alp*a*et
Life left:5
So far you have used these letters:atelp

alp*a*et
Enter a lower case letter:
>h

alpha*et
Life left:5
So far you have used these letters:atelph

alpha*et
Enter a lower case letter:
>g
Life left:4
So far you have used these letters:atelphg

alpha*et
Enter a lower case letter:
>b

alphabet
Life left:4
So far you have used these letters:atelphgb
You won!
```

