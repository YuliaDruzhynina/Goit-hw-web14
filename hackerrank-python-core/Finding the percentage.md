The provided code stub will read in a dictionary containing key/value pairs of name:[marks] for a list of students. 
Print the average of the marks array for the student name provided, showing 2 places after the decimal.
Example




The query_name is 'beta'. beta's average score is .
Input Format
The first line contains the integer , the number of students' records. 
The next  lines contain the names and marks obtained by a student, 
each value separated by a space. The final line contains query_name, the name of a student to query.
---
```py
if __name__ == '__main__':
    n = int(input())
    students_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        students_marks[name] = scores

    query_name = input() 
    scores = students_marks[query_name]
    average_score = sum(scores)/len(scores)   
    
    print(f"{average_score:.2f}")
```

#     Другие примеры форматирования:
# {value:.0f} — округляет до 0 знаков после запятой (выводит целое число).
# {value:.3f} — округляет до 3 знаков после запятой.
# {value:.1f} — округляет до 1 знака после запятой.
    

#  example:   
# 2
# gg 4 5 6
# kk 4 5 6
# kk
# 5.00
