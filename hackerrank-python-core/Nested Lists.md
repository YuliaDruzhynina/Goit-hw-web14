Given the names and grades for each student in a class of  students, 
store them in a nested list and print the name(s) of any student(s) 
having the second lowest grade.
Note: If there are multiple students with the second lowest grade, 
order their names alphabetically and print each name on a new line.
Example


There are two students with that score: . Ordered alphabetically, the names are printed as:
There are 5 students in this class whose names and grades are assembled to build the following list:
python students = [['Harry', 37.21], ['Berry', 37.21], ['Tina', 37.2], ['Akriti', 41], ['Harsh', 39]]
The lowest grade of 37,2 belongs to Tina. The second lowest grade of 37,2 belongs to both Harry and Berry, 
so we order their names alphabetically and print each name on a new line.
----
```py
if __name__ == '__main__':
    lst = []
    for _ in range(int(input())):
        name = input()
        score = float(input())
        lst.append((name, score))

    grades = sorted(set(score for name, score in lst))
    second_lowest_grade = grades[1] 

    second_lowest_students = [name for name, score in lst if score == second_lowest_grade]

    second_lowest_students.sort()

    for student in second_lowest_students:
        print(student)
```
