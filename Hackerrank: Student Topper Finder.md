# # 🔢 Hackerrank:# 🏆 Student Topper Finder

---
This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---
## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.
---
##💻 PROGRAM:
~~~
students = {
    "Alice": [85, 90, 78, 92, 88],
    "Bob": [75, 80, 70, 85, 78],
    "Charlie": [90, 95, 88, 92, 91],
    "David": [60, 65, 70, 55, 62]
}

total_marks = {}

for student, marks in students.items():
    total_marks[student] = sum(marks)

print("Total Marks for each student:")
for student, total in total_marks.items():
    print(f"{student}: {total}")

topper = max(total_marks, key=total_marks.get)
topper_marks = total_marks[topper]

print(f"\nThe student with the highest total marks is {topper} with {topper_marks} marks.")
~~~
## OUTPUT
~~~
Input                                         Result
Alice [85, 90, 78, 92, 88]              
Bob [75, 80, 70, 85, 78]                   The student with the highest total marks is Charlie with 456 marks.
Charlie [90, 95, 88, 92, 91]
David [60, 65, 70, 55, 62]
~~~
---
## RESULT
The program was successful
