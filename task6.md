# Task_5: Other Data Types - Lists, Tuples, and Dictionaries

## Objective:

### Lists: Ordered, Mutable Collection
A **list** is an ordered collection of items, and it is **mutable**, meaning you can change its content after creation.
Lists are defined using **square brackets `[]`**, and items are separated by **commas `,`**.

#### Example of a list:
```python
learning_topics = ["Variables", "Data Types", "Control Flow", "Functions", "Loops"]
```

### Tuples: Ordered, Immutable Collection
A **tuple** is similar to a list, but unlike lists, **tuples are immutable**, meaning you **cannot modify** the items once the tuple is created.
Tuples are defined using **parentheses `()`**.

#### Example of a tuple:
```python
project_elements = ("feedback", "progress", "status")
```

### Dictionaries: Key-Value Pairs
A **dictionary** is an unordered collection of items, where each item is stored as a pair consisting of a **key** and a **value**.
Dictionaries are defined using **curly braces `{}`**, and the key-value pairs are separated by a **colon `:`**.

#### Example of a dictionary:
```python
project_status = {"topic": "Variables", "status": "Not Started"}
```

---

## Practice:

1. A **list** of learning topics.
2. A **tuple** that holds elements of a mini-project.
3. A **dictionary** to represent the status of a mini-project element.

---

## Best Practices:

- **Lists**: Use lists when you need to store an ordered collection of items that you might need to **modify** (add/remove elements).
- **Tuples**: Use tuples when you need an ordered collection of items that should **remain constant** (e.g., coordinates, fixed data).
- **Dictionaries**: Use dictionaries for storing **key-value pairs**, especially when you need to **map** a specific piece of data (like the status of a task or project).

---

# Task_6: Operators - Arithmetic, Assignment, Comparison, Logical

## Objective:
Operators are used to perform operations on variables and values. In this task, we will:

- Understand different types of operators.
- Use arithmetic operators for calculations.
- Use comparison and logical operators to check conditions.

### 1. Arithmetic Operators
Used for mathematical operations:

#### Example:
```python
a = 10
b = 3
print(a + b)  # Addition → 13
print(a - b)  # Subtraction → 7
print(a * b)  # Multiplication → 30
print(a / b)  # Division → 3.33
print(a // b) # Floor Division → 3
print(a % b)  # Modulus (Remainder) → 1
print(a ** b) # Exponentiation → 1000
```

### 2. Assignment Operators
Used to assign values:

#### Example:
```python
x = 10
x += 5  # x = x + 5 → 15
x *= 2  # x = x * 2 → 30
print(x)
```

### 3. Comparison Operators
Used for value comparison (returns True/False):

#### Example:
```python
a, b = 10, 3
print(a > b)   # True
print(a < b)   # False
print(a == b)  # False
print(a != b)  # True
```

### 4. Logical Operators
Used for multiple conditions:

#### Example:
```python
score = 75
attendance = 85

if score > 50 and attendance > 75:
    print("Pass with good attendance")  # Output: Pass with good attendance
```

---

## Best Practices:

- Use **f-strings** for clean formatting in print statements.
- Use **comparison and logical operators** for making decisions in programs.
- Use **proper indentation** for if-else conditions to avoid errors.

