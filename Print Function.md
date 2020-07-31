# Print Function

```
The included code stub will read an integer,n , from STDIN.

Without using any string methods, try to print the following:

123...n
Note that "..." represents the consecutive values in between.
```
```
Sample Input 

3

```
```
Sample Output 

123
```
```
n = int(input())
lis = []
for i in range(1,n+1):
    lis.append(str(i))
print ("".join(lis))
```
