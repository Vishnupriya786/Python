# Tuples

```
Given an integer,n , and n space-separated integers as input, create a tuple,t , of those n integers. Then compute and print the result of (hash(t)).
```
```
Sample Input 

2
1 2

```
```
Sample Output 

3713081631934410656
```
```
n = int(input())
lis = input().split()
a=[]
for i in lis:
     i = int(i)
     a.append(i)

print (hash(tuple(a)))
```
