# itertools.combinations_with_replacement()

```
You are given a string S.
Your task is to print all possible size k replacement combinations of the string in lexicographic sorted order.
```
```
Sample Input

HACK 2
```
```
Sample Output

AA
AC
AH
AK
CC
CH
CK
HH
HK
KK
```
```
from itertools import *
a = input().split()
word =  a[0]
word = sorted(word)
n = int(a[1])

res = (list(combinations_with_replacement(word,n)))
for i in res:
    print ("".join(i))
```
