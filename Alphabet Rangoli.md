# Alphabet Rangoli
```
You are given an integer, N. Your task is to print an alphabet rangoli of size N.
```
```
Sample Input

5

```
```
Sample Output

--------e--------
------e-d-e------
----e-d-c-d-e----
--e-d-c-b-c-d-e--
e-d-c-b-a-b-c-d-e
--e-d-c-b-c-d-e--
----e-d-c-d-e----
------e-d-e------
--------e--------
```
```
def print_rangoli(n):
    alphabets = list(map(chr,range(97,123)))
    length =len("-".join(alphabets[n-1::-1]+ alphabets[1:n]))
    for i in range(1,n):
        print("-".join(alphabets[n-1:n-i:-1]+ alphabets[n-i:n]).center(length,"-"))
    for i in range(n,0,-1):
        print("-".join(alphabets[n-1:n-i:-1]+ alphabets[n-i:n]).center(length,"-"))
n = int(input())
print_rangoli(n)
```
