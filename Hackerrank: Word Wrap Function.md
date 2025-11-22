# 🔄 Hackerrank : # 📦 Python Word Wrap Function

This Python program defines a function that **wraps a long string into multiple lines**, ensuring each line does not exceed a specified width.

---

## 🎯 Aim

To write a Python function that takes a long string and a specified width, and returns the string formatted with line breaks such that each line has **at most the given width**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Define a function `wrap(string, max_width)`:
   - Create an empty list `wrapped_lines` to store parts of the string.
   - Loop through the string using steps of `max_width`.
   - In each iteration, extract a substring of length `max_width`.
   - Append this substring to the list.
3. Join the list with `\n` to create the final string.
4. Return the result.
5. **End** the program.

---


## 🧪 Program
               def format_string(input_string, width):
      
          words = input_string.split()
          
          # Initialize an empty list to store the formatted lines
          lines = []
          current_line = ""
          for word in words:
              # If adding the next word exceeds the width, start a new line
              if len(current_line) + len(word) + 1 > width:
                  lines.append(current_line)
                  current_line = word
              else:
        
                  if current_line:
                      current_line += " " + word
                  else:
                      current_line = word
          if current_line:
              lines.append(current_line)
         
          return "\n".join(lines)
      
      input_string = "This is an example of a long string that will be formatted into multiple lines based on the specified width."
      width = 20
      formatted_string = format_string(input_string, width)
      print(formatted_string)
## Sample Output
      This is an example
      of a long string
      that will be
      formatted into
      multiple lines based
      on the specified
      width.
## Result
The program was successful.
