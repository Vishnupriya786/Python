# The Minion Game

```
Kevin and Stuart want to play the 'The Minion Game'.

Game Rules

Both players are given the same string, S.
Both players have to make substrings using the letters of the string S.
Stuart has to make words starting with consonants.
Kevin has to make words starting with vowels.
The game ends when both players have made all possible substrings.
```
```
Sample Input

BANANA
```
```
Sample Output

Stuart 12
```
```
def minion_game(s):
    stuart_score = 0
    kevin_score = 0
    for i in range(len(s)):
        if s[i] in "AEIOU":
            kevin_score += len(s) - i
        else:
            stuart_score += len(s) - i
    
    if stuart_score > kevin_score:
        print("Stuart", stuart_score)
    elif kevin_score > stuart_score:
        print("Kevin",kevin_score)
    else:
        print("Draw")
s = input()
minion_game(s)
```
