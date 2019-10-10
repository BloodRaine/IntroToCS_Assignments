# The Minion Game

Kevin and Stuart want to play the 'The Minion Game'.

# Game Rules
- Both players are given the same string, *S*.
- Both players have to make substrings using the letters of the string *S*.
- Stuart has to make words starting with consonants.
- Kevin has to make words starting with vowels.
- The game ends when both players have made all possible substrings.

# Scoring
A player gets +1 point for each occurrence of the substring in the string *S*.
For Example:
String *S* = BANANA
Kevin's vowel beginning word = ANA
Here, ANA occurs twice in BANANA. Hence, Kevin will get 2 Points. 

For better understanding, see the image below: 

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Your task is to determine the winner of the game and their score.

# Output Format
Print one line: the name of the winner and their score separated by a space.
If the game is a draw, print Draw.

# Sample Output
```
OUTPUT> Stuart 12
```

**Note : Vowels are only defined as *"AEIOU"*. In this problem, *Y* is not considered a vowel.**

# Helpful Hints
start by importing the Random and string libraries as follows:
```
import random
import string
```

To generate a randomized string use:
```
stringLength = 6
letters = string.ascii_uppercase
''.join(random.choice(letters) for i in range(stringLength))
```
