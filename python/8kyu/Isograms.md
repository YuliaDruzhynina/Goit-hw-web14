An isogram is a word that has no repeating letters,
consecutive or non-consecutive. Implement a function 
that determines whether a string that contains only letters 
is an isogram. Assume the empty string is an isogram. 
Ignore letter case.

Example: (Input --> Output)

```py
def is_isogram(string):
    return len(string) == len(set(string.lower()))


# Создание множества
my_set = {1, 2, 3, 4, 5}
print(my_set)  # Выведет: {1, 2, 3, 4, 5}

# Добавление элемента
my_set.add(6)
print(my_set)  # Выведет: {1, 2, 3, 4, 5, 6}

# Попытка добавить дубликат не изменяет множество
my_set.add(3)
print(my_set)  # Выведет: {1, 2, 3, 4, 5, 6} (3 не добавится, так как он уже есть)

# Преобразование списка в множество (удаляются дубликаты)
my_list = [1, 2, 3, 2, 1]
my_set_from_list = set(my_list)
print(my_set_from_list)  # Выведет: {1, 2, 3}
```
