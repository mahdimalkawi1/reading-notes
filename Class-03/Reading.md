# Read: Class 03

## FileIO & Exceptions:

### Q1. What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?

The 'with' statement in Python helps manage file resources by automatically opening and closing the file, ensuring that resources are properly released and reducing the risk of errors. It also allows for cleaner code by eliminating the need for explicit calls to open and close the file.

### Q2. Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method.

The read() method is used to read the entire contents of a file, while the readline() method is used to read a single line of text at a time. The read() method is useful when you want to process the entire contents of a file, while the readline() method is useful when you want to read a file line by line, such as when processing a large text file or log file.


### Q3. Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.


Exception handling is a way to handle errors and unexpected situations in Python. It uses the try, except, and finally blocks. The try block contains code that may raise an exception, while the except block is used to handle the exception if it occurs. The finally block is used to execute code that should always run, regardless of whether an exception was raised or not.

#### Example:

try: <br>

code that may raise an exception <br>

except: <br>

handle the exception <br>

finally:<br>

code that should always run <br>
