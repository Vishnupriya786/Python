# Mutations

```
Read a given string, change the character at a given index and then print the modified string.
```
```
Sample Input

abracadabra
5 k

```
```
Sample Output

abrackdabra
```
```
def mutate_string(string, position, character):
    return(string[:position]+character+string[position+1:])
s = input()
i, c = input().split()
s_new = mutate_string(s, int(i), c)
print(s_new)
```
