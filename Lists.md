# Lists

```
Consider a list (list = []). You can perform the following commands:

insert i e: Insert integer e at position i.
print: Print the list.
remove e: Delete the first occurrence of integer e.
append e: Insert integer e at the end of the list.
sort: Sort the list.
pop: Pop the last element from the list.
reverse: Reverse the list.
Initialize your list and read in the value of n followed by n lines of commands where each command will be of the 7 types listed above. Iterate through each command in order and perform the corresponding operation on your list.
```
```
Sample Input 

12
insert 0 5
insert 1 10
insert 0 6
print
remove 6
append 9
append 1
sort
print
pop
reverse
print

```
```
Sample Output 

[6, 5, 10]
[1, 5, 9, 10]
[9, 5, 1]
```
```
n = int(input())
lis = []
for i in range(n):
    s = input().split()
    for i in range(1,len(s)):
        s[i] = int(s[i])
    if s[0] == "insert":
        lis.insert(s[1],s[2])
    elif s[0] == "append":
        lis.append(s[1])

    elif s[0] == "remove":
        lis.remove(s[1])
    elif s[0] == "sort":
        lis.sort()
    elif s[0] == "reverse":
        lis.reverse()
    elif s[0] == "pop":
        lis.pop()
    else:
        print (lis)

```
