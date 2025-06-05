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

### 1.1 What is Programming?
Programming involves creating instructions for computers to perform tasks, such as building apps, analyzing data, or automating processes. It’s like giving a recipe to a chef, where the computer follows your steps to achieve a goal. Programming is essential in modern technology, powering everything from websites to AI systems.

#### Why Learn Programming?
- **Problem-Solving**: Develops logical thinking and structured problem-solving skills.
- **Career Opportunities**: High demand for programmers in software development, data science, and AI.
- **Automation**: Saves time by automating repetitive tasks.
- **Creativity**: Enables you to create games, apps, or innovative solutions.

#### Programming Languages
Python is one of many languages, each suited for specific tasks:
- **Python**: Beginner-friendly, versatile, used in web development and data science.
- **Java**: Common in enterprise applications and Android development.
- **C++**: High-performance, used in games and system programming.
- **JavaScript**: Essential for interactive web development.

### 1.2 Introduction to Python
Python, created by Guido van Rossum in 1991, is a high-level, interpreted language known for its readability and simplicity. Its design philosophy, outlined in [PEP 20](https://www.python.org/dev/peps/pep-0020/), emphasizes clarity and simplicity, making it ideal for beginners.

#### History of Python
- **1980s**: Guido van Rossum began working on Python at CWI in the Netherlands.
- **1991**: Python 0.9.0 was released, introducing core features.
- **2000**: Python 2.0 added list comprehensions and garbage collection.
- **2008**: Python 3.0 introduced breaking changes for better consistency.
- **2025**: Python 3.13.4 is the latest version, with features like JIT compilation.

#### Key Features
- **Readable Syntax**: Code resembles English, reducing the learning curve.
- **Dynamic Typing**: No need to declare variable types.
- **Interpreted**: Code runs line-by-line, simplifying debugging.
- **Extensive Libraries**: Includes standard libraries and third-party packages like NumPy and Django.
- **Cross-Platform**: Runs on Windows, macOS, Linux, and more.
- **Community Support**: Large community with resources like Stack Overflow and Reddit.

#### Applications
- **Web Development**: Frameworks like Django and Flask.
- **Data Science**: Libraries like Pandas, NumPy, and Matplotlib.
- **AI and Machine Learning**: TensorFlow, Scikit-learn, and PyTorch.
- **Automation**: Scripts for file management, web scraping, and more.
- **Game Development**: Pygame for creating games.
- **Scientific Computing**: Used in research and simulations.

#### Why Python for Beginners?
- **Simplicity**: Fewer lines of code compared to languages like C++.
- **Versatility**: Suitable for small scripts and large projects.
- **Job Market**: High demand for Python developers, with salaries ranging from $50,000 to $160,000 annually.

### 1.3 Setting Up Python
To start coding, you need to install Python and set up an environment.

#### Step 1: Install Python
- Download from [python.org/downloads/](https://www.python.org/downloads/).
- Choose Python 3.13.4 or later.
- On Windows, check “Add Python to PATH” during installation.
- Verify with:
  ```bash
  python --version
  ```
  Expected output: `Python 3.13.4`.

#### Step 2: Choose an IDE or Editor
- **IDLE**: Bundled with Python, simple for beginners.
- **Visual Studio Code**: Lightweight, with Python extensions ([VS Code](https://code.visualstudio.com/)).
- **PyCharm**: Professional IDE with advanced features ([PyCharm](https://www.jetbrains.com/pycharm/)).
- **Jupyter Notebook**: Ideal for data science ([Jupyter](https://jupyter.org/)).
- **Thonny**: Beginner-friendly IDE ([Thonny](https://thonny.org/)).

#### Step 3: Test Your Setup
Create a file `test.py`:
```python
print("Python is working!")
```
Run it:
```bash
python test.py
```
Output: `Python is working!`

### 1.4 Writing Your First Program
Let’s write a “Hello, World!” program:
```python
print("Hello, World!")
```
Save as `hello.py` and run:
```bash
python hello.py
```
Output: `Hello, World!`

#### Exploring the Code
- `print()`: Outputs text to the console.
- `"Hello, World!"`: A string, enclosed in quotes.
- Python files use the `.py` extension.

### 1.5 Basic Syntax Overview
Python’s syntax is designed for readability. Key elements include:

#### Variables
Variables store data and are created upon assignment:
```python
name = "Alice"
age = 25
height = 5.6
```
- No type declaration needed.
- Case-sensitive: `Name` and `name` are different.

#### Data Types
| Type         | Description                     | Example                     |
|--------------|---------------------------------|-----------------------------|
| Integer      | Whole numbers                  | `x = 5`                    |
| Float        | Decimal numbers                | `y = 5.0`                  |
| String       | Sequence of characters         | `s = "Hello"`              |
| Boolean      | True or False                  | `b = True`                 |
| List         | Ordered, mutable collection    | `lst = [1, 2, 3]`         |
| Tuple        | Ordered, immutable collection  | `tup = (1, 2, 3)`         |
| Dictionary   | Key-value pairs                | `dict = {"name": "Alice"}` |
| Set          | Unordered, unique collection   | `set = {1, 2, 3}`         |

#### Operators
- **Arithmetic**: `+`, `-`, `*`, `/`, `%`, `**`, `//`
- **Comparison**: `==`, `!=`, `>`, `<`, `>=`, `<=`
- **Logical**: `and`, `or`, `not`
Example:
```python
x = 10
y = 5
print(x + y)  # Output: 15
print(x > y)  # Output: True
```

#### Comments
- Single-line: `# This is a comment`
- Multi-line:
  ```python
  """
  This is a multi-line comment.
  It spans multiple lines.
  """
  ```

#### Indentation
Python uses indentation (4 spaces) to define code blocks:
```python
if True:
    print("This is indented")
```

### 1.6 Real-World Applications
Python’s simplicity makes it ideal for real-world tasks. For example, automating file renaming:
```python
import os
for filename in os.listdir():
    if filename.endswith(".txt"):
        os.rename(filename, filename.replace(".txt", ".py"))
```
This script renames all `.txt` files to `.py` in the current directory.

### 1.7 Common Pitfalls
- **Forgetting to Install Python**: Ensure Python is added to PATH.
- **Indentation Errors**: Always use consistent indentation (4 spaces).
- **Case Sensitivity**: `Name` and `name` are different variables.
- **Running Files**: Use the correct command (`python filename.py`).

### 1.8 Exercises
1. Install Python and verify the version.
2. Write a program to print your name and age.
3. Create variables for different data types and print their types using `type()`.
4. Write a program that takes user input for a name and prints a greeting.
5. Write a program to calculate the area of a rectangle based on user input.
6. Explore the Python documentation and find one new feature.
7. Write a program to print the first 10 numbers using a loop.
8. Create a script to check if a number is even or odd.
9. Write a program to concatenate two strings.
10. Experiment with different operators and print the results.

---

## 2. Basic Syntax

### 2.1 Variables
Variables store data and are created upon assignment without explicit declaration.

#### Declaration and Assignment
```python
x = 5  # Integer
y = "Hello"  # String
z = 3.14  # Float
```

#### Naming Conventions
- Start with a letter or underscore.
- Use letters, numbers, or underscores.
- Case-sensitive: `myVar` ≠ `myvar`.
- Avoid reserved keywords (e.g., `if`, `for`).

#### Dynamic Typing
Variables can change types:
```python
x = 5  # Integer
x = "Hello"  # Now a string
```

#### Multiple Assignments
```python
a, b, c = 1, 2, 3
x = y = z = 10
```

#### Deleting Variables
```python
del x
```

### 2.2 Data Types
Python’s built-in data types include:

#### Numeric Types
- **Integer**: Whole numbers.
  ```python
  x = 5
  print(type(x))  # <class 'int'>
  ```
- **Float**: Decimal numbers.
  ```python
  y = 3.14
  print(type(y))  # <class 'float'>
  ```
- **Complex**: Numbers with real and imaginary parts.
  ```python
  z = 3 + 4j
  print(type(z))  # <class 'complex'>
  ```

#### String Type
- Enclosed in single or double quotes.
- Methods: `upper()`, `lower()`, `strip()`, etc.
  ```python
  s = "Hello, World!"
  print(s.upper())  # HELLO, WORLD!
  ```

#### Boolean Type
- Represents `True` or `False`.
  ```python
  b = True
  print(type(b))  # <class 'bool'>
  ```

#### Sequence Types
- **List**: Ordered, mutable.
  ```python
  lst = [1, 2, 3]
  lst.append(4)
  print(lst)  # [1, 2, 3, 4]
  ```
- **Tuple**: Ordered, immutable.
  ```python
  tup = (1, 2, 3)
  print(tup[0])  # 1
  ```
- **Range**: Sequence of numbers.
  ```python
  r = range(5)
  print(list(r))  # [0, 1, 2, 3, 4]
  ```

#### Mapping Type
- **Dictionary**: Key-value pairs.
  ```python
  d = {"name": "Alice", "age": 30}
  print(d["name"])  # Alice
  ```

#### Set Types
- **Set**: Unordered, unique elements.
  ```python
  s = {1, 2, 3, 3}
  print(s)  # {1, 2, 3}
  ```
- **Frozen Set**: Immutable set.
  ```python
  fs = frozenset([1, 2, 3])
  ```

### 2.3 Operators
Operators perform operations on values.

#### Arithmetic Operators
| Operator | Description | Example |
|----------|-------------|---------|
| `+`      | Addition    | `5 + 3` |
| `-`      | Subtraction | `5 - 3` |
| `*`      | Multiplication | `5 * 3` |
| `/`      | Division    | `5 / 2` |
| `%`      | Modulus     | `5 % 2` |
| `**`     | Exponentiation | `5 ** 2` |
| `//`     | Floor Division | `5 // 2` |

#### Comparison Operators
| Operator | Description | Example |
|----------|-------------|---------|
| `==`     | Equal       | `5 == 5` |
| `!=`     | Not equal   | `5 != 3` |
| `>`      | Greater than | `5 > 3` |
| `<`      | Less than   | `5 < 3` |

#### Logical Operators
| Operator | Description | Example |
|----------|-------------|---------|
| `and`    | Logical AND | `True and False` |
| `or`     | Logical OR  | `True or False` |
| `not`    | Logical NOT | `not True` |

### 2.4 Input and Output
- **Output**: `print()` displays text.
  ```python
  print("Hello", "World", sep=", ")  # Hello, World
  ```
- **Input**: `input()` reads user input.
  ```python
  name = input("Enter your name: ")
  print(f"Hi, {name}!")
  ```

### 2.5 Comments
- Single-line: `# Comment`
- Multi-line: `""" Comment """`

### 2.6 Indentation
Indentation defines code blocks:
```python
if True:
    print("This is indented")
```

### 2.7 Exercises
1. Create variables for different data types and print them.
2. Swap two variables without using a temporary variable.
3. Write a program to calculate the square of a number.
4. Use `input()` to get a number and print its double.
5. Write a program to concatenate two strings.
6. Create a list and append an element.
7. Access a dictionary value by key.
8. Remove duplicates from a list using a set.
9. Use arithmetic operators to perform calculations.
10. Write a program to check if a string is empty.

---

## 3. Control Structures

### 3.1 If-Else Statements
Control program flow based on conditions.

#### Basic Syntax
```python
x = 10
if x > 0:
    print("Positive")
else:
    print("Non-positive")
```

#### Elif
```python
x = 0
if x > 0:
    print("Positive")
elif x < 0:
    print("Negative")
else:
    print("Zero")
```

#### Nested If
```python
x = 10
if x > 0:
    if x % 2 == 0:
        print("Positive even")
    else:
        print("Positive odd")
```

### 3.2 Loops
Loops repeat code blocks.

#### For Loop
Iterates over a sequence:
```python
for i in range(5):
    print(i)  # 0, 1, 2, 3, 4
```

#### While Loop
Repeats while a condition is true:
```python
i = 0
while i < 5:
    print(i)
    i += 1
```

#### Nested Loops
```python
for i in range(3):
    for j in range(3):
        print(f"({i}, {j})")
```

### 3.3 Loop Control Statements
- **Break**: Exits the loop.
  ```python
  for i in range(5):
      if i == 3:
          break
      print(i)
  ```
- **Continue**: Skips to the next iteration.
  ```python
  for i in range(5):
      if i == 3:
          continue
      print(i)
  ```
- **Pass**: Placeholder.
  ```python
  for i in range(5):
      if i == 3:
          pass
      print(i)
  ```

### 3.4 Exercises
1. Check if a number is positive, negative, or zero.
2. Print the first 10 natural numbers using a for loop.
3. Skip printing 5 and 6 in a loop using `continue`.
4. Print a multiplication table for a given number.
5. Check if a number is prime.
6. Print a pattern (e.g., triangle of stars).
7. Find the sum of numbers from 1 to 100.
8. Count vowels in a string.
9. Write a program to find the factorial of a number.
10. Use nested loops to create a 3x3 grid.

---

## 4. Functions

### 4.1 Defining Functions
Functions are reusable code blocks:
```python
def greet(name):
    return f"Hello, {name}!"
print(greet("Alice"))
```

### 4.2 Parameters and Arguments
- **Positional**: Order matters.
- **Keyword**: Specify by name.
- **Default**: Provide default values.
  ```python
  def add(a, b=10):
      return a + b
  print(add(5))  # 15
  ```

### 4.3 Return Values
Functions can return multiple values:
```python
def divide(a, b):
    return a // b, a % b
quotient, remainder = divide(10, 3)
```

### 4.4 Scope
- **Local**: Inside a function.
- **Global**: Outside functions.
  ```python
  x = 10
  def func():
      x = 5  # Local
      print(x)
  func()  # 5
  print(x)  # 10
  ```

### 4.5 Recursive Functions
```python
def factorial(n):
    if n == 1:
        return 1
    return n * factorial(n-1)
```

### 4.6 Lambda Functions
```python
double = lambda x: x * 2
print(double(5))  # 10
```

### 4.7 Exercises
1. Write a function to calculate the square of a number.
2. Create a function with default arguments.
3. Write a recursive function for Fibonacci numbers.
4. Use a lambda function to sort a list.
5. Write a function that returns multiple values.
6. Create a function to check if a string is a palindrome.
7. Write a function to find the maximum of three numbers.
8. Create a function to reverse a string.
9. Write a function to calculate the area of a circle.
10. Use a higher-order function to apply a function to a list.

---

## 5. Data Structures

### 5.1 Lists
Ordered, mutable collections:
```python
lst = [1, 2, 3]
lst.append(4)
print(lst)  # [1, 2, 3, 4]
```

#### Methods
- `append()`, `remove()`, `pop()`, `sort()`, `reverse()`

### 5.2 Tuples
Ordered, immutable:
```python
tup = (1, 2, 3)
print(tup[0])  # 1
```

### 5.3 Dictionaries
Key-value pairs:
```python
d = {"name": "Alice", "age": 30}
print(d["name"])  # Alice
```

### 5.4 Sets
Unordered, unique elements:
```python
s = {1, 2, 3, 3}
print(s)  # {1, 2, 3}
```

### 5.5 Strings
Immutable sequences:
```python
s = "Hello"
print(s.upper())  # HELLO
```

### 5.6 Exercises
1. Create a list and perform basic operations.
2. Access elements in a tuple.
3. Update a dictionary value.
4. Remove duplicates from a list using a set.
5. Reverse a string.
6. Sort a list in descending order.
7. Merge two dictionaries.
8. Create a list comprehension.
9. Check if an element exists in a set.
10. Split a string into a list of words.

---

## 6. Modules and Packages

### 6.1 Importing Modules
```python
import math
print(math.pi)  # 3.141592653589793
```

### 6.2 Creating Modules
Save in `mymodule.py`:
```python
def say_hello():
    print("Hello from module!")
```
Import:
```python
import mymodule
mymodule.say_hello()
```

### 6.3 Packages
Directories containing modules:
```python
from mypackage import mymodule
```

### 6.4 Exercises
1. Use the `math` module to calculate a square root.
2. Create a custom module with two functions.
3. Import a specific function from a module.
4. Use the `random` module to generate a random number.
5. Create a package with multiple modules.
6. Use the `datetime` module to get the current date.
7. Import a module with an alias.
8. Use the `os` module to list directory contents.
9. Create a module to calculate the area of shapes.
10. Explore the `sys` module.

---

## 7. File Handling

### 7.1 Reading Files
```python
with open("file.txt", "r") as f:
    content = f.read()
    print(content)
```

### 7.2 Writing Files
```python
with open("file.txt", "w") as f:
    f.write("Hello, World!")
```

### 7.3 CSV and JSON
```python
import csv
with open("data.csv", "w", newline="") as f:
    writer = csv.writer(f)
    writer.writerow(["Name", "Age"])
    writer.writerow(["Alice", 30])
```

### 7.4 Exercises
1. Read a text file and print its contents.
2. Write a list to a text file.
3. Create a CSV file with sample data.
4. Read a CSV file and print its contents.
5. Write a JSON file with a dictionary.
6. Append text to an existing file.
7. Count lines in a text file.
8. Read a file line by line.
9. Create a program to copy a file.
10. Use JSON to store and retrieve data.

---

## 8. Object-Oriented Programming

### 8.1 Classes and Objects
```python
class Dog:
    def __init__(self, name):
        self.name = name
    def bark(self):
        return f"{self.name} barks!"
dog = Dog("Buddy")
print(dog.bark())
```

### 8.2 Inheritance
```python
class Animal:
    def __init__(self, name):
        self.name = name
class Dog(Animal):
    def bark(self):
        return f"{self.name} barks!"
```

### 8.3 Polymorphism
```python
class Cat(Animal):
    def meow(self):
        return f"{self.name} meows!"
```

### 8.4 Exercises
1. Create a `Car` class with attributes and methods.
2. Implement inheritance for a `SportsCar` class.
3. Create a class with multiple methods.
4. Use polymorphism with two classes.
5. Create a class to represent a student.
6. Implement encapsulation with private attributes.
7. Create a class hierarchy for animals.
8. Write a class to calculate geometric shapes.
9. Create a class with a static method.
10. Use a class to manage a bank account.

---

## 9. Exception Handling

### 9.1 Try-Except
```python
try:
    x = 1 / 0
except ZeroDivisionError:
    print("Cannot divide by zero")
```

### 9.2 Raising Exceptions
```python
x = -1
if x < 0:
    raise ValueError("Number must be positive")
```

### 9.3 Custom Exceptions
```python
class CustomError(Exception):
    pass
```

### 9.4 Exercises
1. Handle a `ValueError` for invalid input.
2. Raise an exception for negative numbers.
3. Create a custom exception class.
4. Handle multiple exceptions in one try block.
5. Write a program to handle file errors.
6. Use `finally` in a try-except block.
7. Handle an index out-of-range error.
8. Create a program to validate user input.
9. Write a function that raises an exception.
10. Handle exceptions in a loop.

---

## 10. Advanced Topics

### 10.1 Decorators
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

### 10.2 Generators
```python
def fibonacci(n):
    a, b = 0, 1
    for _ in range(n):
        yield a
        a, b = b, a + b
```

### 10.3 Context Managers
```python
with open("file.txt", "r") as f:
    print(f.read())
```

### 10.4 Exercises
1. Write a decorator to log function calls.
2. Create a generator for even numbers.
3. Use a context manager to handle files.
4. Write a decorator to time function execution.
5. Create a generator for prime numbers.
6. Use a context manager for database connections.
7. Write a lambda function for sorting.
8. Create a decorator to check input types.
9. Write a generator to yield squares.
10. Use a context manager to manage resources.

---

## 11. Standard Libraries

### 11.1 `os` and `sys`
```python
import os
print(os.listdir())
```

### 11.2 `datetime`
```python
from datetime import datetime
print(datetime.now())
```

### 11.3 `re`
```python
import re
text = "My number is 123"
numbers = re.findall(r"\d+", text)
```

### 11.4 Exercises
1. List files in a directory using `os`.
2. Get the current date using `datetime`.
3. Use `re` to find emails in a text.
4. Use `sys` to get Python version.
5. Create a program to rename files using `os`.
6. Use `datetime` to calculate age.
7. Use `re` to validate a phone number.
8. Use `os` to create a directory.
9. Write a program to log events with `datetime`.
10. Use `sys` to handle command-line arguments.

---

# Python Development E-Book for Students (Chapters 12–16)

## Table of Contents
- [12. Web Development](#12-web-development)
- [13. Data Science](#13-data-science)
- [14. Projects](#14-projects)
- [15. Best Practices](#15-best-practices)
- [16. Conclusion](#16-conclusion)

## 12. Web Development

Web development involves creating applications accessible via the internet, combining frontend (user interface), backend (server logic), and databases. Python’s simplicity and powerful frameworks make it a top choice for backend development. This chapter explores Django and Flask, two popular frameworks, and covers setup, development, and deployment.

### 12.1 Introduction to Web Development with Python
Web applications consist of:
- **Frontend**: HTML, CSS, JavaScript for user interaction.
- **Backend**: Server-side logic handling requests and data.
- **Database**: Stores persistent data (e.g., SQLite, PostgreSQL).

Python excels in backend development due to:
- **Readability**: Clear syntax reduces development time.
- **Frameworks**: Django, Flask, and FastAPI simplify complex tasks.
- **Scalability**: Supports high-traffic applications like Instagram.
- **Community**: Extensive libraries and tutorials.

#### Key Concepts
- **HTTP**: Protocol for client-server communication (GET, POST methods).
- **REST**: Architectural style for APIs, emphasizing stateless operations.
- **MVC/MVT**: Django uses Model-View-Template (MVT) for organized code:
  - **Model**: Represents data structure.
  - **View**: Handles logic and returns responses.
  - **Template**: Defines the presentation layer.

#### Why Python for Web Development?
- **Ease of Use**: Minimal boilerplate code.
- **Versatility**: Suitable for small APIs or large-scale apps.
- **Security**: Frameworks include built-in protections (e.g., CSRF, XSS).

### 12.2 Django Web Framework
Django is a high-level framework promoting rapid development and clean design, used by companies like Instagram and Spotify.

#### 12.2.1 Setting Up Django
Install Django using pip:
```bash
pip install django
```
Create a project:
```bash
django-admin startproject myproject
cd myproject
```
This generates:
```
myproject/
    manage.py
    myproject/
        __init__.py
        settings.py
        urls.py
        asgi.py
        wsgi.py
```
Create an app:
```bash
python manage.py startapp myapp
```
Add `myapp` to `INSTALLED_APPS` in `settings.py`:
```python
INSTALLED_APPS = [
    ...
    'myapp',
]
```
Run the development server:
```bash
python manage.py runserver
```
Access at `http://127.0.0.1:8000`.

#### 12.2.2 Models and Database
Models define data structures. Example for a blog:
```python
# myapp/models.py
from django.db import models

class Post(models.Model):
    title = models.CharField(max_length=100)
    content = models.TextField()
    author = models.CharField(max_length=50)
    date_posted = models.DateTimeField(auto_now_add=True)

    def __str__(self):
        return self.title
```
Apply migrations:
```bash
python manage.py makemigrations
python manage.py migrate
```
Register the model in `admin.py`:
```python
# myapp/admin.py
from django.contrib import admin
from .models import Post

admin.site.register(Post)
```

#### 12.2.3 Views and Templates
Views process requests and return responses. Example:
```python
# myapp/views.py
from django.shortcuts import render
from .models import Post

def home(request):
    posts = Post.objects.all()
    return render(request, 'myapp/home.html', {'posts': posts})
```
Create a template (`myapp/templates/myapp/home.html`):
```html
<!DOCTYPE html>
<html>
<head>
    <title>Blog</title>
</head>
<body>
    <h1>Blog Posts</h1>
    {% for post in posts %}
        <h2>{{ post.title }}</h2>
        <p>{{ post.content }}</p>
        <p>By {{ post.author }} on {{ post.date_posted }}</p>
    {% endfor %}
</body>
</html>
```

#### 12.2.4 URLs and Routing
Map URLs to views in `myapp/urls.py`:
```python
from django.urls import path
from . import views

urlpatterns = [
    path('', views.home, name='home'),
]
```
Include in project `urls.py`:
```python
from django.contrib import admin
from django.urls import path, include

urlpatterns = [
    path('admin/', admin.site.urls),
    path('', include('myapp.urls')),
]
```

#### 12.2.5 Forms and User Input
Create a form:
```python
# myapp/forms.py
from django import forms

class PostForm(forms.ModelForm):
    class Meta:
        model = Post
        fields = ['title', 'content', 'author']
```
Handle form submission:
```python
# myapp/views.py
from django.shortcuts import render, redirect
from .forms import PostForm

def create_post(request):
    if request.method == 'POST':
        form = PostForm(request.POST)
        if form.is_valid():
            form.save()
            return redirect('home')
    else:
        form = PostForm()
    return render(request, 'myapp/create_post.html', {'form': form})
```
Template (`myapp/templates/myapp/create_post.html`):
```html
<form method="post">
    {% csrf_token %}
    {{ form.as_p }}
    <button type="submit">Submit</button>
</form>
```

#### 12.2.6 User Authentication
Django provides built-in authentication:
```python
# myproject/urls.py
from django.contrib.auth import views as auth_views

urlpatterns = [
    path('login/', auth_views.LoginView.as_view(template_name='myapp/login.html'), name='login'),
    path('logout/', auth_views.LogoutView.as_view(), name='logout'),
]
```
Login template (`myapp/templates/myapp/login.html`):
```html
<form method="post">
    {% csrf_token %}
    {{ form.as_p }}
    <button type="submit">Login</button>
</form>
```

#### 12.2.7 Advanced Topics
- **Class-Based Views**:
  ```python
  from django.views.generic import ListView
  class PostListView(ListView):
      model = Post
      template_name = 'myapp/home.html'
      context_object_name = 'posts'
  ```
- **Middleware**: Add custom request processing.
- **Signals**: Trigger actions on model changes.
- **Django Rest Framework**: Build APIs:
  ```python
  from rest_framework import serializers, viewsets
  class PostSerializer(serializers.ModelSerializer):
      class Meta:
          model = Post
          fields = '__all__'
  ```

#### 12.2.8 Deploying Django Applications
- Use Heroku:
  ```bash
  heroku create
  git push heroku main
  ```
- Configure `settings.py`:
  ```python
  DEBUG = False
  ALLOWED_HOSTS = ['your-app.herokuapp.com']
  ```

### 12.3 Flask Web Framework
Flask is a lightweight framework ideal for small projects or APIs.

#### 12.3.1 Setting Up Flask
Install Flask:
```bash
pip install flask
```
Create a simple app:
```python
# app.py
from flask import Flask
app = Flask(__name__)

@app.route('/')
def home():
    return "Hello, World!"

if __name__ == '__main__':
    app.run(debug=True)
```

#### 12.3.2 Routing
Handle dynamic routes:
```python
@app.route('/user/<username>')
def profile(username):
    return f"Welcome, {username}!"
```

#### 12.3.3 Templates
Use Jinja2:
```python
from flask import render_template

@app.route('/posts')
def posts():
    posts = [{'title': 'Post 1', 'content': 'Content 1'}]
    return render_template('posts.html', posts=posts)
```
Template (`templates/posts.html`):
```html
{% for post in posts %}
    <h2>{{ post.title }}</h2>
    <p>{{ post.content }}</p>
{% endfor %}
```

#### 12.3.4 Forms
Use Flask-WTF:
```python
from flask_wtf import FlaskForm
from wtforms import StringField, SubmitField

class PostForm(FlaskForm):
    title = StringField('Title')
    content = StringField('Content')
    submit = SubmitField('Submit')
```

#### 12.3.5 Database Integration
Use Flask-SQLAlchemy:
```python
from flask_sqlalchemy import SQLAlchemy
app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///site.db'
db = SQLAlchemy(app)

class Post(db.Model):
    id = db.Column(db.Integer, primary_key=True)
    title = db.Column(db.String(100))
    content = db.Column(db.Text)
```

#### 12.3.6 User Authentication
Use Flask-Login:
```python
from flask_login import LoginManager, UserMixin

login_manager = LoginManager(app)

class User(UserMixin, db.Model):
    id = db.Column(db.Integer, primary_key=True)
    username = db.Column(db.String(80), unique=True)
```

#### 12.3.7 Building APIs
Use Flask-RESTful:
```python
from flask_restful import Resource, Api
api = Api(app)

class PostAPI(Resource):
    def get(self):
        return {'posts': [{'id': 1, 'title': 'Post 1'}]}
api.add_resource(PostAPI, '/api/posts')
```

#### 12.3.8 Deploying Flask Applications
Use Gunicorn and Heroku:
```bash
pip install gunicorn
gunicorn -w 4 app:app
```

### 12.4 Comparing Django and Flask
| Feature          | Django                     | Flask                     |
|------------------|----------------------------|---------------------------|
| Type             | Full-stack                | Micro-framework           |
| Use Case         | Large, complex apps       | Small apps, APIs          |
| Built-in Features| Admin, ORM, Auth          | Minimal, extensible       |
| Learning Curve   | Steeper                   | Easier                    |

### 12.5 Other Python Web Frameworks
- **FastAPI**: High-performance for APIs.
- **Pyramid**: Flexible for various project sizes.

### 12.6 Best Practices
- **Security**: Use HTTPS, validate inputs.
- **Performance**: Cache responses, optimize queries.
- **Testing**: Use `unittest` or `pytest`.

### 12.7 Real-World Examples
- **Django Blog**: Full-stack blog with authentication.
- **Flask API**: To-do list API with CRUD operations.

### 12.8 Exercises
1. Create a Django project with a blog app.
2. Build a Flask app with a simple form.
3. Implement user authentication in Django.
4. Create a REST API with Flask-RESTful.
5. Deploy a Django app to Heroku.
6. Use Flask-SQLAlchemy to manage a database.
7. Create a template with dynamic data in Django.
8. Handle form validation in Flask.
9. Build a simple API with FastAPI.
10. Optimize a Django query for performance.

## 13. Data Science

Data science involves analyzing data to extract insights, and Python’s libraries make it accessible and powerful.

### 13.1 Introduction to Data Science
Data science combines statistics, programming, and domain knowledge to solve problems in fields like finance, healthcare, and marketing.

#### Why Python?
- **Libraries**: NumPy, Pandas, Matplotlib, Scikit-learn.
- **Community**: Extensive tutorials and forums.
- **Flexibility**: Handles data analysis, visualization, and machine learning.

### 13.2 NumPy: Numerical Computing
NumPy provides efficient array operations.

#### 13.2.1 Introduction to NumPy
Install:
```bash
pip install numpy
```

#### 13.2.2 NumPy Arrays
Create arrays:
```python
import numpy as np
arr = np.array([1, 2, 3])
arr2d = np.array([[1, 2], [3, 4]])
```

#### 13.2.3 Mathematical Operations
```python
arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6])
print(arr1 + arr2)  # [5 7 9]
print(np.mean(arr1))  # 2.0
```

#### 13.2.4 Indexing and Slicing
```python
print(arr[1:3])  # [2 3]
```

### 13.3 Pandas: Data Manipulation
Pandas handles structured data.

#### 13.3.1 Series and DataFrames
```python
import pandas as pd
s = pd.Series([1, 2, 3], index=['a', 'b', 'c'])
df = pd.DataFrame({'Name': ['Alice', 'Bob'], 'Age': [25, 30]})
```

#### 13.3.2 Data Cleaning
Handle missing data:
```python
df['Age'].fillna(df['Age'].mean(), inplace=True)
```

#### 13.3.3 Reading/Writing Data
```python
df = pd.read_csv('data.csv')
df.to_csv('output.csv')
```

### 13.4 Data Visualization
#### 13.4.1 Matplotlib
```python
import matplotlib.pyplot as plt
plt.plot([1, 2, 3], [4, 5, 6], label='Line')
plt.legend()
plt.show()
```

#### 13.4.2 Seaborn
```python
import seaborn as sns
sns.scatterplot(x='Age', y='Salary', data=df)
plt.show()
```

### 13.5 Machine Learning with Scikit-learn
#### 13.5.1 Supervised Learning
Example (Logistic Regression):
```python
from sklearn.linear_model import LogisticRegression
from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
model = LogisticRegression()
model.fit(X_train, y_train)
```

#### 13.5.2 Unsupervised Learning
K-means clustering:
```python
from sklearn.cluster import KMeans
kmeans = KMeans(n_clusters=3)
kmeans.fit(X)
```

### 13.6 Real-World Projects
- **Sales Analysis**: Use Pandas to analyze sales data.
- **Churn Prediction**: Build a model to predict customer churn.

### 13.7 Exercises
1. Create a NumPy array and perform operations.
2. Load a CSV file with Pandas.
3. Visualize data with Matplotlib.
4. Build a classification model with Scikit-learn.
5. Clean a dataset with missing values.
6. Create a Seaborn pairplot.
7. Perform statistical analysis with NumPy.
8. Merge two DataFrames.
9. Train a regression model.
10. Cluster data using K-means.

## 14. Projects

Projects reinforce learning through practical application. Below are five detailed projects.

### 14.1 Simple Blog with Django
#### 14.1.1 Overview
Build a blog with user authentication, posts, and comments.

#### 14.1.2 Steps
- Set up Django project and app.
- Define models:
  ```python
  class Comment(models.Model):
      post = models.ForeignKey(Post, on_delete=models.CASCADE)
      content = models.TextField()
      author = models.CharField(max_length=50)
  ```
- Create views, templates, and URLs.
- Implement authentication and deployment.

### 14.2 Titanic Survival Prediction
#### 14.2.1 Overview
Predict survival using the Titanic dataset.

#### 14.2.2 Steps
- Load data:
  ```python
  df = pd.read_csv('titanic.csv')
  ```
- Clean data (handle missing values, encode categories).
- Train a model:
  ```python
  from sklearn.ensemble import RandomForestClassifier
  model = RandomForestClassifier()
  ```

### 14.3 File Organizer
#### 14.3.1 Overview
Organize files by type.

#### 14.3.2 Steps
```python
import os
import shutil
for file in os.listdir():
    if file.endswith('.jpg'):
        shutil.move(file, 'images/')
```

### 14.4 Tic-Tac-Toe with Pygame
#### 14.4.1 Overview
Build a Tic-Tac-Toe game.

#### 14.4.2 Steps
```python
import pygame
pygame.init()
screen = pygame.display.set_mode((400, 400))
```

### 14.5 To-Do List API with Flask
#### 14.5.1 Overview
Create a REST API for tasks.

#### 14.5.2 Steps
```python
from flask_restful import Resource
class TaskAPI(Resource):
    def get(self):
        return {'tasks': []}
```

### 14.6 Exercises
1. Complete the Django blog project.
2. Analyze the Titanic dataset.
3. Build the file organizer.
4. Create the Tic-Tac-Toe game.
5. Implement the Flask API.

## 15. Best Practices

Adopting best practices ensures maintainable, efficient code.

### 15.1 Coding Standards
Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/) for style:
- Use 4 spaces for indentation.
- Limit lines to 79 characters.

### 15.2 Debugging
Use `pdb`:
```python
import pdb
pdb.set_trace()
```

### 15.3 Version Control
Use Git:
```bash
git init
git add .
git commit -m "Initial commit"
```

### 15.4 Testing
Use `pytest`:
```python
def test_add():
    assert add(2, 3) == 5
```

### 15.5 Performance
Profile with `cProfile`:
```python
import cProfile
cProfile.run('my_function()')
```

### 15.6 Exercises
1. Format code per PEP 8.
2. Debug a program with `pdb`.
3. Set up a Git repository.
4. Write unit tests with `pytest`.
5. Optimize a slow function.

## 16. Conclusion

### 16.1 Summary
This e-book covers Python from basics to advanced topics, including web development, data science, and projects.

### 16.2 Further Learning
- **Books**: *Python Crash Course*, *Automate the Boring Stuff with Python*.
- **Courses**: [Codecademy](https://www.codecademy.com/learn/learn-python-3), [Coursera](https://www.coursera.org).
- **Communities**: [Stack Overflow](https://stackoverflow.com), [Reddit](https://www.reddit.com/r/learnpython).

### 16.3 Encouragement
Continue building projects and contributing to open-source communities.
