## **Task 15: File I/O – Reading and Writing Files**

###  Objective : 
Learn how to read data from and write data to files.

---

##  Explanation of File I/O
- **Reading a File (`r` mode):** Opens a file for reading.
- **Writing to a File (`w` mode):** Opens a file for writing (overwrites existing content).
- **Appending to a File (`a` mode):** Adds new content to an existing file without deleting previous data.
- **Using `with` Statement:** Ensures files are properly closed after operations.

---

## Best Practices for File Handling

###  Use `with` Statement to Handle Files Properly
**Example:**
```python
with open("progress.txt", "w") as file:
    file.write("Completed: Variables, Data Types, Loops\n")  # File is auto-closed
```

---

### Handle File Exceptions to Avoid Errors
✅ **Example:**
```python
try:
    with open("progress.txt", "r") as file:
        content = file.read()
        print(content)
except FileNotFoundError:
    print("File not found! Please check the filename.")
```

---

### Use Append Mode (`a`) for Progress Updates
✅ **Example:**
```python
with open("progress.txt", "a") as file:
    file.write("Completed: Functions, Error Handling\n")
```

---

##  Summary of Best Practices

- **Use `with open()`** – Ensures the file is automatically closed after use.
- **Handle Exceptions** – Use `try-except` to catch errors like `FileNotFoundError`.
- **Use `append` (`a`) mode** – To add new data without overwriting existing content.
- **Avoid Hardcoding Filenames** – Use variables or user input for flexibility.

---

