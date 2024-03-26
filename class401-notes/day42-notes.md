# Read: Class 42

1. **What are dunder methods in Python, and how do they allow for the customization of built-in behavior in classes? Provide an example of a common dunder method and its purpose.**

Dunder methods, short for "double underscore" methods, are special methods in Python that are surrounded by double underscores on both sides of their name (e.g., __init__, __str__). These methods allow customization of built-in behavior for classes. They are also called magic methods or special methods.

class MyClass:
    def __init__(self, value):
        self.value = value

    def __str__(self):
        return f"MyClass instance with value: {self.value}"

obj = MyClass(42)
print(obj)  # This will call the __str__ method implicitly

2. **Explain the concept of an iterator in Python. How do you create a custom iterator using the iter() and next() methods, and why are they important for enabling iteration in a class?**

An iterator in Python is an object that can be iterated (looped) over. It defines two methods: __iter__ and __next__. The __iter__ method returns the iterator object itself, and the __next__ method returns the next value from the iterator.

3. **What is a generator in Python, and how does it differ from a regular function? Illustrate your answer with an example of a generator function using the ‘yield’ keyword.**

Generators are a type of iterable, like iterators, but they are created using a function with the yield keyword. Unlike a regular function that returns a value and its state is not preserved, a generator function will maintain its state between calls.

4. **Define decorators in Python and explain their primary use case. How can you create and apply a custom decorator to a function or method? Provide a simple example to demonstrate this concept.**

Decorators in Python are a way to modify or extend the behavior of functions or methods. They use the @decorator syntax. A decorator is a function that takes another function as an argument and returns a new function that usually extends or modifies the behavior of the original function.

## `Things I want to know more about`
