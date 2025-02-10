## **Task 11: Functions – Parameters, Return Values, and Scope**  

### **Objective**  
Understanding how to pass parameters, return values, and the concept of variable scope (local vs global).  

---

### **Explanation**  
#### **Parameters & Return Values**  
- Functions are reusable code blocks that perform a specific task.  
- **Parameters:** Used to provide input to a function.  
- **Return Value:** Used to return the result of a function.  

#### **Example of Function with Parameters and Return Value**  
```python
# Function with parameters and return value
def add_numbers(a, b):  
    return a + b  

result = add_numbers(5, 3)  
print(result)  # Output: 8
```

---

### **Local vs Global Scope**  
- **Local Variable:** Accessible only inside the function.  
- **Global Variable:** Accessible throughout the program.  

#### **Example:**  
```python
# Global variable
global_var = 10  

def example_function():
    local_var = 5  # Local variable
    return global_var + local_var  

print(example_function())  # Output: 15
```

---

### **Step-by-Step Learning Experience**  
- Functions provide **reusability** and **modularity**.  
- Used **parameters** and **return values** to modify the checklist.  
- Understood **global vs local scope** by using variables.  

---

## **Best Practices for Functions – Parameters, Return Values, and Scope**  
To write **clean, efficient, and maintainable** functions in Python, follow these best practices:

### **1️⃣ Use Descriptive Function Names**  
A function name should describe **what it does**. Use meaningful names so that the code is self-explanatory.  

✅ **Use this:**  
```python
# Descriptive function name
def calculate_total_price(price, quantity):
    return price * quantity
```

❌ **Instead of this:**  
```python
# Poor function name
def ct(p, q):
    return p * q
```

The first function **clearly states** its purpose, whereas the second function is **unclear**.  

---

### **2️⃣ Keep Functions Short & Focused (Single Responsibility Principle)**  
Each function should **do only one thing** and do it well.  

✅ **Use this:**  
```python
# Function that only calculates discounted price
def get_discounted_price(price, discount_rate):
    return price - (price * discount_rate / 100)
```

❌ **Instead of this:**  
```python
# Function doing multiple things
def process_order(price, discount_rate, stock, user_id):
    price = price - (price * discount_rate / 100)
    stock -= 1
    print(f"Order placed for user {user_id}. New stock: {stock}")
    return price
```

The **first function** is focused, while the **second function** is handling multiple tasks, making it harder to maintain.  

---

### **3️⃣ Use Parameters Instead of Global Variables**  
Global variables should be **avoided inside functions** unless necessary, as they make debugging difficult.  

✅ **Use this:**  
```python
# Function using parameters
def add_item(checklist, item):
    checklist.append(item)
    return checklist
```

❌ **Instead of this:**  
```python
# Function modifying a global variable
checklist = []

def add_item(item):
    checklist.append(item)
```

The **first function** is **reusable** because it takes `checklist` as a parameter. The **second function** modifies a global variable, making it harder to track changes.  

---

### **4️⃣ Always Return Values Instead of Printing Inside Functions**  
A function should **return** the result instead of printing it directly.  

✅ **Use this:**  
```python
# Function returning a value
def get_message(name):
    return f"Hello, {name}!"

message = get_message("John")
print(message)  # Output: Hello, John!
```

❌ **Instead of this:**  
```python
# Function printing directly
def get_message(name):
    print(f"Hello, {name}!")

get_message("John")  # Output: Hello, John!
```

The **first function** gives flexibility by returning a value. The **second function** forces printing, which limits reusability.  

---
