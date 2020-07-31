# Text Wrap

```
You are given a string S and width w .
Your task is to wrap the string into a paragraph of width w.
```
```
Sample Input 

ABCDEFGHIJKLIMNOQRSTUVWXYZ
4

```
```
Sample Output 

ABCD
EFGH
IJKL
IMNO
QRST
UVWX
YZ
```
```
import textwrap
def wrap(string, max_width):
     return textwrap.fill(string,max_width)
string = input()
max_width = int(input())
result = wrap(string, max_width)
print(result)
```
