# Task 13: Python Modules & Importing

## Objective

Understand how to use built-in Python modules like `math` and `datetime`, and learn how to create and import custom modules.

## What is a Module?

A module in Python is a file containing Python code (functions, classes, or variables) that can be reused in other programs.

## Types of Modules:

- **Built-in Modules**: Pre-installed in Python (e.g., `math`, `datetime`).
- **User-defined Modules**: Custom modules created by users.
- **Third-party Modules**: External modules installed via pip (e.g., `numpy`, `requests`).

## Importing Built-in Modules

Python provides many built-in modules that simplify various tasks.

### Example 1: Using the `math` Module

```python
import math

num = 25
sqrt_value = math.sqrt(num)  # Square root
power = math.pow(2, 3)  # 2^3 = 8

print(f"Square Root of {num}: {sqrt_value}")
print(f"2 to the Power 3: {power}")
```
## Explanation:

- `math.sqrt(x)` – Returns the square root of `x`.
- `math.pow(a, b)` – Returns `a` raised to the power of `b`.

### Example 2: Using the `datetime` Module

```python
import datetime

current_time = datetime.datetime.now()  # Get the current date & time
formatted_time = current_time.strftime("%Y-%m-%d %H:%M:%S")  # Formatting date

print(f"Current Date & Time: {formatted_time}")
```
## Explanation:

- `datetime.datetime.now()` – Returns the current date & time.
- `.strftime()` – Formats the date & time as a string.

## Creating & Importing a Custom Module

You can create your own module and use it in different files.

### Step 1: Create a Custom Module (`my_module.py`)

```python
# my_module.py - Custom module

def greet(name):
    return f"Hello, {name}! Welcome to user-defined modules."

def add(a, b):
    return a + b
```
### Step 2: Import & Use the Module

```python
import my_module  # Importing the module

message = my_module.greet("Samad")
sum_result = my_module.add(5, 3)

print(message)  # Output: Hello, Samad! Welcome to user-defined modules.
print(f"Sum: {sum_result}")  # Output: Sum: 8
```
## Explanation:

- `import my_module` – Imports the custom module.
- `my_module.greet("Samad")` – Calls the `greet` function.
- `my_module.add(5, 3)` – Calls the `add` function.

## Importing Specific Functions from a Module

Instead of importing the whole module, you can import specific functions.

```python
from my_module import greet  # Import only 'greet' function

message = greet("Bob")  # No need to use my_module.greet()
print(message)
```
- **Benefit**: Improves readability and saves memory by not loading unnecessary functions.

## Renaming Modules Using `as`

```python
import math as m  # Renaming math module

print(m.sqrt(36))  # Output: 6.0
```
## Best Practices for Using Modules

- Use built-in modules whenever possible instead of writing redundant code.
- Use meaningful names when creating custom modules.
- Keep custom modules reusable by avoiding hard-coded values.
- Use aliasing (`as`) for long module names.
