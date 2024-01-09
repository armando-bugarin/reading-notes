# Read: Class 03

1. **What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?** The 'with' statement in Python is used for context management. When opening a file using the 'with' statement, it ensures that the file is properly opened and closed. The main advantage is that it automatically takes care of resource management, releasing system resources (such as file handles) when they are no longer needed. This is done through the implementation of the context management protocol, and it simplifies the code by eliminating the need for explicit close statements.

2. **Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method.** Use read() when you want to read the entire content or a specific number of characters, and use readline() when you want to read line by line, especially in a loop until the end of the file is reached.

3. **Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.** Exception handling is a mechanism to gracefully handle errors in a program. The 'try', 'except', and 'finally' blocks are used for this purpose.

try: Contains the code that might raise an exception.

except: Contains the code to be executed if an exception is raised.

finally: Contains code that will be executed no matter what, whether an exception occurs or not.

try:
    x = 10 / 0
except ZeroDivisionError:
    print("Error: Division by zero!")
finally:
    print("This will be executed regardless of whether an exception occurred or not.")

## `Things I want to know more about`
