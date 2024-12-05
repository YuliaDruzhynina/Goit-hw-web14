Consider an array/list of sheep where some sheep
may be missing from their place. We need a function that 
counts the number of sheep present in the array (true means present).
---
```py
#For example,

#[True,  True,  True,  False,
  #True,  True,  True,  True ,
  #True,  False, True,  False,
  #True,  False, False, True ,
  #True,  True,  True,  True ,
  #False, False, True,  True]
#The correct answer would be 17.
#В списке sheep находятся булевые значения True и False!!!
#Hint: Don't forget to check for bad values like null/undefined

def count_sheeps(sheep):
# Проверка на None, если список пустой или неопределённый
    if sheep is None:
        return 0  # Возвращаем 0, если список не задан
  number = sheep.count(True)
    return number

print(count_sheeps(None))
print(count_sheeps([True, True, False, True, False]))  # Выведет: 3

```
