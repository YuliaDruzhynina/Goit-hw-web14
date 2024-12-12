Complete the square sum function so that it squares each number passed 
into it and then sums the results together.

For example, for [1, 2, 2] it should return 9 

---
```py
def square_sum(numbers):
    sum = 0
    for number in numbers:
        sum +=number*number
    return sum

def square_sum(numbers):
    return sum(number**2 for number in numbers)
```
