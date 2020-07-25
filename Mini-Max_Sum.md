# Mini-Max Sum

```
Given five positive integers, find the minimum and maximum values that can be calculated by summing exactly four of the five integers. Then print the respective minimum and maximum values as a single line of two space-separated long integers.
```
```
Sample Input

1 2 3 4 5
```
```
Sample Output

10 14
```
```
def miniMaxSum(arr):
    ascen_arr = sorted(arr)
    min = ascen_arr[0] + ascen_arr [1] + ascen_arr[2]+ascen_arr[3]
    max = ascen_arr[1] + ascen_arr[2]+ascen_arr[3] + ascen_arr [4]
    print (min,max)
arr = list(map(int, input().rstrip().split()))
miniMaxSum(arr)    

```
