Write a function that takes an array of strings as an argument 
and returns a sorted array containing the same strings, ordered from shortest to longest.

For example, if this array were passed as an argument:

["Telescopes", "Glasses", "Eyes", "Monocles"]
Your function would return the following array:

["Eyes", "Glasses", "Monocles", "Telescopes"]
All of the strings in the array passed to your
function will be different lengths, so you will not have to decide
how to order multiple strings of the same length.


---
```py
def sort_by_length(arr):
    arr.sort(key=len)  # Это изменит сам список
    return arr

# Пример использования:
words = ["banana", "apple", "cherry"]
sorted_words = sort_by_length(words)
print(sorted_words)

def sort_by_length(arr):
    return sorted(arr, key=len)  # Это вернет новый отсортированный список

# Пример использования:
words = ["banana", "apple", "cherry"]
sorted_words = sort_by_length(words)
print(sorted_words)


```
