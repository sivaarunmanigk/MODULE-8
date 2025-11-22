# 🎓 Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.

---

## 🎯 Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

## 🧠 Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.

---

## 💻  Program

    N=int(input())
    records=[]
    for _ in range(N):
        name=input()
        grade=float(input())
        records.append([name,grade])
    grades=sorted(set([grade for name,grade in records]))
    second_lowest_grade=grades[1]
    students_with_second_lowest=[name for name,grade in records if grade==second_lowest_grade]
    students_with_second_lowest.sort()
    for student in students_with_second_lowest:
        print(student)

## Output
<img width="332" height="341" alt="image" src="https://github.com/user-attachments/assets/2cca47df-166e-4338-920f-dd56d3767c0e" />

## Result
Thus, the program has been execueted successfully.

