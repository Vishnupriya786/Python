# Staircase

```
Consider a staircase of size n = 4 :

   #
  ##
 ###
####
Observe that its base and height are both equal to n, and the image is drawn using # symbols and spaces. The last line is not preceded by any spaces.

Write a program that prints a staircase of size n .
```
```
Sample Input

6 
```
```
Sample Output

     #
    ##
   ###
  ####
 #####
######
```
```
def staircase(n):
    for i in range(1,n+1):
        print(" "*(n-i)+"#"*i)
n = int(input())
staircase(n)

```
