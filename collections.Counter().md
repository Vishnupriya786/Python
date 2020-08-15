# collections.Counter()

```
Raghu is a shoe shop owner. His shop has X number of shoes.
He has a list containing the size of each shoe he has in his shop.
There are N number of customers who are willing to pay xi amount of money only if they get the shoe of their desired size.

Your task is to compute how much money Raghu earned.
```
```
Sample Input

10
2 3 4 5 6 8 7 6 5 18
6
6 55
6 45
6 55
4 40
18 60
10 50
```
```
Sample Output

200
```
```

from collections import Counter
total_size = int(input())
avail_size =  list(map(int, input().split()))
    
n = int(input())
a_lis = []
for i in range(n):
    a =  (list(map(int,input().split())))
    a_lis.append(a)
prob_size = []
price = []
for i in range(n):
    prob_size.append (a_lis[i][0])
    price.append(a_lis[i][1])

count = 0
for i in range(n):
    if prob_size[i] in avail_size:
        count += price[i]
        avail_size.remove(prob_size[i])
print (count)

```
