# Read: Class 32

## Permissions & Postgresql:

### Q1. What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?

Django Rest Framework (DRF) permissions are essential for securing APIs:

- Authentication: Verifies user identity and allows only authorized users to access resources.

- Permissions: Controls user actions on API endpoints, restricting unauthorized access.

- Object-level permissions: Fine-grained access controls for specific resources based on user roles or ownership.

- Throttling: Limits the number of requests per user to prevent abuse and denial-of-service attacks.

- CSRF Protection: Guards against CSRF attacks when using session-based authentication.

### Q2. In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’?

In SQL, the SELECT statement is used to retrieve data from a database table. It allows to specify which columns you want to retrieve and filter the rows based on certain conditions if needed.

To retrieve all columns from a table called 'employees,' you can use the '*' wildcard character, which represents all columns. Here's how you would use it:

``` python 

    SELECT *
    FROM employees;

```
This query will return all the rows and columns from the 'employees' table.


### Q3. Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?

In Django Rest Framework (DRF), Generic Views are pre-built view classes that provide common functionalities for handling typical use cases in building RESTful APIs. They help in reducing boilerplate code and promoting a more consistent and maintainable codebase. DRF offers several types of Generic Views, each catering to specific CRUD (Create, Retrieve, Update, Delete) operations and list views.

#### The key advantages of DRF Generic Views are:

- Reduction of Code Duplication: Generic Views encapsulate common patterns, allowing developers to reuse code and reduce the amount of repetitive code that needs to be written for various views.

- Consistency and Conventions: By using Generic Views, the API adheres to consistent patterns and follows conventions, making the codebase easier to understand and navigate.

- Flexibility and Customization: Despite being generic, these views can be customized and extended to suit specific requirements by overriding methods and attributes.

#### Example: ListAPIView

```python
# serializers.py
from rest_framework import serializers
from .models import Book

class BookSerializer(serializers.ModelSerializer):
    class Meta:
        model = Book
        fields = '__all__'

# views.py
from rest_framework.generics import ListAPIView
from .models import Book
from .serializers import BookSerializer

class BookListView(ListAPIView):
    queryset = Book.objects.all()
    serializer_class = BookSerializer

```