# Plus Minus

```
Given an array of integers, calculate the ratios of its elements that are positive, negative, and zero. Print the decimal value of each fraction on a new line with 6 places after the decimal.
```
```
Sample Input

6
-4 3 -9 0 4 1        
```
```
Sample Output

0.500000
0.333333
0.166667
```
```
def plusMinus (arr):
    positive_num =0
    negative_num= 0
    zero_num = 0
    for i in range(0,len(arr)):
        if arr[i]>0:
            positive_num += 1
        elif arr[i]<0:
            negative_num += 1
        else:
            zero_num += 1
    print ('%.6f'%(positive_num/n))
    print ('%.6f'%(negative_num/n))
    print ('%.6f'%(zero_num/n))


n = int(input())
arr = list(map(int, input().rstrip().split()))
plusMinus(arr)
```
