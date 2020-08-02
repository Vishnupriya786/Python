# Finding the percentage

```
The provided code stub will read in a dictionary containing key/value pairs of name:[marks] for a list of students. Print the average of the marks array for the student name provided, showing 2 places after the decimal.
```
```
Sample Input 

3
Krishna 67 68 69
Arjun 70 98 63
Malika 52 56 60
Malika

```
```
Sample Output 

56.00
```
```
n = int(input())
dic = {}
for i in range(n):
    name ,*line = input().split()
    score = list(map(float, line))
    dic[name] = score
stu_name = input()

a = dic[stu_name]
print ('%.2f'%(sum(a)/len(a)))
```
