# Read: Class 07

## Ten Thousand 2:

### Q1. Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.

Variable scope in Python refers to where a variable is recognized and can be accessed. Python has two types of variable scope:

- Local Scope: Variables defined within a function or block are local and can only be accessed within that function or block. They exist only while the function or block is executing.

##### Example:

def my_function():
    x = 10  # Local variable
    print(x)

my_function()  # Output: 10

print(x)  # Raises NameError: name 'x' is not defined


- Global Scope: Variables defined outside any function or block are global and can be accessed from anywhere in the program. They exist throughout the program's execution.

##### Example:

x = 10  # Global variable

def my_function():
    print(x)

my_function()  # Output: 10

def modify_variable():
    global x
    x = 20

modify_variable()
print(x)  # Output: 20

### Q2. How do the global and nonlocal keywords work in Python, and in what situations might you use them?

The global and nonlocal keywords in Python are used to access and modify variables in different scopes:

- global keyword:
The global keyword is used to indicate that a variable is a global variable. It allows accessing and modifying the global variable from within a local scope, such as a function. By default, if a variable is assigned a value inside a function, it becomes a local variable. However, using global before the variable name tells Python to use the global variable instead.

- nonlocal keyword:
The nonlocal keyword is used to access and modify variables from an outer (enclosing) local scope in nested functions. It allows modifying variables in the nearest enclosing scope that are neither local nor global. This keyword is useful when working with nested functions where you want to access and update variables from an outer scope.

- global is used to access and modify global variables within a local scope, while nonlocal is used to access and modify variables from an outer local scope within nested functions. These keywords provide flexibility in handling variable scopes in Python.

### Q3. In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis.

Big O notation is a way to analyze and compare the efficiency of algorithms. It helps us understand how an algorithm's performance changes with larger inputs. By focusing on the most significant factors that impact performance, it simplifies analysis and allows us to make informed choices. Big O notation facilitates communication and collaboration among developers and researchers by providing a standardized language for discussing algorithmic complexity.

### Q4. Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials.

To simulate a dice roll in Python, you can use the random module.
#### Example:

import random

target = 6
num_trials = 100000

occurrences = sum(random.randint(1, 6) == target for _ in range(num_trials))
probability = occurrences / num_trials

print("Probability of rolling a", target, "over", num_trials, "trials:", probability)


In this code, we use a list comprehension to generate a sequence of True and False values indicating whether the dice roll matches the target number. The sum() function counts the number of True values, representing the occurrences of the desired outcome. The probability is calculated by dividing the occurrences by the total number of trials.