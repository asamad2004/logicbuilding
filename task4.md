# Task 4: Detailed Exploration of Strings

## Objective
Understanding string manipulation, concatenation, slicing, and formatting using f-strings or `.format()` in Python.

---

## 1. String Manipulation
Strings in Python are incredibly versatile. You can manipulate them in many ways, such as changing their case, splitting them into parts, and formatting them for output.

---

## 2. String Methods
Python provides several built-in methods that you can use on strings to manipulate and work with them:

- **`.upper()`**: Converts all characters in a string to uppercase.  
- **`.lower()`**: Converts all characters in a string to lowercase.  
- **`.split()`**: Splits a string into a list, based on a delimiter (e.g., space, comma, etc.).

---

## 3. Practice Example

```python
# User input capturing education problems
education_problems = input("Enter your thoughts on the problems with education: ")

# Convert the string to uppercase
uppercase_problems = education_problems.upper()
print(f"Uppercase Version: {uppercase_problems}")

# Convert the string to lowercase
lowercase_problems = education_problems.lower()
print(f"Lowercase Version: {lowercase_problems}")

# Split the string into words (by spaces) and display the list
splitted_problems = education_problems.split()
print(f"Split Version (Words): {splitted_problems}")

# Format the string with f-string
formatted_string = f"Education Problems: {education_problems}"
print(formatted_string)
