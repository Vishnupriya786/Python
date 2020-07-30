# Between Two Sets

```
You will be given two arrays of integers and asked to determine all integers that satisfy the following two conditions:

The elements of the first array are all factors of the integer being considered
The integer being considered is a factor of all elements of the second array
These numbers are referred to as being between the two arrays. You must determine how many such numbers exist.
```
```
Sample Input

2 3
2 4
16 32 96
```
```
Sample Output

3
```
```
def getTotalX(a,b):
    lis_a = []
    lis_b =[]
    for item_a in a:
        for i in range(1, 101):
            if i%item_a == 0:
                lis_a.append(i)

    for item_b in b:
        for i in range(1, 101):
            if item_b % i == 0:
                lis_b.append(i)
    temp = lis_a+lis_b
    length = len(a+b)
    result = []
    for item in temp:
        if temp.count(item) == length:
            result.append(item)
    print (len(set(result)))

num = input().split()
a = list(map(int, input().split()))
b = list(map(int, input().split()))
getTotalX(a,b)

```
