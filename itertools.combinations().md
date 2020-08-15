# itertools.combinations()

```
You are given a string S.
Your task is to print all possible combinations, up to size k, of the string in lexicographic sorted order.
```
```
Sample Input

HACK 2
```
```
Sample Output

A
C
H
K
AC
AH
AK
CH
CK
HK
```
```
from itertools import *
a = input().split()
word =  a[0]
word = sorted(word)
n = int(a[1])
for i in range(1,n+1):
    res = (list(combinations(word,i)))
    for j in res:
        print ("".join(j))
```
