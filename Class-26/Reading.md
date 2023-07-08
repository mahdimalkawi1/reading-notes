# Read: Class 17

## Intro to Django:

### Q1. What are the key components of the Django framework, and how do they contribute to building a web application?



#### The key components of the Django framework are:

- Models: Define the database structure and handle interactions with the database.
- Views: Handle user requests, process data, and generate responses.
- Templates: Define the structure and layout of HTML pages.
- URL Dispatcher: Maps URLs to appropriate views.
- Forms: Simplify user input handling and validation.
- Middleware: Intercepts and processes requests and responses.
- Admin Interface: Provides a web-based interface for managing data.


### Q2. Explain the role of Django’s MTV (Model-View-Template) architecture and how it handles a typical web request-response cycle.

Django's MTV (Model-View-Template) architecture separates the concerns of data, logic, and presentation.

- Model: Represents the data structure and interacts with the database.
- Template: Defines the HTML layout and dynamically renders data.
- View: Handles requests, retrieves data from the Model, and passes it to the Template for rendering.<br>


During a web request-response cycle, Django's URL dispatcher maps the URL to the appropriate View. The View interacts with the Model, retrieves data, and passes it to the Template. The Template generates an HTML response, which is sent back to the user's browser for rendering. This architecture promotes code modularity and separation of concerns.


### Q3. What is the purpose of Tailwind CSS, and how does it differ from Bootstrap CSS?

Tailwind CSS is a utility-first CSS framework that offers a wide range of utility classes for precise styling control. It emphasizes customization and lets you compose styles by directly applying classes to HTML elements. In contrast, Bootstrap CSS is a feature-rich framework that provides pre-designed components and a responsive grid system for faster development. It focuses on consistency and offers ready-to-use UI components.




