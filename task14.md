## **Task 14: Error Handling – try, except, finally**

### Objective:
Understand the importance of exception handling and prevent program crashes.

---

##  Explanation of Exception Handling
- **`try` Block:** Contains the code that might raise an error.
- **`except` Block:** Catches and handles specific errors, preventing crashes.
- **`finally` Block:** Always executes, whether an exception occurs or not.

---

##  Best Practices for Exception Handling

### Catch Specific Exceptions (Avoid Generic `except`)

Avoid this (Catching all errors blindly):
```python
try:
    user_input = int(input("Enter a number: "))
except:
    print("Something went wrong!")  # Not clear what went wrong
```

Use this :
```python
try:
    user_input = int(input("Enter a number: "))
except ValueError:  # Handles only conversion errors
    print("Invalid input! Please enter a valid number.")
```

---

### Always Use the `finally` Block for Cleanup

Example :
```python
try:
    file = open("data.txt", "r")
    content = file.read()
except FileNotFoundError:
    print("File not found!")
finally:
    if 'file' in locals():  # Closes file only if it was opened
        file.close()
```

---

### Handle Multiple Exceptions When Necessary

Example :
```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
except ValueError:
    print("Invalid input! Please enter a valid number.")
except ZeroDivisionError:
    print("Cannot divide by zero!")
```

---

## Summary of Best Practices

- **Catch Specific Exceptions:** Avoid generic `except`, handle expected errors like `ValueError` or `ZeroDivisionError`.

- **Use `finally` for Cleanup:** Ensure files or connections are always closed.

- **Handle Multiple Exceptions Separately:** Keep different errors in separate `except` blocks for clarity.
- **Use Custom Error Messages:** Provide 
meaningful error messages for better debugging.
- **Log Errors Instead of Printing:** Use `logging` to track errors in a file instead of just printing them.


