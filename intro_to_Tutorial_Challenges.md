# Intro to Tutorial Challenges

```
Given a sorted array (arr) and a number (V), can you print the index location of V in the array?
```
```
Sample Input 

4
6
1 4 5 7 9 12
```
```
Sample Output 

1
```
```
def introTutorial(arr,V):
    for item in arr:
        if item == V:
            print (arr.index(item))

V = int(input())
n = int(input())
arr = list(map(int,input().rstrip().split()))
introTutorial(arr,V)

```
