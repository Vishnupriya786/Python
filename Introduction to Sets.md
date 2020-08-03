# Introduction to Sets

```
Now, let's use our knowledge of sets and help Mickey.

Ms. Gabriel Williams is a botany professor at District College. One day, she asked her student Mickey to compute the average of all the plants with distinct heights in her greenhouse.

Formula used:

      average = sum of distinct heights/total number of distinct heights
```
```
Sample Input

10
161 182 161 154 176 170 167 171 170 174

```
```
Sample Output

169.375
```
```
def average(arr):
    arr = set(arr)
    return(sum(arr)/len(arr))
n = int(input())
arr = list(map(int, input().split()))
result = average(arr)
print(result)
```
