# Task_3

## Variables & Basic Data Types (Numbers & Strings)

**Objective:** Understanding what variables are and how integer, float, and string data types work in Python.

## 1. What are Variables?
A variable in Python is like a container that holds data. You can assign a value to a variable, and the variable will store that value. The value can be anything: a number, a string, or more complex data.

**Syntax:**
```python
variable_name = value
x = 10
```

## 2. Data Types in Python
Python has several data types, but we will focus on three basic types: Integer, Float, and String.

### a) Integer (int)
An integer is a whole number without a decimal point.

**Example:**
```python
age = 25  # integer
```

### b) Float (float)
A float is a number that has a decimal point.

**Example:**
```python
height = 5.9  # float
```

### c) String (str)
A string is a sequence of characters, enclosed in single or double quotes.

**Example:**
```python
name = "John Doe"  # string
greeting = 'Hello!'  # string
```

## 3. Best Practices

- **Descriptive Names:** Use meaningful names for variables. For example, instead of `x` or `a`, use `age`, `height`, or `student_name` so that the variable’s purpose is clear.
- **Consistency:** Stick to one naming convention throughout the program. Typically, variables are written in lowercase letters and separated by underscores (snake_case), like `student_age` or `course_name`.
- **Avoid Overwriting Built-in Names:** Don’t name your variables after built-in Python functions or keywords like `list`, `print`, `input`, etc.

## Example Code:
```python
# Integer Variable
age = 21

# Float Variable
height = 5.8

# String Variable
name = "Alice"

# Printing variables
print(f"{name} is {age} years old and {height} feet tall.")
```
