# Nested Lists

```
Given the names and grades for each student in a class of N students, store them in a nested list and print the name(s) of any student(s) having the second lowest grade.

Note: If there are multiple students with the second lowest grade, order their names alphabetically and print each name on a new line.
```
```
Sample Input 

5
Harry
37.21
Berry
37.21
Tina
37.2
Akriti
41
Harsh
39
```
```
Sample Output 

Berry
Harry
```
```
lis = []
lowest_mark = []
second_lowmark =[]
res= []
for i in range(int(input())):
    lis.append([input(), float(input())])

lis.sort(key = lambda x:x[1])

for item in lis:
    if item[1] == lis[0][1]:
        lowest_mark.append(item)
    else:
        second_lowmark.append(item)

for item in second_lowmark:
    if item[1] == second_lowmark[0][1]:
        res.append(item)
res.sort(key = lambda x:x[0])
for item in res:
    print (item[0])

```
