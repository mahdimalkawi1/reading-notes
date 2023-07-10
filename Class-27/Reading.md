# Read: Class 27

## Django Models:

### Q1. Explain the purpose and basic structure of Django models. How do they help in creating and managing database schema in a Django application?

Django models are Python classes that represent database tables. They define the structure and behavior of data in the tables. Models help create and manage the database schema in a Django application by abstracting away database details and providing an easy API for data manipulation. Models define fields and relationships between tables. Migrations handle schema changes based on model modifications. Models also offer query APIs for retrieving data from the database.


### Q2. Describe the primary features and functionality of the Django Admin interface. How can it be customized to suit the specific needs of a project?

The Django Admin interface is a built-in feature that provides an easy-to-use interface for managing database data. It offers CRUD operations, search/filtering, bulk actions, and permissions. The Admin interface is customizable by defining model-specific behaviors, customizing templates, adding custom actions, extending Admin classes, or using third-party packages. Customization allows adapting the interface to project requirements.


### Q3. Briefly outline the key components and workflow of a Django application, as discussed in the Beginner’s Guide to Django. How do these components interact with each other to create a functional web application?

A Django application consists of models, views, URLs, templates, and forms. Users send requests, URLs map them to views, which interact with models and process data. Views generate responses using templates, and the resulting HTML is sent back to users. Models handle database interactions, views handle logic, templates create the user interface, and URLs connect everything together.




