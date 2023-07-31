## Question 1: What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading?



Keep settings in separate modules for better organization.
Use environment variables to store sensitive information like secret keys.
Use the "local settings" approach to manage sensitive or environment-specific settings.
Split settings into different files based on their purpose (e.g., base, development, production).
Utilize the "dj-database-url" library for easier database configuration.
Use "django-environ" to read environment variables and assign them to settings.
Use "python-decouple" to separate configuration from code.

## Question 2: How does the White Noise library contribute to the efficient serving of static files in a Django application, and what are the steps to integrate it into a project?

White Noise is a library that efficiently serves static files in a Django application.
It can serve static files directly from the application, eliminating the need for a separate web server.
It reduces the complexity and overhead of configuring a web server for static file serving.
To integrate White Noise into a Django project, first, install the library using pip.
Add "whitenoise.middleware.WhiteNoiseMiddleware" to the MIDDLEWARE setting in Django.
Set the STATICFILES_STORAGE setting to "whitenoise.storage.CompressedManifestStaticFilesStorage."
## Question 3: What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources?
CORS is a security feature to control access to resources on a web server from a different domain.
It prevents unauthorized requests from domains other than the one serving the resources.
To implement CORS in a Django project, first, install the "django-cors-headers" package.
Add "corsheaders.middleware.CorsMiddleware" to the MIDDLEWARE setting in Django.
Configure the CORS_ALLOW_ALL_ORIGINS setting to allow requests from specific domains or use "*" to allow all.
Other CORS-related settings can be adjusted based on project requirements, such as allowing specific methods or headers.
