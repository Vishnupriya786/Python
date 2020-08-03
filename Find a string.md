# Find a string

```
In this challenge, the user enters a string and a substring. You have to print the number of times that the substring occurs in the given string. String traversal will take place from left to right, not from right to left.
```
```
Sample Input

ABCDCDC
CDC

```
```
Sample Output

2
```
```
def count_substring(string,sub_string):
    count = 0
    for i in range(0,(len(string) - len(sub_string)+1)):
        if (string[i:len(sub_string)+i]) == sub_string:
            count +=1
    return(count)
string = input().strip()
sub_string = input().strip()
count = count_substring(string, sub_string)
print(count)
```
