In a small town the population is p0 = 1000 at the beginning of a year.
The population regularly increases by 2 percent per year and moreover 50 
new inhabitants per year come to live in the town. How many
years does the town need to see its population greater than or 
equal to p = 1200 inhabitants?


Note:
Don't forget to convert the percent parameter as a percentage 
in the body of your function: if the parameter percent is 
2 you have to convert it to 0.02.

There are no fractions of people. At the end of each year,
the population count is an integer: 252.8 people round down to 252 persons.

Examples:
nb_year(1500, 5, 100, 5000) -> 15
nb_year(1500000, 2.5, 10000, 2000000) -> 10


Оператор присваивания не является выражением: 
В Python оператор += изменяет значение переменной, 
но сам по себе не является выражением,
которое можно вернуть. Он просто выполняет действие, 
не возвращая значения.
---
```py


def nb_year(p0, percent, aug, p):
    years=0
    while p0<p:
        p0 = int(p0 + p0*percent/100 + aug)
        years +=1
    return years 

```
