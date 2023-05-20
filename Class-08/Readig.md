# Read: Class 08

## Ten Thousand 3:

### Q1. What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers.

The basic syntax of Python list comprehension is:

``` python
new_list = [expression for item in iterable if condition]


```
List comprehension allows you to create a new list in a concise and readable manner.

##### Example:
``` python
squared_numbers = [x**2 for x in numbers]


```


### Q2. What is a decorator in Python?

Design pattern that allows you to modify the behavior of a function or class without directly changing its source code. Decorators use a decorator function to wrap the original function or class, providing additional functionality. Decorators are denoted using the @ symbol followed by the decorator function name above the function or class definition.


### Q3. Explain the concept of decorators in Python. How do they work, and what are some common use cases for them? Provide an example of a simple decorator function from the reading.

Decorators are commonly used for logging, timing, authentication, caching, validation, and more. They provide a concise way to enhance existing functionality in a modular and reusable manner.

##### Example:

``` python
@uppercase_decorator
def greet(name):
    return f"Hello, {name}!"

print(greet("Mahdi"))

```