# 🔍 Hackerrank:Python Program to Check if a String Ends with a Numeric Digit

This Python program checks whether the last character of a given input string is a **numeric digit (0–9)**.

---

## 🎯 Aim

To write a Python program that checks if a given string ends with a number using Python's built-in string methods.

---

## 🧠 Algorithm

1. **Start the program.**
2. **Input** a string from the user.
3. **Access** the last character using indexing (`string[-1]`).
4. **Check** if the last character is a digit using the `.isdigit()` method.
5. **If true**, print that the string ends with a number.
6. **Else**, print that the string does not end with a number.
7. **End the program.**

---

## 💻  Program
    import re
    s=input()
    p='[a-zA-Z0-9]*[0-9]+'
    x=re.match(p,s)
    if x:
     print("True")
    else:
     print("False")

## Output
<img width="260" height="148" alt="image" src="https://github.com/user-attachments/assets/e850ad1d-89f9-4acc-b2ae-c9326b98cef6" />

## Result
Thus, the program has been execueted successfully.
