# Task_9

## While Loop in Python

### Objective:
A while loop runs as long as a specified condition remains True.

### Syntax:
```python
while condition:
    # Code that runs in loop
```
### Example:
```python
# Initialize a variable
number = 1

# Loop while number is less than or equal to 5
while number <= 5:
    print(number)  # Print the current number
    number += 1    # Increase the number by 1
```
### Explanation:
- We initialize number = 1.
- The while loop runs as long as number <= 5.
- Inside the loop:
print(number) displays the current value.
number += 1 increases the value by 1 in each iteration.
- When number becomes 6, the condition number <= 5 fails, and the loop stops.
  
## Best Practices:

- Ensure loops have an exit condition to prevent infinite loops.
- Use `.lower()` to make input case-insensitive.
- Use `break` to stop the loop when needed.
