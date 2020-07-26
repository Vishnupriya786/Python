# CamelCase

```
Alice wrote a sequence of words in CamelCase as a string of letters,n , having the following properties:

It is a concatenation of one or more words consisting of English letters.
All letters in the first word are lowercase.
For each of the subsequent words, the first letter is uppercase and rest of the letters are lowercase.
Given n, print the number of words in n on a new line.
```
```
Sample Input

saveChangesInTheEditor
```
```
Sample Output

5
```
```
def camelcase(n):
    count = 0
    for letters in n:
        if letters.isupper():
            count += 1
    print (count + 1)
n = list(input())
camelcase(n)

```
