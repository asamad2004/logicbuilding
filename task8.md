# Task_8

## For Loop in Python

### Objective:
A for loop is used to iterate over a sequence (list, tuple, string, dictionary, etc.).

### Syntax:
```python
for variable in sequence:
    for topic in learning_topics:
        # Code to execute in loop
```
### Example:
```python
# Using a for loop to print numbers from 1 to 5
for number in range(1, 6):  
    print(number)
```
## Explanation:
- range(1, 6) generates numbers from 1 to 5 (the last number 6 is not included).
- for number in range(1, 6): loops through each number in the range.
- print(number) prints each number on a new line.

## Best Practices:

- Use `enumerate()` if you need index values.
- Use `.items()` for iterating key-value pairs in dictionaries.
- Avoid modifying lists while looping to prevent errors.
