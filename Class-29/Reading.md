# Read: Class 29

## Django Custom User:

### Q1. What are the key benefits of using a Django Custom User Model, and how does it differ from the default Django User Model?


A Django Custom User Model offers flexibility, scalability, compatibility, and security advantages over the default User model. It allows you to tailor the user model to fit your project's unique requirements, integrate with existing data, and provide a solid foundation for future development.


### Q2. Explain the process of creating and implementing a Custom User Model in Django, including the necessary changes to settings.py and the required model fields.

#### To create and implement a Custom User Model in Django:

- Create a new Django app (custom_user).
- Define the Custom User Model by subclassing AbstractBaseUser and PermissionsMixin, and add the desired fields.
- Create a custom User Manager class by subclassing BaseUserManager and associate it with the Custom User Model.
- Update the AUTH_USER_MODEL setting in settings.py to point to your Custom User Model.
- Create and apply database migrations.
- Update references to the default User model in your codebase.
- Utilize the Custom User Model for authentication and authorization.


### Q3. What is DjangoX and how does it complement or extend the functionality of Django? Provide an example use case for incorporating DjangoX in a project.

DjangoX is a package that extends Django's functionality by providing pre-built components for authentication, user profiles, social authentication, and admin interface enhancements. It simplifies development tasks, saves time, and improves productivity in Django projects.


