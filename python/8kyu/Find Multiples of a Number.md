In this simple exercise, you will build a program that takes a value, integer , 
and returns a list of its multiples up to another value, limit . 
If limit is a multiple of integer, it should be included as well. 
There will only ever be positive integers passed into the function, not consisting of 0. 
The limit will always be higher than the base.

For example, if the parameters passed are (2, 6), 
the function should return [2, 4, 6] as 2, 4, and 6 are the multiples of 2 up to 6.


```py
def find_multiples(integer, limit):
    return list(range(integer, limit + 1, integer))

print(find_multiples(3, 10))  # Выведет: [3, 6, 9]
print(find_multiples(5, 20))  # Выведет: [5, 10, 15, 20]
print(find_multiples(7, 50))  # Выведет: [7, 14, 21, 28, 35, 42, 49]

def find_multiples(integer, limit):
    arr = []
    count = integer
    while count <= limit:
        arr.append(count)
        count += integer
    return arr
```
