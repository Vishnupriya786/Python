# Time Conversion

```
Given a time in 12-hour AM/PM format, convert it to military (24-hour) time.
```
```
Sample Input 

07:05:45PM
```
```
Sample Output 

19:05:45
```
```
def timeConversion(n):
    if n[-2:] == "AM":
        if n[:2] == "12":
            print ("00" + n[2:-2])
        else:
            print (n[:-2])
    else:
        if n[:2] == "12":
            print(n[:-2])
        else:
            a = int(n[0] + n[1]) + 12
            print (str(a) + n[2:-2])
n = input()
timeConversion(n)
```
