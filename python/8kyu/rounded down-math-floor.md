The cockroach is one of the fastest insects. 
Write a function which takes its speed in km per hour 
and returns it in cm per second, rounded down to the integer (= floored).

For example:

1.08 --> 30
---
```py
import math
def cockroach_speed(s):
    # Good Luck!
    new_speed = s*100000/3600
    return math.floor(new_speed)
```
