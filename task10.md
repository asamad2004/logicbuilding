# Task 10: Functions – Definition and Basic Syntax

## 🎯 Objective  
Functions are a key concept in programming that help you avoid repetition and organize code efficiently.  

### **What will you learn?**  
- What functions are?  
- How to define and use functions in Python?  
- Why functions are useful (DRY Principle - "Don’t Repeat Yourself")?  

---

##  What is a Function?  
A function is a **reusable block of code** that performs a specific task.  
Instead of writing the same code multiple times, you can **write a function once and call it whenever needed**.  

### **Example:**  
```python
def function_name():
    # Function body
    print("This is a function")
```
##  Key Points  

- `def` (keyword) is used to define a function.  
- `function_name` (custom name) is the name of the function.  
- `()` (parentheses) are used, sometimes with parameters.  
- **Indentation** is used to write the function body.  

---

## 📌 Example of a Function  
```python
def greet():
    print("Hello! Welcome to the Checklist Reminder.")

# Function Call
greet()
```
🔹 **Note:** The function `greet()` is **defined once** but can be **called multiple times**.  

---

##  Why Use Functions? (DRY Principle)  

 **Avoids Code Duplication** – Instead of writing the same code again and again, use functions.  

 **Improves Readability** – Makes the program easier to understand.  

 **Easier Debugging** – If an error occurs, fix it in one place.  

 **Reusability** – Functions can be used multiple times.  

# Best Practices for Using Functions in Python

## 1. Use Descriptive Names

Use this:-  
```python
def print_greeting():  # (Good)
```
 Instead of this:-
```python
def p(): (Bad)
```
## 2. Keep Functions Short & Focused

A function should do one task only.

## 3. Use Parameters Instead of Global Variables

Use this:-  
```python
def add_item(items_list, item): # (Good)
```
Instead of this:-
```python
Modifying global variables inside functions (Bad)
 ```
