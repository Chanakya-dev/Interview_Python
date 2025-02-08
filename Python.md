### **Frequently Asked Python Interview Questions and Answers**  

#### **1. Python Basics**  

1. **What is Python?**  
   - Python is a high-level, interpreted programming language known for its simplicity and readability.  

2. **What are the key features of Python?**  
   - Python is interpreted, dynamically typed, object-oriented, and has extensive libraries.  

3. **What is the difference between Python 2 and Python 3?**  
   - Python 3 introduced print as a function, improved integer division, and better Unicode support.  

4. **How is Python interpreted?**  
   - Python code is executed line by line by the Python interpreter.  

5. **What is the use of Python virtual environments?**  
   - Virtual environments allow project-specific dependencies, avoiding conflicts between packages.  

#### **2. Data Types and Variables**  

6. **What are Python’s built-in data types?**  
   - `int`, `float`, `str`, `list`, `tuple`, `dict`, `set`, `bool`.  

7. **How do you define a variable in Python?**  
   - Just assign a value: `x = 10` (no need to declare type explicitly).  

8. **What is the difference between a list and a tuple?**  
   - A list is mutable (`[]`), while a tuple is immutable (`()`).  

9. **What is the difference between `is` and `==`?**  
   - `is` checks identity (memory location), while `==` checks value equality.  

10. **What is type casting in Python?**  
   - Converting data types using functions like `int()`, `str()`, `list()`, etc.  

#### **3. Control Flow and Loops**  

11. **What is the difference between `break`, `continue`, and `pass`?**  
   - `break` exits a loop, `continue` skips to the next iteration, and `pass` does nothing.  

12. **What is the difference between `for` and `while` loops?**  
   - `for` loops iterate over sequences, while `while` loops run based on a condition.  

13. **How do you handle exceptions in Python?**  
   - Using `try-except` blocks to catch and handle errors.  

#### **4. Functions and Modules**  

14. **How do you define a function in Python?**  
   - Using the `def` keyword:  
     ```python
     def my_function():
         return "Hello"
     ```  

15. **What is the difference between arguments and keyword arguments?**  
   - Positional arguments are passed in order, while keyword arguments specify parameter names.  

16. **What is a lambda function in Python?**  
   - A small anonymous function using the `lambda` keyword.  

17. **What are Python modules and packages?**  
   - Modules are single Python files, while packages are directories with multiple modules.  

18. **How do you import a module in Python?**  
   - Using `import module_name` or `from module_name import function`.  

#### **5. Object-Oriented Programming (OOP)**  

19. **What is a class in Python?**  
   - A class is a blueprint for objects, defined using the `class` keyword.  

20. **What is an object in Python?**  
   - An instance of a class that contains attributes and methods.  

21. **What is inheritance in Python?**  
   - A mechanism to allow a class to inherit attributes and methods from another class.  

22. **What is polymorphism in Python?**  
   - The ability of different classes to define methods with the same name but different behavior.  

23. **What is encapsulation?**  
   - Restricting direct access to data within a class using private (`_var`) and protected (`__var`) attributes.  

#### **6. File Handling**  

24. **How do you open a file in Python?**  
   - Using `open("filename", "mode")`.  

25. **What are the different file modes in Python?**  
   - `'r'` (read), `'w'` (write), `'a'` (append), `'r+'` (read/write).  

26. **How do you write data to a file?**  
   - Using `file.write("text")`.  

27. **How do you read a file in Python?**  
   - Using `file.read()` or `file.readlines()`.  

28. **How do you close a file in Python?**  
   - Using `file.close()` or the `with` statement.  

#### **7. Advanced Topics**  

29. **What is a generator in Python?**  
   - A function that returns an iterator using `yield`.  

30. **What is the difference between `deepcopy()` and `copy()`?**  
   - `copy()` creates a shallow copy, whereas `deepcopy()` creates an independent duplicate.  

31. **What is multithreading in Python?**  
   - Running multiple threads concurrently using the `threading` module.  

32. **What is the Global Interpreter Lock (GIL)?**  
   - A mutex that allows only one thread to execute at a time in Python.  

33. **What is Python’s `re` module used for?**  
   - Regular expressions for pattern matching in strings.  

34. **How do you work with JSON in Python?**  
   - Using the `json` module with `json.dumps()` and `json.loads()`.  

35. **What is `map()`, `filter()`, and `reduce()` in Python?**  
   - Higher-order functions for applying transformations to iterables.  

36. **How do you measure execution time in Python?**  
   - Using the `time` module’s `time.time()` or `timeit` module.  

37. **What is the difference between `None` and `0`?**  
   - `None` represents the absence of a value, while `0` is a numeric value.  

38. **What is a virtual environment in Python?**  
   - An isolated environment for managing dependencies using `venv`.  

39. **What is monkey patching in Python?**  
   - Dynamically modifying a module or class at runtime.  

40. **What is the `with` statement used for?**  
   - For resource management, such as handling files efficiently.  
