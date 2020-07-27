# Apple and Orange

```
Sam's house has an apple tree and an orange tree that yield an abundance of fruit. In the diagram below, the red region denotes his house, where s is the start point, and t is the endpoint. The apple tree is to the left of his house, and the orange tree is to its right. You can assume the trees are located on a single point, where the apple tree is at point a, and the orange tree is at point b.
When a fruit falls from its tree, it lands d units of distance from its tree of origin along the x-axis. A negative value of d means the fruit fell d units to the tree's left, and a positive value of d means it falls d units to the tree's right.

Given the value of d for m apples and n oranges, determine how many apples and oranges will fall on Sam's house (i.e., in the inclusive range )[s,t]?
```
```
Sample Input 

7 11 (s t)
5 15 (a b)
3 2 (m n)
-2 2 1 (apples)
5 -6 (oranges)
```
```
Sample Output 

1
1
```
```
def countApplesAndOranges(distance_apple, distance_orange):
    apple_list = []
    orange_list = []
    count_apple = 0
    count_orange = 0

    for item in distance_apple:
        apple = item + a
        apple_list.append(apple)
    for item in distance_orange:
        orange = item + b
        orange_list.append(orange)
    for item in apple_list:
        if s<=item<=t:
            count_apple += 1
    for item in orange_list:
        if s<=item<=t:
            count_orange += 1
    
    print (count_apple)
    print (count_orange)

#sam house
st = input().split()
s = int(st[0])
t = int(st[1])
#tree location
ab = input().split()
a = int(ab[0])
b = int(ab[1])
#count of apple and orange
mn = input().split()
m = int(mn[0])
n = int(mn[1])
distance_apple = list(map(int, input().rstrip().split()))
distance_orange = list(map(int, input().rstrip().split()))

countApplesAndOranges(distance_apple,distance_orange)

```
