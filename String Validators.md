# String Validators

```
You are given a string s.
Your task is to find out if the string s contains: alphanumeric characters, alphabetical characters, digits, lowercase and uppercase characters.
```
```
Sample Input

qA2

```
```
Sample Output

True
True
True
True
True
```
```
s = (input())
for item in (".isalnum()",".isalpha()",".isdigit()",".islower()",".isupper()"):
    print(any(eval("i"+item) for i in s))
```
