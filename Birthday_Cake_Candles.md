# Birthday Cake Candles

```
You are in charge of the cake for your niece's birthday and have decided the cake will have one candle for each year of her total age. When she blows out the candles, she’ll only be able to blow out the tallest ones. Your task is to find out how many candles she can successfully blow out.
```
```
Sample Input 

4
3 2 1 3
```
```
Sample Output 

2
```
```
def birthdayCakeCandles(arr):
    max_candle = max(arr)
    print (arr.count(max_candle))
n = int(input())
arr = list(map(int,input().rstrip().split()))
birthdayCakeCandles(arr)
```
