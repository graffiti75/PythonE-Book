# Python Development E-Book for Students

## Table of Contents
1. [Introduction to Python](#introduction-to-python)
2. [Basic Syntax](#basic-syntax)
3. [Control Structures](#control-structures)
4. [Functions](#functions)
5. [Data Structures](#data-structures)
6. [Modules and Packages](#modules-and-packages)
7. [File Handling](#file-handling)
8. [Object-Oriented Programming](#object-oriented-programming)
9. [Exception Handling](#exception-handling)
10. [Advanced Topics](#advanced-topics)
11. [Standard Libraries](#standard-libraries)
12. [Web Development](#web-development)
13. [Data Science](#data-science)
14. [Projects](#projects)
15. [Best Practices](#best-practices)
16. [Conclusion](#conclusion)

## 1. Introduction to Python

### What is Python?
Python is an easy-to-learn, powerful programming language with efficient high-level data structures and a simple approach to object-oriented programming. Its elegant syntax, dynamic typing, and interpreted nature make it ideal for scripting and rapid application development. Created by Guido van Rossum in the late 1980s and released in 1991, Python is widely used across various domains.

### Why Learn Python?
- **Versatility**: Applied in web development, data science, automation, and scientific computing.
- **Community Support**: Backed by a large community with extensive libraries and frameworks.
- **Career Opportunities**: Highly sought-after in industries like AI, machine learning, and data analysis.

### Setting Up the Environment
- **Install Python**: Download from [python.org](https://www.python.org/downloads/) or use package managers like `apt` (Linux) or `Homebrew` (macOS).
- **Choose an IDE/Editor**: Options include Visual Studio Code, PyCharm, or simple editors like Notepad++.
- **Python Interpreter**: Run Python interactively or as scripts using `python filename.py`.

### Hello, World!
```python
print("Hello, World!")
```
Save as `hello.py` and run with `python hello.py`.

### Exercises
1. Install Python and run the "Hello, World!" program.
2. Explore the Python interpreter by performing basic arithmetic operations.

## 2. Basic Syntax

### Variables
Variables store data without explicit type declaration.
```python
x = 5  # Integer
y = "Hello"  # String
```

### Data Types
| Type         | Description                     | Example                     |
|--------------|---------------------------------|-----------------------------|
| Integer      | Whole numbers                  | `x = 5`                    |
| Float        | Decimal numbers                | `y = 5.0`                  |
| String       | Sequence of characters         | `s = "Hello"`              |
| List         | Ordered, mutable collection    | `lst = [1, 2, 3]`         |
| Tuple        | Ordered, immutable collection  | `tup = (1, 2, 3)`         |
| Dictionary   | Key-value pairs                | `dict = {"name": "Alice"}` |
| Set          | Unordered, unique collection   | `set = {1, 2, 3}`         |

### Operators
- **Arithmetic**: `+`, `-`, `*`, `/`, `%`, `**`, `//`
- **Comparison**: `==`, `!=`, `>`, `<`, `>=`, `<=`
- **Logical**: `and`, `or`, `not`

### Input/Output
- **Input**: `input("Enter your name: ")`
- **Output**: `print("Hello, World!")`

### Comments
- Single-line: `# This is a comment`
- Multi-line: `"""This is a multi-line comment"""`

### Indentation
Python uses indentation to define code blocks.
```python
if True:
    print("This is indented")
```

### Exercises
1. Create variables for your name and age, then print them.
2. Convert a string "123" to an integer and add 10.

## 3. Control Structures

### If-Else Statements
```python
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")
```

### Loops
- **For Loop**:
  ```python
  for i in range(5):
      print(i)
  ```
- **While Loop**:
  ```python
  i = 0
  while i < 5:
      print(i)
      i += 1
  ```

### Break, Continue, Pass
- **Break**: Exit a loop.
- **Continue**: Skip to the next iteration.
- **Pass**: Placeholder for future code.

### Exercises
1. Write a program to check if a number is even or odd.
2. Print numbers from 1 to 10 using a while loop.

## 4. Functions

### Defining Functions
```python
def greet(name):
    return f"Hello, {name}!"
print(greet("Alice"))
```

### Parameters and Arguments
- **Positional**: Order matters.
- **Keyword**: Specify by name.
- **Default**: Set default values.
```python
def add(a, b=10):
    return a + b
print(add(5))  # Uses default b=10
```

### Scope
- **Local**: Variables inside functions.
- **Global**: Variables outside functions.

### Exercises
1. Create a function to calculate the area of a rectangle.
2. Write a function with default arguments.

## 5. Data Structures

### Lists
```python
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")
```

### Tuples
```python
colors = ("red", "green", "blue")
```

### Dictionaries
```python
person = {"name": "Alice", "age": 30}
print(person["name"])
```

### Sets
```python
numbers = {1, 2, 3, 4, 4}  # Duplicates removed
```

### Exercises
1. Add an element to a list and remove another.
2. Create a dictionary with your details and access a value.

## 6. Modules and Packages

### Importing Modules
```python
import math
print(math.pi)
```

### Creating Modules
Save functions in a `.py` file and import them.
```python
# mymodule.py
def say_hello():
    print("Hello from module!")
```
```python
# main.py
import mymodule
mymodule.say_hello()
```

### Standard Libraries
- `math`, `random`, `os`, `sys`

### Exercises
1. Use the `math` module to calculate the square root.
2. Create a custom module with a function and import it.

## 7. File Handling

### Reading Files
```python
with open("file.txt", "r") as f:
    content = f.read()
    print(content)
```

### Writing Files
```python
with open("file.txt", "w") as f:
    f.write("Hello, World!")
```

### CSV and JSON
- Use `csv` and `json` modules for structured data.
```python
import csv
with open("data.csv", "w", newline="") as f:
    writer = csv.writer(f)
    writer.writerow(["Name", "Age"])
    writer.writerow(["Alice", 30])
```

### Exercises
1. Read a text file and print its contents.
2. Write a list of numbers to a CSV file.

## 8. Object-Oriented Programming

### Classes and Objects
```python
class Dog:
    def __init__(self, name):
        self.name = name
    def bark(self):
        return f"{self.name} barks!"
dog = Dog("Buddy")
print(dog.bark())
```

### Inheritance
```python
class Animal:
    def __init__(self, name):
        self.name = name
class Dog(Animal):
    def bark(self):
        return f"{self.name} barks!"
```

### Polymorphism
Different classes can share method names.

### Exercises
1. Create a `Car` class with attributes and methods.
2. Implement inheritance for a `SportsCar` class.

## 9. Exception Handling

### Try-Except
```python
try:
    x = 1 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
```

### Raising Exceptions
```python
x = -1
if x < 0:
    raise ValueError("Number must be positive")
```

### Exercises
1. Handle a `ValueError` when converting a string to an integer.
2. Create a custom exception for invalid input.

## 10. Advanced Topics

### Decorators
```python
def decorator(func):
    def wrapper():
        print("Before")
        func()
        print("After")
    return wrapper
@decorator
def say_hello():
    print("Hello")
say_hello()
```

### Generators
```python
def fibonacci(n):
    a, b = 0, 1
    for _ in range(n):
        yield a
        a, b = b, a + b
```

### Context Managers
```python
with open("file.txt", "r") as f:
    print(f.read())
```

### Exercises
1. Write a decorator to log function calls.
2. Create a generator for Fibonacci numbers.

## 11. Standard Libraries

### `os` and `sys`
- `os`: File and directory operations.
- `sys`: System-specific parameters.
```python
import os
print(os.listdir())
```

### `datetime` and `re`
- `datetime`: Date and time handling.
- `re`: Regular expressions.
```python
import re
text = "My number is 123"
numbers = re.findall(r"\d+", text)
```

### Exercises
1. List all files in a directory using `os`.
2. Use `re` to find all numbers in a string.

## 12. Web Development

### Django and Flask
- **Django**: Full-stack framework.
- **Flask**: Lightweight framework.

### Example: Simple Flask App
```python
from flask import Flask
app = Flask(__name__)
@app.route("/")
def hello():
    return "Hello, World!"
app.run()
```

### Exercises
1. Set up a basic Flask app.
2. Create a Django project and run the server.

## 13. Data Science

### NumPy and Pandas
- **NumPy**: Numerical computations.
- **Pandas**: Data manipulation.
```python
import numpy as np
array = np.array([1, 2, 3])
import pandas as pd
df = pd.DataFrame({"Name": ["Alice"], "Age": [30]})
```

### Matplotlib and Seaborn
- **Matplotlib**: Basic plotting.
- **Seaborn**: Advanced visualizations.
```python
import matplotlib.pyplot as plt
plt.plot([1, 2, 3], [4, 5, 6])
plt.show()
```

### Exercises
1. Create a NumPy array and perform operations.
2. Load a CSV file into a Pandas DataFrame and analyze it.

## 14. Projects

### Project 1: Simple Calculator
```python
def calculator():
    num1 = float(input("Enter first number: "))
    op = input("Enter operation (+, -, *, /): ")
    num2 = float(input("Enter second number: "))
    if op == "+":
        result = num1 + num2
    elif op == "-":
        result = num1 - num2
    elif op == "*":
        result = num1 * num2
    elif op == "/":
        if num2 != 0:
            result = num1 / num2
        else:
            return "Error: Division by zero"
    else:
        return "Invalid operation"
    return f"Result: {result}"
print(calculator())
```

### Project 2: To-Do List App
```python
tasks = []
def add_task(task):
    tasks.append(task)
def view_tasks():
    for i, task in enumerate(tasks, 1):
        print(f"{i}. {task}")
add_task("Buy groceries")
view_tasks()
```

### Project 3: Web Scraper
```python
import requests
from bs4 import BeautifulSoup
url = "https://example.com"
response = requests.get(url)
soup = BeautifulSoup(response.text, "html.parser")
print(soup.title.text)
```

### Exercises
1. Implement the calculator project.
2. Extend the to-do list app with save/load functionality.

## 15. Best Practices

### PEP 8
Follow style guidelines for readability ([PEP 8](https://www.python.org/dev/peps/pep-0008/)).

### Debugging
Use `print` or tools like `pdb`.

### Version Control
Use Git for tracking changes ([Git](https://git-scm.com/)).

### Exercises
1. Format a script according to PEP 8.
2. Set up a Git repository for your projects.

## 16. Conclusion

### Further Resources
- **Books**: *Python Crash Course*, *Automate the Boring Stuff with Python*
- **Online Courses**: Codecademy, Coursera
- **Communities**: Stack Overflow, Reddit (r/learnpython)

### Final Thoughts
This e-book provides a foundation for Python programming. Practice regularly, build projects, and engage with the community to deepen your skills.
