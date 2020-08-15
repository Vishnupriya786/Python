# itertools.permutations()

```
You are given a string S .
Your task is to print all possible permutations of size k  of the string in lexicographic sorted order.
```
```
Sample Input

HACK 2
```
```
Sample Output

AC
AH
AK
CA
CH
CK
HA
HC
HK
KA
KC
KH
```
```
from itertools import *
a = input().split()
word =  a[0]
word = sorted(word)
n = int(a[1])
res = (list(permutations(word,n)))
for i in res:
    print ("".join(i))
```
