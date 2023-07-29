[hithup](https://ahmadlotfyfalah1998.github.io/reading-notes/)
## Q1.What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?
Purpose: JWTs are used for secure transmission of information between parties as JSON objects.m<br>
Their primary purpose is to enable stateless authentication and authorization in web applications.<br>
Encoding and Decoding: JWTs consist of three parts separated by periods: header, payload, and signature.<br>
The header specifies the algorithm used, the payload contains the user-specific data, and the signature ensures data integrity.<br>
To create a JWT, the data is encoded using Base64Url encoding and signed using a secret key. On the receiving end,<br>
the signature is verified to ensure data integrity and authenticity.<br>



## Q2.How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?
Integration: Django REST Framework (DRF) supports JWT authentication out of the box.<br>
You can use third-party libraries like djangorestframework-simplejwt to easily implement JWT authentication in your Django project.<br>
Key Components: The process involves configuring the authentication settings in DRF settings.py, <br>
including the JWT-specific settings like token expiration time and refresh token settings.<br>
Users can obtain tokens by authenticating using their credentials, and the tokens are then sent with subsequent API requests to access protected endpoints.<br>



## Q3.Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?
Limitations: Django's built-in development server (runserver) is not suitable for production environments due to its lack of performance <br>
optimizations and security features. It is only designed for development purposes.<br>
Alternatives: For deploying a Django application in production, you should consider using production-ready web servers like Gunicorn, uWSGI,<br>
or Apache with mod_wsgi. These servers are capable of handling high traffic, offer better performance, and provide additional security features.<br>
Additionally, using reverse proxies like Nginx in front of the application server can further improve performance and security.<br>
These alternatives ensure the Django application is ready for real-world production usage.<br>

## Things I want to know more about
1.JWT<br>
