# Simple Array Sum

```
Given an array of integers, find the sum of its elements.
The first line contains an integer,n , denoting the size of the array.
The second line contains n space-separated integers representing the array's elements.
```
```
Sample Input

6
1 2 3 4 10 11

```
```
Sample Output

31
```
```
def simpleArraySum(array):
    total= sum(array)
    return total
ar_count = int(input())

array = list(map(int, input().rstrip().split()))

result = simpleArraySum(array)
print(result)

```
