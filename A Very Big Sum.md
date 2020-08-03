# A Very Big Sum

```
Complete the aVeryBigSum function in the editor below. It must return the sum of all array elements.

aVeryBigSum has the following parameter(s):

int ar[n]: an array of integers .
```
```
Sample Input

5
1000000001 1000000002 1000000003 1000000004 1000000005
```
```
Output

5000000015
```
```
def aVeryBigSum(arr):
    return (sum(arr))
n = int(input())
arr = list(map(int, input().rstrip().split()))
result = aVeryBigSum(arr)
print(result)

```
