[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15339639&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   **Python is a high-level, interpreted programming language known for its readability and simplicity. It supports multiple programming paradigms, including procedural, object-oriented, and functional programming. Python is widely used in web development, data analysis, scientific computing, artificial intelligence, and more.**
   ## Key Features of Python
- **Easy to Read and Write:** Python's syntax is clean and easy to understand, making it beginner-friendly.
- **Interpreted Language:** Python code is executed line by line, which makes debugging easier.
- **Dynamic Typing:** Variables in Python are not bound to a specific data type, and their types can change at runtime.
- **Extensive Standard Library:** Python has a vast standard library that supports many common programming tasks.
- **Cross-Platform:** Python can run on various operating systems, including Windows, macOS, and Linux.
- **Community Support:** Python has a large and active community, contributing to a wealth of resources and libraries.

## Use Cases
- **Web Development:** Using frameworks like Django and Flask.
- **Data Science and Machine Learning:** With libraries such as Pandas, NumPy, and scikit-learn.
- **Automation and Scripting:** For automating repetitive tasks.
- **Software Development:** Building applications with GUI frameworks like Tkinter and PyQt.



2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
   ### Windows
      1.**Download the Python installer from [python.org](https://www.python.org/).**

      2. **Run the installer and check the box to "Add Python to PATH."**
      3. Follow the prompts to complete the installation.
      4. **Verify the installation by opening Command Prompt and typing:** python --version

     **To install a virtual envririnment one needs to open up a termina(git bash) and write the following command**:
         pip install virtualenv

      **To Create a virtual environment we write the following command**:
         **virtualenv myenv**
         **where myenv is the name of the vitual environment**

      **To Activate the virtual environment created we write the following commmand**:
         **myenv\Scripts\activate**

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   
         print("Hello, World!")
         
   - print is a built-in function that outputs text to the console.
   - "Hello, World!" is a string literal enclosed in double quotes.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

      - int: Integer numbers 

               x = 5000
               print(type(x), x)

      - float: Floating-point numbers

               y = 3.14 
               print(type(y), y)
      - str: Strings (text)

               name = "Omondi Timon"
               print(type(name), name)
      - bool: Boolean values (True or False)

               is_student = True
               print(type(is_student), is_student)

      - list: Ordered, mutable collections of elements

               numbers = [99, 69, 333, 222, 556]
               print(type(numbers), numbers)

      - tuple: Ordered, immutable collections of elements

              coordinates = (67.09, 55.55)
              print(type(coordinates), coordinates)

      - dict: Unordered collections of key-value pairs

              person = {"name": "Rich", "age": 20}
              print(type(person), person)
      - set: Unordered collections of unique elements

              unique_numbers = {20, 40, 36, 39, 69}
              print(type(unique_numbers), unique_numbers)


5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
   
      **Conditional statements in Python allow one to execute certain blocks of code based on specific conditions allocated. The most common conditional statements are `if` and `else`.**

               age = 20
               if age < 18:
                  print("You are a minor.")
               else:
                  print("You are an adult.")
    Example of a for loop which prints numbers between 1 to 5:

               for i in range(5):
                  print(i)
   

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
   
      **Functions are reusable blocks of code that perform a specific task. They help in organizing and managing code efficiently.**

               def add(a, b):
                  return a + b

               result = add(5, 3)
               print(result)


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   ### Differences Between Lists and Dictionaries
      Lists:
      Ordered collections of items.
      Items are accessed by their position (index).
      Allows duplicate elements.
      Syntax: list_name = [item1, item2, item3]

            numbers_list = [1, 2, 3, 4, 5]
            numbers_list.append(6)  # Adding an element
            numbers_list.remove(3)  # Removing an element
            print("Updated List:", numbers_list)

      Dictionaries:

      Unordered collections of key-value pairs.
      Items are accessed by their keys.
      Keys must be unique.
      Syntax: dict_name = {key1: value1, key2: value2, key3: value3}
      x
            info_dict = {
                  'name': 'Alice',
                  'age': 30,
                  'city': 'New York'
            }
                  info_dict['age'] = 31  # Updating a value
            info_dict['country'] = 'USA'  # Adding a new key-value pair
            print("Updated Dictionary:", info_dict)

8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

      **Exception handling in Python is a way to handle runtime errors, allowing the program to continue execution or fail gracefully. The try, except, and finally blocks are used to catch and handle exceptions.**

             try:
                  numerator = 10
                  denominator = 0
                  result = numerator / denominator
             except ZeroDivisionError:
                  print("Error: Division by zero is not allowed.")
             finally:
                  print("This will always be executed.")



9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   **Modules are files containing Python code, which can include functions, classes, and variables. They help in organizing code into manageable and reusable components. You can create your own modules or use built-in and third-party modules.**

   The below code finds the square root of a number:

         import math

         # Using a function from the math module
         result = math.sqrt(16)
         print(result)


10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

            with open('example.txt', 'r') as file:
            content = file.read()
            print(content)

      For writing a file:

               lines = ["First line", "Second line", "Third line"]

                with open('output.txt', 'w') as file:
                     for line in lines:
                        file.write(line + '\n')

## REFERNCES
 - Python Software Foundation. (n.d.). Python documentation. Python.org. Retrieved from https://www.python.org/doc/
 - Python Software Foundation. (n.d.). Python installer for Windows. Python.org. Retrieved from https://www.python.org/downloads/windows/
 - W3Schools. (n.d.). Python Tutorial. Retrieved June 28, 2024, from https://www.w3schools.com/python/

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


