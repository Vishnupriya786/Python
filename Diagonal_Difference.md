# Diagonal Difference

```
Given a square matrix, calculate the absolute difference between the sums of its diagonals.

```
```
Sample Input

3
11 2 4
4 5 6
10 8 -12
```
```
Sample Output

15
```
```
def diagnolDifference (arr):
    diagnol_1 = 0
    diagnol_2 = 0
    for i in range(0,n):
        diagnol_1 = diagnol_1 + arr[i][i]
        diagnol_2 = diagnol_2 + arr[i][n-i-1]
    print (abs(diagnol_1-diagnol_2))

arr =[]
n = int(input())
for _ in range(n):
    arr.append(list(map(int, input().rstrip().split())))
diagnolDifference(arr)

```
