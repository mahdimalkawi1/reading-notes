# Read: Class 33

## Authentication & Production Server:

### Q1. What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?

JSON Web Tokens (JWTs) are compact tokens used for secure data transmission. Their primary purpose is authentication and authorization. JWTs consist of three parts: header, payload (claims), and signature. The header and payload are Base64URL encoded, and the signature ensures data integrity. Servers encode data into JWTs for transmission and decode them to validate and access the information. JWTs are widely used in web apps for stateless communication and secure data exchange.

### Q2. How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?

JWT Authentication integrates with Django REST Framework (DRF) to secure API endpoints. Key components involved:

* **DRF**: Django REST Framework is used for building APIs in Django.

* **JWT Library**: Use "djangorestframework-simplejwt" for JWT support.

* **Settings**: Configure DRF in settings.py to include JWT authentication.

* **User Authentication**: Add authentication classes to views or viewsets.

* **Obtain JWT Token**: Clients get a token by authenticating with credentials.

* **Use JWT Token**: Include the token in the "Authorization" header.

* **Validation**: DRF automatically validates the token, granting access if valid and not expired.

### Q3.Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?

Django's runserver is not suitable for production due to security, performance, and reliability limitations. For production, consider using Gunicorn, uWSGI, Nginx, Apache with mod_wsgi, Docker with orchestration, or cloud-based platforms like Heroku, AWS Elastic Beanstalk, or Google App Engine. These options provide better performance, security, and scalability.




