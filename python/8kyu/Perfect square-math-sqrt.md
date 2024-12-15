проверить является число совершенным квадратом

 In Python, n**0.5 is the same as sqrt(n) вычисляем корень квадратный из n
---
```py
import math

def is_square(n): 
    if n<0:
        return False
    if int(math.sqrt(n))**2!=n:
        return False 
    else:
        return True


def is_square(n):    
    if n < 0:
        return False
    sqrt = math.sqrt(n)
    return sqrt.is_integer()


def is_square(n):    
    return n >= 0 and (n**0.5) % 1 == 0
    return n > -1 and math.sqrt(n) % 1 == 0

n**0.5 и sqrt(n) — это извлечение квадратного корня из числа n.
Если результат квадратного корня является целым числом (например, корень из 16 равен 4), то его дробная часть будет равна 0.
Если результат не является целым числом (например, корень из 14 равен 3.74166...), то дробная часть будет ненулевой.
Таким образом, n**0.5 % 1 == 0 проверяет, является ли квадратный корень числа целым числом, а значит, и само число n является совершенным квадратом.


Examples

-1  =>  false
 0  =>  true
 3  =>  false
 4  =>  true
25  =>  true
26  =>  false
```
