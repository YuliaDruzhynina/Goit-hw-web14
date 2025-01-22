
The included code stub will read an integer, , from STDIN.
Without using any string methods, try to print the following:

Note that "" represents the consecutive values in between.
Example

Print the string .
Input Format
The first line contains an integer .
Constraints

Output Format
Print the list of integers from  through  as a string, without spaces.

---
```py
def main(n) :
    if 1<=n<=150:
        for i in range(1, n+1):
            print(i, end="")

if __name__ == '__main__':
    n = int(input())
    main(n) 

```
Після виклику print(), курсор автоматично переміщується на новий рядок, 
тому наступний виклик print() виведе текст уже на новому рядку. 
Але цю поведінку можна змінити за допомогою параметра end. 
Наприклад, print("Привіт", end=" ") не перейде на новий рядок після виведення.
