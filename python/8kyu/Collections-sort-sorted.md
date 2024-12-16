Write a function that takes an array of strings as an argument 
and returns a sorted array containing the same strings, ordered from shortest to longest.

For example, if this array were passed as an argument:

["Telescopes", "Glasses", "Eyes", "Monocles"]
Your function would return the following array:

["Eyes", "Glasses", "Monocles", "Telescopes"]
All of the strings in the array passed to your
function will be different lengths, so you will not have to decide
how to order multiple strings of the same length.

Метод sort():
Метод sort() используется для сортировки существующего списка и изменяет его на месте.
Метод sort() не возвращает никакого значения. Он работает с объектом, к которому применяется,
то есть с самим списком. Если вы попытаетесь вызвать sort() как return sort(key=len), 
это вызовет ошибку, потому что sort() не возвращает никакого значения.
Функция sorted():
Функция sorted() является функцией, которая принимает список (или другой итерируемый объект)
и возвращает новый отсортированный список.
В отличие от метода sort(), sorted() не изменяет исходный список, а возвращает новый отсортированный список.



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
