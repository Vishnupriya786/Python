# Big Sorting

```
Consider an array of numeric strings where each string is a positive number with anywhere from 1 to 10^6 digits. Sort the array's elements in non-decreasing, or ascending order of their integer values and print each element of the sorted array on a new line.

Function Description

Complete the bigSorting function in the editor below. It should return the sorted string array.

bigSorting has the following parameter(s):

unsorted: an unsorted array of integers as strings
```
```
Sample Input 

6
31415926535897932384626433832795
1
3
10
3
5
```
```
Sample Output 

1
3
3
5
10
31415926535897932384626433832795
```
```
def bigSorting(unsorted):
    unsorted.sort(key = lambda x: (len(x),x))
    return unsorted
n = int(input())
unsorted = []
for _ in range(n):
    unsorted_item = input()
    unsorted.append(unsorted_item)

result = bigSorting(unsorted)
    
```
