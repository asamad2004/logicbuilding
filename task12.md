# Task 12: Lambda Functions & Higher-Order Functions

## Objective
Understand anonymous functions (lambda), their usage, and practical implementation.

---

##  What is a Lambda Function?
A **lambda function** in Python is an **anonymous (nameless) function** that can have multiple arguments but only one expression. It is used when we need a short function for immediate use.

### **Syntax:**
```python
lambda arguments: expression
```
**Key Points:**  
- Lambda functions **don’t require** a `def` keyword.
- They return the result **automatically** (no need for `return`).
- One-liner function for **simple tasks**.

---

##  Example of a Lambda Function
### **Add Two Numbers**
```python
# Normal function
def add(x, y):
    return x + y

# Lambda function equivalent
add_lambda = lambda x, y: x + y

print(add(3, 5))       # Output: 8
print(add_lambda(3, 5))  # Output: 8
```
 The lambda function is **shorter and more concise**.

---

## Object & Properties of Lambda Function
A lambda function is still an **object** in Python, just like a normal function.

### **Example:**
```python
# Lambda function stored in a variable
multiply = lambda x, y: x * y

# Checking type
print(type(multiply))  # Output: <class 'function'>

# Calling function
print(multiply(5, 3))  # Output: 15
```
 Lambda functions are **function objects**, meaning they can be:
- Stored in variables
- Passed as arguments
- Returned from other functions

---

## Lambda Functions with Higher-Order Functions – Single Example
In this example, we explore **lambda functions** and their integration with **higher-order functions** such as `map()`, `filter()`, `reduce()`, `sorted()`, dictionaries, nested functions, and list comprehensions.

```python
from functools import reduce

numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# 1️⃣ Using map() to square each number
squared_numbers = list(map(lambda x: x**2, numbers))

# 2️⃣ Using filter() to select even numbers
even_numbers = list(filter(lambda x: x % 2 == 0, numbers))

# 3️⃣ Using reduce() to sum all numbers
sum_of_numbers = reduce(lambda x, y: x + y, numbers)

# 4️⃣ Sorting a list of tuples (name, age) by age using sorted()
people = [("Alice", 25), ("Bob", 20), ("Charlie", 30)]
sorted_people = sorted(people, key=lambda person: person[1])

# 5️⃣ Using lambda in a dictionary to perform different operations
operations = {
    "add": lambda x, y: x + y,
    "subtract": lambda x, y: x - y,
    "multiply": lambda x, y: x * y
}
result = operations["multiply"](5, 3)

# 6️⃣ Using lambda inside a function (Nested Lambda)
def make_multiplier(n):
    return lambda x: x * n

double = make_multiplier(2)
triple = make_multiplier(3)

# 7️⃣ Using lambda inside list comprehension
squared_list_comp = [(lambda x: x**2)(num) for num in numbers]

# 🔹 Printing results
print("Squared Numbers:", squared_numbers)
print("Even Numbers:", even_numbers)
print("Sum of Numbers:", sum_of_numbers)
print("Sorted by Age:", sorted_people)
print("Multiplication Result:", result)
print("Double of 5:", double(5))
print("Triple of 5:", triple(5))
print("Squared List Comprehension:", squared_list_comp)
```

###  Expected Output:
```
Squared Numbers: [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
Even Numbers: [2, 4, 6, 8, 10]
Sum of Numbers: 55
Sorted by Age: [('Bob', 20), ('Alice', 25), ('Charlie', 30)]
Multiplication Result: 15
Double of 5: 10
Triple of 5: 15
Squared List Comprehension: [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
```

---

##  Lambda vs Regular Function – When to Use?
| Feature           | Lambda Function           | Regular Function (`def`) |
|------------------|-------------------------|--------------------------|
| **Syntax**       | Short (one-liner)        | Longer (multi-line)      |
| **Readability**  | Good for simple cases    | Better for complex cases |
| **Reusability**  | Mostly one-time use      | Can be used repeatedly   |
| **Performance**  | Slightly faster (inline) | Similar                  |

 **When to use?**
- **Lambda functions** → When you need a **simple, one-liner function** for quick operations.
- **`def` functions** → When the function is **complex and needs documentation**.

---

##  Best Practices for Using Lambda Functions
- **Use lambda for short, simple tasks.**  
- **Prefer named functions (`def`) for complex operations.**  
- **Combine lambda with `map()`, `filter()`, and `reduce()`.**  
- **Use lambda for sorting and dictionary-based operations.**  
- **Avoid lambda when it reduces readability.**

---
