# Read: Class 34

## API Deployment:

### Q1. What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading?

**the key principles for organizing and configuring Django settings:**

1. **Separation of Concerns**: Divide settings into separate files for better organization.
2. **Use Environment Variables**: Store sensitive data as environment variables.
3. **Import from Environment**: Import sensitive settings from environment variables.
4. **Use Constants**: Create a constants.py file for non-sensitive configuration values.
5. **Secure Sensitive Information**: Avoid hardcoding secrets and use tools like python-decouple.
6. **Conditional Importing**: Use try-except blocks for conditional loading of settings.
7. **Configuration Inheritance**: Allow settings files to inherit from each other.
8. **Default Settings**: Provide sensible defaults for smooth application operation.
9. **Use Settings Validators**: Implement validators for valid settings.
10. **Version Control and Documentation**: Include settings in version control, exclude secrets, and document thoroughly.
11. **Deployment Management**: Use tools like django-configurations for different environments.

### Q2. How does the White Noise library contribute to the efficient serving of static files in a Django application, and what are the steps to integrate it into a project?

WhiteNoise is a Django middleware that efficiently serves static files in a Django application. It compresses files, sets caching headers, and delivers files directly from memory.

**To integrate it:**


1. Install WhiteNoise: pip install whitenoise
2. Update Django settings: Add 'whitenoise.middleware.WhiteNoiseMiddleware' to the MIDDLEWARE setting.
3. Configure static files: Set STATIC_URL and STATICFILES_STORAGE.
4. Collect static files: Run python manage.py collectstatic.
5. No need to configure a separate web server; WhiteNoise handles static file serving within Django.

### Q3. What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources?

CORS (Cross-Origin Resource Sharing) is a web securiaty feature to control cross-origin requests. 

**To enable CORS in a Django project:**

1. Install django-cors-headers: pip install django-cors-headers
2. Configure settings: Add 'corsheaders' to INSTALLED_APPS, and 'corsheaders.middleware.CorsMiddleware' as the first middleware in MIDDLEWARE.
3. Specify allowed origins: Set CORS_ALLOWED_ORIGINS to a list of allowed domains or use '*' for any origin.
4. Optionally, configure other settings like CORS_ALLOW_CREDENTIALS, CORS_ALLOW_METHODS, and CORS_ALLOW_HEADERS.
5. Exempt CSRF cookie (if using CSRF protection): Add CSRF_COOKIE_SAMESITE = None to settings.py.
6. Restart Django server.
