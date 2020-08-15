# itertools.product()

```
You are given a two lists A and B. Your task is to compute their cartesian product A X B.
```
```
Sample Input

 1 2
 3 4
```
```
Sample Output

 (1, 3) (1, 4) (2, 3) (2, 4)
```
```
from itertools import *
a = list(map(int, input().split()))
b =list(map(int, input().split()))
res =(list(product(a,b)))
for i in res:
    print (i, end = " ")
```
