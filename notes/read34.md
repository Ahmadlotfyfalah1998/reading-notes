[githup](https://ahmadlotfyfalah1998.github.io/reading-notes/)
## Question 1: What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading?



Keep settings in separate modules for better organization.<br>
Use environment variables to store sensitive information like secret keys.<br>
Use the "local settings" approach to manage sensitive or environment-specific settings.<br>
Split settings into different files based on their purpose (e.g., base, development, production).<br>
Utilize the "dj-database-url" library for easier database configuration.<br>
Use "django-environ" to read environment variables and assign them to settings.<br>
Use "python-decouple" to separate configuration from code.<br>

## Question 2: How does the White Noise library contribute to the efficient serving of static files in a Django application, and what are the steps to integrate it into a project?

White Noise is a library that efficiently serves static files in a Django application.<br>
It can serve static files directly from the application, eliminating the need for a separate web server.<br>
It reduces the complexity and overhead of configuring a web server for static file serving.<br>
To integrate White Noise into a Django project, first, install the library using pip.<br>
Add "whitenoise.middleware.WhiteNoiseMiddleware" to the MIDDLEWARE setting in Django.<br>
Set the STATICFILES_STORAGE setting to "whitenoise.storage.CompressedManifestStaticFilesStorage."<br>
## Question 3: What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources?
CORS is a security feature to control access to resources on a web server from a different domain.<br>
It prevents unauthorized requests from domains other than the one serving the resources.<br>
To implement CORS in a Django project, first, install the "django-cors-headers" package.<br>
Add "corsheaders.middleware.CorsMiddleware" to the MIDDLEWARE setting in Django.<br>
Configure the CORS_ALLOW_ALL_ORIGINS setting to allow requests from specific domains or use "*" to allow all.<br>
Other CORS-related settings can be adjusted based on project requirements, such as allowing specific methods or headers.<br>
