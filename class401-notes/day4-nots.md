# Read: Class 04

1. **What are the key differences between classes and objects in Python, and how are they used to create and manage instances of a class?** 

Classes: In Python, a class is a blueprint or a template for creating objects. It defines attributes and methods that will be shared by all instances (objects) created from it. Classes are defined using the class keyword.

Objects: Objects are instances of a class. They represent concrete instances created based on the structure defined by the class. You can create multiple objects from the same class, and each object is a separate entity with its own set of attributes.

Creating and Managing Instances: To create an instance of a class, you call the class as if it were a function. The __init__ method is commonly used for initializing the attributes of the object.

2. **Explain the concept of recursion and provide an example of how it can be used to solve a problem in Python. What are some best practices to follow when implementing a recursive function?**

Recursion is a programming concept where a function calls itself in its own definition. In Python, a function can call itself to solve a smaller instance of the same problem, usually with simpler input.

3. **What is the purpose of pytest fixtures and code coverage in testing Python code? Explain how they can be used together to improve the quality and maintainability of a project.**

Pytest Fixtures: Fixtures in pytest are a way to set up preconditions for tests. They provide a way to initialize resources or data that is needed for testing. Fixtures can be used to create and provide test-specific data or objects.

Code Coverage: Code coverage measures how much of your code is executed during testing. It helps identify areas of code that are not covered by tests. Tools like pytest-cov can be used with pytest to measure code coverage.

Using Together:

Fixture Setup: Use fixtures to set up the necessary environment or data for your tests.

Code Coverage Measurement: Run tests with code coverage tools to identify which parts of your code are executed during the tests.

Improve Testing Quality: By ensuring comprehensive test coverage, you increase confidence in the reliability of your code.

## `Things I want to know more about`
