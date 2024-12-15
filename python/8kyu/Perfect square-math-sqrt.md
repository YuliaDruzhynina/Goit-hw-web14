проверить является число совершенным квадратом
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


Examples

-1  =>  false
 0  =>  true
 3  =>  false
 4  =>  true
25  =>  true
26  =>  false
```
