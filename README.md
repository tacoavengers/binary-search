# binary-search
Binary search

https://repl.it/@webdevdave/Binary-Search#main.py

- The data must be sorted
- 0(log n)

```
def binary_search(list, item):
    low = 0
    high = len(list) -1
    
    while low <= high:
        mid = (low + high) // 2
        guess = list[mid]
        if guess == item:
            return mid
        if guess > item:
            high = mid - 1
        else:
            low = mid + 1
    return None
        
    
list = [1,2,3,4,6,7,8,9,10,14]  
print(binary_search(list, 9))
```
