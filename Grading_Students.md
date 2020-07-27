# Grading Students

```
HackerLand University has the following grading policy:

Every student receives a grade in the inclusive range from 0 to 100.
Any grade less than 40 is a failing grade.
Sam is a professor at the university and likes to round each student's grade according to these rules:

If the difference between the grade and the next multiple of 5 is less than 3, round grade up to the next multiple of 5.
If the value of grade is less than 38, no rounding occurs as the result will still be a failing grade.
```
```
Sample Input 

4
73
67
38
33
```
```
Sample Output 

75
67
40
33
```
```
def gradingStudents(grade):
    for marks in grade:
        if marks<38:
            result = marks
        else:
            reminder = marks%5
            round = marks - reminder
            if reminder>0:
                round +=5

            difference = round - marks
            if difference<3:
                result = round
            else:
                result = marks
        print(result)

n = int(input())
grade = []
for i in range(n):
    grade.append(int( input()))

gradingStudents(grade)
```
